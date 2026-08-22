# DQ1-M0 Control-Development Charter

## Comparator Families, Builders, Competence, Budgets, and Veto Rights

**Document type:** DQ1-M0 required artifact (Doc 08 §§6.4, 17, 18.1, 26; Doc 07 §4.2)
**Version:** 0.1 — Draft for four-role review plus control-builder approval
**Date:** 22 August 2026
**Candidate bounded by this charter:** PDSGRO-0.1 under attribution label `generic_sanskrit_inspired_scope_machinery`

---

# 1. Purpose and Binding Principle

This charter guarantees that when PDSGRO-0.1 is compared against anything, the comparison is fair by construction:

> Every comparator receives the **same neutral source bundle**, the **same task theory**, the **same evaluation interface**, **equivalent engineering resources**, and must pass **absolute competence tests before any comparative result is unsealed**.

Doc 08 §6.4 presumption governs throughout: *if a target implementation and a competent generic implementation return different logical answers under genuinely identical information and semantics, the first presumption is an implementation defect or failed information equivalence — not target superiority.*

---

# 2. Mandatory Comparator Formulations

| ID | Formulation | Required by | Build gate |
|---|---|---|---|
| U | **Universal linguistic structure**: information-equivalent feature/inheritance organization statable without Sanskrit terminology (e.g., typed feature hierarchies with default inheritance) | Doc 08 §26; Doc 07 §4.2 | Specified at M2, implemented+tested at DQ3 |
| G | **Generic executable scope machinery**: scoped rule engine (agenda-group/context analogue) with defaults, exceptions, precedence, blocking, optionality — closest prior-art composition from Kill Screen F2+F7+F10+F11+F12 | Doc 08 §§6.4, 26 | Specified at M2; its **interface approval** is required before M0 Freeze (§18.1) |
| A | Anonymized-label variant (topology preserved, labels replaced by opaque IDs) | §26; Doc 07 §4.2 | Specified M2, built DQ3 |
| C | Well-formed counterfactual structure (valid alternative organization, predicted to change target conclusions) | §26; Doc 07 §4.2 | Specified M2, built DQ3 |
| X | Type-preserving shuffled/corrupted structure | §26; Doc 07 §4.2 | Specified M2, built DQ3 |

M0 Freeze requires: **both the G and U builders approve the minimal representation-neutral I/O contract (§3)** and the competence-test specifications (§5) — Doc 08 §18.1 names universal *and* generic control builders as approvers. U/A/C/X specification ownership is assigned now; their construction follows at M2/DQ3.

---

# 3. Minimal Representation-Neutral Input/Output Contract

Every formulation consumes and emits exactly:

~~~text
INPUT : neutral source bundle B, valid against schemas/source_bundle.schema.json
OUTPUT: (i) condition-specific compiled instance (formulation's own schema,
        registered in the version/hash manifest),
        (ii) Decode_X specification with exact round-trip obligation
              Decode_X(Compile_X(B)) ≡ B  over the declared consequence language,
        (iii) resource-counter report using the common counter vocabulary
              (Doc 08 §21 counter names),
        (iv) provenance manifest entries (builder, tool versions, hashes).
~~~

Binding clauses:

1. **No target-only mandatory state.** No formulation may be required to populate or consume any field whose meaning is defined only by PDSGRO internals. If a field is mandatory in the shared interface, it must be derivable from B alone.
2. **Symmetric visibility.** Identical field-visibility classes apply to every formulation (model-visible / compiler-visible / evaluator-only / provenance-only, Doc 08 §9.5).
3. **Identical evaluator contact surface.** Query format (`skeptical-v1` ground literals) and output aggregation semantics are shared verbatim.
4. **Interface freeze discipline.** Post-approval changes require builder consultation; builders hold veto rights (§7).

---

# 4. Independent Builders

| Family | Builder requirement | Independence |
|---|---|---|
| G (generic) | ≥1 engineer unaffiliated with PDSGRO design/implementation | Not mechanism owner; not target implementer; discloses prior collaboration |
| U (universal) | ≥1 linguist-or-engineer pair able to state feature-hierarchy equivalents | Same |
| A/C/X | May share one builder team distinct from G | Same |

AI assistance is permitted under the reviewer-playbooks Tier-2 policy: AI may draft; the named human builder verifies and owns the verdict, disclosing tool use. Correlated-blindness mitigation applies (different model/vendor than authored the target artifacts).

Builders receive, symmetrically and simultaneously: B bundles, both JSON Schemas, public fixtures F01–F16 + oracles, Compile_T spec, TreatmentSignature, kill screen, and the owner's **pre-freeze engineering-disclosure register** (§6).

---

# 5. Absolute Competence-Test Specifications

Each formulation must pass ALL of the following before any comparative result involving it is unsealed:

| # | Test | Threshold |
|---|---|---|
| CT-1 | Schema conformance of emitted instances | 100% structural validity |
| CT-2 | Round-trip `Decode_X(Compile_X(B)) ≡ B` over declared domain (public witness cases) | Exact, 100% |
| CT-3 | **Expressibility witnesses:** every valid public fixture scenario (F01–F13, F15, F16) re-expressible in the formulation, yielding the **same aggregated query statuses** where the outcome is formulation-independent semantic content; F14 malformed variants are governed by CT-4 fail-closed expectations, and F15's exhaustion semantics are compared through the shared counter vocabulary rather than engine-specific limits | Exact match on all in-scope fixtures |
| CT-4 | Execution-equivalence spot check: independent engine (or denotational oracle) runs the compiled formulation on fixture scenarios; divergence from expected statuses triggers defect-vs-equivalence review, never silent reinterpretation | All divergences resolved before unseal |
| CT-5 | Counter parity: resource counters reported in shared vocabulary with documented counting rules | Complete, no missing categories |
| CT-6 | Provenance completeness (builder identity, hashes) | Complete |

CT-3 is deliberately absolute: partial competence cannot enter a sealed comparison (mirrors §16.4's exact-conformance rule).

---

# 6. Symmetric Resources and Budget Parity

1. **Pre-freeze disclosure register.** Before M0 Freeze, the mechanism owner records all PDSGRO-specific engineering hours (specification, schemas, fixtures) in the cost-ledger labour format (Doc 08 §21.4 tags: `target_specific`, stage `exploratory`). This register is delivered to every builder.
2. **Matching budget with sufficiency floor.** Each comparator family receives an engineering-hour envelope ≥ the target's disclosed same-stage spend **and** ≥ the methods-reviewer-certified minimum sufficient to reach CT-1…CT-6 competence for that family — whichever is greater. Parity to an under-resourced target is never an excuse; allocated by the methods reviewer from the programme budget. Under-resourcing a control below the disclosed-target level is a charter violation and voids affected comparisons.
3. **Equal post-freeze search.** After interfaces freeze, all formulations receive identical tuning/search budgets, seeds, and compute envelopes; deviations require a preregistered amendment.
4. **Data/expert symmetry.** Annotation questions, Sanskrit-reviewer consultations (where a formulation needs linguistic grounding), and clarification channels are answered through the same shared channel with responses visible to all builders.

---

# 7. Baseline-Challenge and Veto Rights

| Right | Holder | Scope |
|---|---|---|
| Interface veto | Any named builder, before M0 Freeze | Reject a proposed contract clause that mandates target-only state or asymmetric visibility; veto blocks freeze until resolved |
| Competence-challenge | Any builder, at any gate | Demand re-run of CT-1…CT-6 for any formulation (including the target) with fresh witness cases drawn by the custodian |
| Unfairness escalation | Any builder | Escalate to the independent methods reviewer; unresolved findings pause the affected gate (Doc 07 §8.4 pause rules apply mutatis mutandis) |
| Prior-art subtraction challenge | U/G builders | Contest the kill screen's residual claims R1–R4 in writing; contested residuals go to the methods reviewer before DQ7 designs lock |

Exercising any right is a **protected activity**: no budget, access, or attribution penalty may attach to a builder for vetoes or challenges.

---

# 8. Workflow to M0 Freeze

1. Owner delivers disclosure register + artifact pack to candidate builders.
2. G builders review §3 contract; iterate until approved or vetoed clauses are repaired.
3. U/A/C/X builder assignments recorded (names may follow post-freeze for build-phase roles, but G-interface approvers sign the freeze package).
4. All approvals recorded in the freeze package with hashes alongside the four governance-role signatures (Doc 08 §23.2).

---

# 9. Review Checklist

- [ ] Four governance roles approve charter within quorum hash
- [ ] G builders approve §3 contract explicitly (named signatures)
- [ ] Disclosure register populated and transmitted before freeze
- [ ] Budget-parity mechanism confirmed by methods reviewer
- [ ] CT-1…CT-6 accepted as absolute gates in writing by all builders

---

# 10. Amendment Log

| Version | Date | Change | Author | Status |
|---|---|---|---|---|
| 0.1 | 22 August 2026 | Initial charter: five formulations, neutral I/O contract, six competence tests, parity economics, veto rights | AI-drafted (opencode agent) | Draft — unverified |
