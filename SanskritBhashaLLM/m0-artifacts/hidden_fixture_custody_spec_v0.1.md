# DQ1-M0 Hidden-Fixture Generation and Custody Specification

## M0 Required Artifact (Doc 08 §16.4; §20.1; §23.4)

**Version:** 0.1 — Draft for four-role review
**Date:** 21 August 2026
**Governs:** the sealed M1 acceptance set only. Public golden fixtures F01–F16 are development data and outside this specification's custody.

---

# 1. Roles and Separation of Duties

| Role | Holder | Duties |
|---|---|---|
| Custodian | **TBD before M0 Freeze** (must not be mechanism owner or any M1 implementer) | Generates seeds + hidden set, maintains manifest and access log, executes unseal event |
| Independent oracle author | **TBD**, separate from interpreter implementation | Implements the denotational reference oracle in a **disjoint codebase** (recommended: different language, e.g., Haskell/Rust vs Python interpreter) |
| Implementer | M1 engineer | May know schema, operator inventory, fixture families, invariants, resource bounds (§16.4). May NOT see instance contents, gold outputs, mutation choices, or acceptance results before the unseal event |
| Witness | One external party (e.g., methods reviewer delegate) | Countersigns the manifest; verifies escrow integrity at unseal |

Production interpreter code may never serve as its own oracle (§20.1).

---

# 2. Generator Specification

## 2.1 Deterministic parameterized generator

A pure function `generate(seed, params) → compiled_instance + expected_audit`, emitting instances that satisfy `compiled_instance.schema.json` and pass all §9–§10 static validity rules (so every generated case is *valid* unless drawn from the adversarial-invalid stratum).

## 2.2 Supported domain bounds (frozen at M0 Freeze)

| Parameter | Bound |
|---|---|
| entities | ≤ 12 |
| scope forest depth / total scopes | ≤ 4 / ≤ 8 |
| inheritance DAG nodes / edges | ≤ 8 / ≤ 12 |
| strata | ≤ 3 |
| rules (strict+default) | ≤ 15 |
| analysis groups × members | ≤ 3 groups × 3 members |
| optional groups | ≤ 2, each 2–3 members |
| derived branch ceiling per instance | ≤ 64 (branch_limit set to exactly the computed product when exercising F15-style exhaustion) |
| predicates / arity | ≤ 8 / ≤ 3 |

## 2.3 Operator-combination coverage matrix

Every cell below requires ≥ n samples (n = sample counts, §4). Operators: Sc(scope), In(inheritance), Bl(block), Dd(default), Ex(exception), Pr(priority), Op(optional group), An(analysis group ≥2), Cn(constraint), Ng(strict negation head).

- **Positive combinations (must co-occur meaningfully):** Sc+In, In+Bl, Dd alone, Dd+Ex, Dd+Pr, Dd+Ex+Pr, An+Op (branch products), An+Cn, Sc+Dd+Ex, In+Bl+Dd+Ex (F16-shape).
- **Boundary:** zero-group single-branch instance; maximal-depth scope chain; inheritance width at bound; priority chain length 3 with ordering-only transitive pair; optional group at min=max.
- **Adversarial-invalid (fail-closed):** scope cycle, inheritance cycle, priority supergraph cycle, defeasible dependency cycle, overlapping optional groups, anchor outside forest, non-GLOBAL self-activation fact, constraint referencing unsettled stratum.
- **Resource:** instances engineered so a named counter hits its frozen limit (per §10.7) — one per counter type {logical_steps, grounded_applications, inheritance_paths, branches, trace_events}.

---

# 3. Independent Denotational Oracle

- Direct implementation of Doc 08 §§10.2–10.8 semantics by brute force: explicit branch enumeration, per-branch fixed-point evaluation in stratum order, Belnap-style TRUE/FALSE/NEITHER/BOTH states, skeptical-v1 aggregation.
- Emits the full semantic projection (query statuses, branch states, grounded-application statuses, conflicts) but **not** the deterministic trace prefix (trace is interpreter-owned; oracle asserts trace *properties* only where specified in fixtures' oracle format).
- Acceptance comparison is on the **semantic projection**: exact equality, no tolerance.
- Oracle must reproduce all 16 public fixture results before sealing (sanity gate), then be locked and hashed.

---

# 4. Sample Counts and Acceptance Threshold

| Stratum | Samples |
|---|---|
| Each positive-combination cell | ≥ 5 |
| Boundary family | ≥ 1 per listed boundary case (7 cases) |
| Adversarial-invalid family | ≥ 2 per failure mode (8 modes ⇒ ≥ 16) |
| Resource-exhaustion per counter | ≥ 1 (5 counters) |

**Acceptance threshold (exact, §16.4):** semantic conformance **100%** — every valid hidden instance matches the oracle exactly; every invalid instance fails closed with the expected error code. Any single mismatch ⇒ M1 Fail. Percentage thresholds govern nothing semantic; they apply only to diagnostic coverage reporting.

**Mutation adequacy (§20.3):** the curated mutant set below must be **100% killed** (each mutant causes ≥1 hidden-case mismatch); sampled structural mutants additionally reported with score ≥ 90% as diagnostics:

Mutants: disable scope check; ignore permitted_properties; drop block evaluation; treat default as strict; exception matches rule-level instead of grounding-level; skip priority filtering order; collapse BOTH→TRUE; aggregate credulously; allow sibling grounding defeat; skip canonical sort before hash; accept cyclic scopes; skip GLOBAL-only activation restriction.

---

# 5. Seed Generation, Commitment, Escrow

1. Custodian generates 256-bit master seed via CSPRNG **after** this spec and the generator are frozen.
2. Custodian publishes `SHA256(master_seed)` as a **commitment** inside the sealed manifest *before* implementation begins; master seed itself stays encrypted-at-rest (age/GPG to custodian + witness keys).
3. Per-instance seeds derive as `SHA256(master_seed || "instance" || index)`; mutation-selection seeds similarly namespaced. Derivation scheme is published; derivation is verifiable post-unseal.
4. Escrow: master seed shares Shamir 2-of-2 between custodian and witness; neither can unseal alone pre-event.

---

# 6. Cryptographic Manifest (sealed at generation)

~~~json
{
  "spec_version": "hidden-fixture-custody v0.1",
  "contract_version": "Doc 08 v0.2 normative hash",
  "generator_version_and_hash": "<...>",
  "seed_commitment": "<sha256>",
  "fixture_hashes": {"<index>": "<sha256 of instance>"},
  "oracle_hash": "<sha256>",
  "expected_result_hashes": {"<index>": "<sha256 of semantic projection>"},
  "custodian": "<name/keyid>", "witness": "<name/keyid>",
  "generated_at": "<iso8601>", "unseal_event": null
}
~~~

Manifest is signed by custodian + witness; stored append-only in `m0-artifacts/sealed/` (git + offline copy).

---

# 7. Access Control, Unseal Event, Leak Handling

- **Access rights:** implementer reads only this spec + public fixtures. Repository path `m0-artifacts/sealed/` blocks via CODEOWNERS/review gate until unseal.
- **Unseal event (exact):** (a) M0 Frozen with quorum hash recorded, AND (b) implementer declares acceptance-readiness in writing, AND (c) custodian + witness co-sign the unseal record. First unseal is immutable (§16.4); disclosed failures make that set development data.
- **Reruns:** require newly generated sealed set under a fresh seed commitment; prior results remain in the decision-record history (never deleted, never reused as lottery tickets).
- **Leak/invalidation:** any evaluator-only content entering compiler, payload, cache, training artifact, or selection rule invalidates the affected run (§14.4); recorded leak ⇒ regenerate; access log is append-only and auditable.
- **Result history:** every generation/unseal/rerun appended to `decision_record` with hashes; retained across contract versions.

---

# 8. Disjointness Rules

| Dataset | Content | Rule |
|---|---|---|
| Development | Public fixtures F01–F16 + generator smoke samples (≤10, owner-visible) | Never counted toward acceptance |
| M1 acceptance | Sealed hidden set (this spec) | Custodian-only until unseal |
| DQ5–DQ10 scored items | Separate pipeline, separate seed namespace `"dq5+"`, independent builders | No instance may share (bundle_hash ∩ acceptance_set) ≠ ∅ — enforced by hash registry diff at each gate |

---

# 9. Review Checklist

- [ ] Four roles approve this spec within the M0 freeze package quorum
- [ ] Custodian + witness named with keys before generation
- [ ] Oracle passes all public fixtures, then is hashed and locked
- [ ] Manifest fields complete; commitment published pre-implementation
- [ ] Disjointness registry query written and rehearsed on dummy sets

---

# 10. Amendment Log

| Version | Date | Change | Author | Status |
|---|---|---|---|---|
| 0.1 | 21 August 2026 | Initial custody spec: bounds, coverage matrix, thresholds, seeds/escrow, manifest, unseal, disjointness | AI-drafted (opencode agent) | Draft — unverified |
