# DQ1-M0 Compile_T Specification

## Deterministic Target Compiler for PDSGRO-0.1

**Document type:** DQ1-M0 required artifact (Doc 08 §§6.1, 8.2, 9, 17)
**Version:** 0.1 — Draft skeleton for reviewer verification
**Date:** 21 August 2026
**Companion artifacts:** 10_M0_TreatmentSignature_v0.1.md (organizational constraints); 09_M0_Prior_Art_Kill_Screen_Matrix_v0.1.md
**Authority:** Document 08 §8.2 compiler obligations; §9 schema minimum; §10.1 validation

---

# 1. Compiler Identity and Obligations

~~~text
compiler_id:   Compile_T
input:         neutral source bundle B = (Σ, V, F_N, A_N, K_N, T, Q)
output:        compiled instance I_m = (Σ, V, F_m, A_m, K_m, S_m, H_m,
               R_m, E_m, X_m, P_m, O_m, Z_m, Q) + ModelPayload
attribution:   generic_sanskrit_inspired_scope_machinery
~~~

Compile_T **must be**:

| Obligation | Definition | Verified by |
|---|---|---|
| O1 Total | Defined behaviour over every input satisfying the source schema | schema-conformance sweep |
| O2 Deterministic | Same input + configuration ⇒ byte-identical output | replay tests |
| O3 Gold-blind | No access to evaluator oracle files at compile or run time | I/O capability audit |
| O4 Versioned + hashed | CompilerManifest with all hashes (§6) | freeze package |
| O5 Semantics-preserving | `Decode_T(Compile_T(B)) ≡ B` over declared consequence language | round-trip witness |
| O6 Non-inventive | May normalize/factor/index/rename/reorder; may not author, infer, retrieve, delete, or add any predicate, literal, condition, relation, or consequence | diff audit vs B |
| O7 Query/runtime-independent | Replacing Q or K_N leaves every structural field unchanged except copied request-context/mapped-anchor fields | metamorphic tests M-Q, M-K |

Failure of O5–O7 on any witness is a compiler defect, never a silent repair.

---

# 2. Pipeline Stages

~~~text
S0  Load & parse B                    → typed object graph
S1  Validate source                   → reject INVALID_SOURCE (fail closed)
S2  Context mapping                   → F_m, A_m, K_m        [MT-1, MT-2]
S3  Scope forest construction         → S_m                  [MT-3]
S4  Inheritance graph compilation     → H_m                  [MT-4]
S5  Rule stratification               → R_m (+ strata)       [MT-5]
S6  Control-object compilation        → E_m, X_m, P_m, O_m, Z_m [MT-6..MT-9]
S7  Provenance attachment             → source_refs on every compiled object
S8  Canonical serialization           → I_m + ModelPayload + hashes
~~~

Stage separation is normative: each stage's output is a checkable intermediate; no stage may read a later stage's output.

## 2.1 Stage contracts

- **S2 Context mapping:** bijective rename of neutral `ContextKey` values to condition-local scope identifiers; `AnchorIntent` maps to exactly one anchor scope. The mapping is recorded in MT-1/MT-2 and reversed by Decode_T.
- **S3 Scope forest:** one scope per distinct applicability context (TreatmentSignature factorization_policy). Rejects multi-parent, cycles, anchors outside the forest.
- **S4 Inheritance:** compiles \(T\) inheritance permissions into `InheritanceEdge`s with explicit `permitted_properties`; acyclicity enforced here.
- **S5 Stratification:** constructs the signed predicate-dependency graph and assigns strata per Doc 08 §10.1; any cycle containing a defeasible/control dependency rejects the instance.
- **S6 Controls:** exceptions target `(rule_id, substitution)` patterns; blocks name property + edge/path pattern; priority edges carry higher/lower substitution patterns + shared-argument alignment; optional groups validated non-overlapping with min ≤ max.

---

# 3. Decode_T Round-Trip Obligation

~~~text
Decode_T(Compile_T(B)) ≡ B          # full bundle equivalence
Decode_T(F_T, A_T, K_T) ≡ (F_N, A_N, K_N)   # explicit context-mapping clause
~~~

- Equivalence is **exact** over the declared consequence language: same predicates, arguments, polarity, context semantics, analyses, rules, controls, constraints, queries.
- Identifier renames are lawful only under the published inverse bijection (non-semantic renaming invariance, Doc 08 §11.15).
- The witness suite (public conformance cases) must pass before M0 Freeze; hidden acceptance cases remain sealed until M1 (Doc 08 §16.4).

---

# 4. Metamorphic Test Obligations

| ID | Transformation | Required invariance |
|---|---|---|
| M-Q | Replace Q, hold Σ,V,F_N,A_N,K_N,T fixed | All structural fields byte-identical |
| M-K | Replace runtime context / AnchorIntent, hold rest fixed | Structural fields unchanged except copied request-context + mapped-anchor fields |
| M-O | Permute semantically unordered records in B | Identical semantic projection of I_m |
| M-R | Apply non-semantic identifier bijection to B | Identical projection after inverse bijection |
| M-I | Add inactive-scope rule / disconnected fact | Affected projections unchanged |

M-Q/M-K failures indicate an answer-relevance topology created at compile time — prohibited (Doc 08 §8.2).

---

# 5. Mapping-Table Inventory

Each table is versioned, hashed, and reviewed; none may encode item-level judgment:

| Table | Content | Feeds stage |
|---|---|---|
| MT-1 ContextKey→ScopeID map | bijection derived from ContextKey definitions | S2/S3 |
| MT-2 AnchorIntent→anchor-scope policy | deterministic selection rule | S2 |
| MT-3 Scope-nesting rules | parent derivation from context generality ordering | S3 |
| MT-4 Inheritance-permission templates | T-statement form → InheritanceEdge fields | S4 |
| MT-5 Stratum assignment algorithm | dependency-graph construction + stratum function | S5 |
| MT-6 Exception-pattern grammar | T exception claim → grounded specification | S6 |
| MT-7 Block-pattern grammar | T block claim → Block fields | S6 |
| MT-8 Priority-alignment rules | substitution patterns + shared-argument alignment | S6 |
| MT-9 Optional-group bounds policy | choice bound derivation + overlap checks | S6 |

Generic-control symmetry obligation (Doc 08 §18.1): every table must have a declared counterpart available to universal/generic control compilers, with no target-only mandatory state in the shared interface.

---

# 6. CompilerManifest and Hash Structure

~~~text
CompilerManifest:
  compiler_id: "Compile_T"
  version: <semver>
  attribution_label: "generic_sanskrit_inspired_scope_machinery"
  treatment_signature_hash: <SHA256 of TreatmentSignature §2 block>
  source_schema_hash:       <SHA256>
  target_schema_hash:       <SHA256>
  mapping_hashes:
    MT-1: <SHA256> … MT-9: <SHA256>
  configuration_hash:       <SHA256 of frozen config>
  implementation_hash:      <SHA256 of implementation artifact>
~~~

Hash preimages use CanonicalJSON with the hash field omitted from its own preimage (Doc 08 §19.4 convention).

---

# 7. Error Handling

| Condition | Result |
|---|---|
| Source schema violation, duplicate IDs, unbound variables | `INVALID_SOURCE`, fail closed |
| Scope/inheritance/priority cycles; multi-parent scope | `INVALID_SOURCE` with cycle report |
| Stratification failure (defeasible/control cycle) | `INVALID_SOURCE` with dependency-graph excerpt |
| Overlapping optional groups, impossible bounds | `INVALID_SOURCE` |
| Missing mapping-table entry for a lawful T-statement form | compile error — **never** discretionary fallback |

The interpreter downstream re-validates the compiled instance independently (Doc 08 §10.1); compiler success does not imply interpreter acceptance.

---

# 8. Implementation Notes (Non-Normative)

Recommended: small pure-Python module, JSON in/out, no external services, stdlib hashing; ~15 modules mirroring Doc 08 §19.3. Implementation begins only as disposable feasibility exploration until M0 Freeze + hidden-set custody are complete (Doc 08 §27).

---

# 9. Reviewer Verification Checklist

1. Methods reviewer: confirm O5–O7 witnesses fully specified; confirm MT tables contain no item-level discretion.
2. Implementation reviewer: confirm stage separation and fail-closed errors are implementable as specified.
3. Control-builders: approve that the shared interface exposes nothing target-only (§5 symmetry note).
4. All: verify hash manifest binds this spec to TreatmentSignature v0.1 and both schemas.

---

# 10. Amendment Log

| Version | Date | Change | Author | Status |
|---|---|---|---|---|
| 0.1 | 21 August 2026 | Initial skeleton: obligations, stages, Decode_T, metamorphics, MT inventory, manifest | AI-drafted (opencode agent) | Draft — unverified |
