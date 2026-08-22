# Golden Fixtures DQ1-M0-F01 – F16

**Status:** Draft — bundles schema-validated; expected outputs are evaluator-only oracles pending independent verification.
**Authority:** Doc 08 §16 (fixture contract), §10 (operational semantics), §11 (invariants).

## Index

| Fixture | Isolates | Bundle | Oracle |
|---|---|---|---|
| F01 | Governing scope: inactive anchor + sibling isolation | `F01_scope_inactive.bundle.json` | `.oracle.json` |
| F02 | Inheritance: permitted property reaches child | `F02_inherited_context.bundle.json` | `.oracle.json` |
| F03 | Property-specific blocking; second path survives | `F03_property_block.bundle.json` | `.oracle.json` |
| F04 | Undefeated default fires | `F04_default_only.bundle.json` | `.oracle.json` |
| F05 | Grounded exception defeats only its named application | `F05_protected_exception.bundle.json` | `.oracle.json` |
| F06 | Acyclic priority chain, transitive closure, ordering-only pairs | `F06_precedence_chain.bundle.json` | `.oracle.json` |
| F07 | Incomparable opposite defaults → CONFLICT | `F07_precedence_tie.bundle.json` | `.oracle.json` |
| F08 | Optional group enumerates branches pre-inference | `F08_optionality.bundle.json` | `.oracle.json` |
| F09 | Analysis ambiguity aggregates AMBIGUOUS | `F09_ambiguity.bundle.json` | `.oracle.json` |
| F10 | Two groups → exact Cartesian product | `F10_two_analysis_groups.bundle.json` | `.oracle.json` |
| F11 | All branches rejected → NO_VALID_ANALYSIS | `F11_no_valid_analysis.bundle.json` | `.oracle.json` |
| F12 | Source/strict/default truth hierarchy and defeat rules | `F12_conflict_matrix.bundle.json` | `.oracle.json` |
| F13 | Constraint fires only at its declared stratum | `F13_derived_constraint.bundle.json` | `.oracle.json` |
| F14 | Malformed cycles fail closed (4 **compiled-instance** variants; §10.1 validator layer) | `F14_malformed_cycles.variants.json` | `.oracle.json` |
| F15 | Deterministic resource exhaustion at branch limit | `F15_resource_bound.bundle.json` | `.oracle.json` |
| F16 | Combined clean-room library world (Doc 08 §16.2 verbatim) | `F16_combined_clean_room.bundle.json` | `.oracle.json` |

## Conventions pinned by this suite

1. **Branch-local assumptions.** Analyses carry `assumed_fact_refs`; facts referenced there hold only in branches selecting that analysis (schema v0.1.1). This implements sense-dependent classification for F09/F11/F16.
2. **Request-context predicates.** Scope activation conditions may reference reserved zero-arity predicates derived from `request_context` fields (e.g. `ctx_special_collections()` ⇐ `request_context.special_collections = true`). The interpreter materializes these as request-context facts before scope evaluation.
3. **Class-node inheritance.** Object-to-object inheritance uses explicit class constants (e.g. `doctoral_class`) carrying the parent property as a GLOBAL fact.
4. **Oracle format.** Oracles are *property expectations*, not full audits: `expected_execution_status`, numbered assertions over audit properties, and the §11 invariants each fixture checks. The hidden acceptance generator remains a separate M0 artifact.
5. **F16 frozen query.** Exactly `q1 = may_borrow(researcher, vel)` per Doc 08 §16.2; expected aggregate `CONTRADICTED`.

## Validation status

- All 15 source bundles validate against `source_bundle.schema.json` v0.1.1; all 4 F14 variants validate against `compiled_instance.schema.json` v0.1.1 (cycles are compiled-layer objects). F14 manifests carry placeholder hashes until M0 freeze binds real ones.
- Oracles are structured JSON but intentionally NOT validated against `execution_audit.schema.json` (they express partial expectations).
- Independent methods reviewer must manually derive each fixture result before M0 Freeze (§18.1); discrepancies become blocking findings or oracle amendments.
