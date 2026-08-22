# DQ1-M0 TreatmentSignature

## Frozen Organizational Constraints of the Candidate Mechanism

**Document type:** DQ1-M0 required artifact (Doc 08 §§6.1, 9, 17)
**Version:** 0.1 — Draft for reviewer verification
**Date:** 21 August 2026
**Candidate:** PDSGRO-0.1 (identifier immutable per Doc 08 §22.1)
**Attribution label carried by this signature:** **Generic Sanskrit-inspired scope machinery** (route selected per Prior-Art Kill Screen Matrix v0.1 §6.2; provisional until methods-reviewer ratification at M0 Freeze)
**Authority:** Document 08 §6.1; Document 07 information/leakage contract

---

# 1. Purpose and Route Decision

Doc 08 §6.1 requires this signature to state the complete target-only constraints on scope construction, factorization, indexing, inheritance organization, exception organization, block placement, priority representation, optional-choice representation, and the mediator each constraint is predicted to change — every constraint statable **without Sanskrit terminology** and derivable from the neutral source bundle without item-level discretionary judgment.

The Prior-Art Kill Screen Matrix v0.1 found every candidate primitive covered at kill or strong level by prior generic families, with residuals R1–R4 classifiable as tightened parameterizations. Accordingly this signature freezes the candidate as **generic executable scope machinery**, with Pāṇinian mappings retained as inspiration-only provenance (§5). This satisfies Doc 08 §6.1's relabel condition voluntarily rather than after contested review.

**What this signature does not claim:** algorithmic novelty, Sanskrit-specific causation, historical authenticity of any mapping, or any usefulness/efficiency result. Those remain with later gates (DQ7 adjudicates attribution empirically regardless of this label).

---

# 2. Normative Signature (Machine-Readable)

~~~yaml
treatment_signature:
  version: "0.1-draft"
  candidate_id: "PDSGRO-0.1"
  attribution_label: "generic_sanskrit_inspired_scope_machinery"
  scope_policy:
    structure: "rooted_forest_single_parent"
    activation: "condition_evaluated_root_to_anchor"
    activation_inputs: ["GLOBAL_context_facts", "compiled_request_context", "branch_analysis_bindings"]
    anchor_rule: "one_compiled_scope_anchor_per_request"
    path_validity: "complete_root_to_anchor_path_must_be_active"
    self_activation_restriction: "scoped_facts_may_not_activate_their_own_scope"
    isolation: "off_path_sibling_scopes_never_exchange_facts"
  factorization_policy:
    derivation: "scopes_derived_only_from_neutral_ContextKey_semantics_and_task_theory_structure"
    prohibition: "no_query_conditioned_or_runtime_conditioned_compilation"
    granularity: "one_scope_per_distinct_applicability_context_declared_in_source_bundle"
  topology_constraints:
    scope_graph: "finite_rooted_forest_max_one_parent_per_non_root_scope"
    inheritance_graph: "finite_directed_acyclic"
    priority_supergraph: "acyclic_over_unconditional_edges"
    optional_groups: "bounded_non_overlapping_min_leq_max_choices"
  indexing_policy:
    rule_index: "by_scope_then_stratum_then_rule_id"
    application_enumeration: "total_substitutions_over_typed_domain_only"
    fact_visibility_index: "per_scope_global_plus_active_ancestor_path"
  inheritance_policy:
    transmission: "property_reaches_target_iff_at_least_one_permitted_path_unblocked"
    permission_granularity: "permitted_properties_listed_per_edge"
    block_evaluation_order: "all_blocks_before_any_materialization"
    commitment: "unblocked_path_support_committed_as_indefeasible_branch_support"
    prohibited_defaults: ["child_override", "parent_order", "shortest_path", "file_order"]
  exception_policy:
    target_granularity: "exact_grounded_pair_rule_id_substitution"
    evaluation_snapshot: "frozen_lower_stratum_snapshot_only"
    defeat_scope: "named_application_only_no_sibling_grounding_defeated"
  priority_representation:
    form: "conditional_edges_between_grounded_default_applications"
    head_constraint: "exact_polarity_complement_heads"
    alignment: "frozen_higher_lower_substitution_patterns_with_shared_argument_alignment"
    instantiation_timing: "after_exception_and_indefeasible_support_filtering"
    tie_handling: "equal_or_incomparable_opposite_defaults_remain_CONFLICT"
  optional_choice_representation:
    enumeration_timing: "pre_inference_cartesian_product_with_analysis_groups"
    inapplicable_selections: "remain_selected_visible_and_non_generating"
    overlap: "prohibited"
  predicted_mediators:
    scope_policy: "irrelevant_rule_activation_decrease"
    factorization_policy: "active_structural_context_size_decrease"
    indexing_policy: "irrelevant_rule_activation_decrease"
    inheritance_policy: "invalid_candidate_propagation_decrease"
    exception_policy: "invalid_candidate_propagation_decrease"
    priority_representation: "avoidable_branching_decrease"
    optional_choice_representation: "avoidable_branching_decrease"
  residual_claims_carried_forward: ["R1", "R2", "R3", "R4"]  # see Kill Screen Matrix v0.1 §6
~~~

---

# 3. Constraint-to-Mediator Traceability

| # | Constraint family | Predicted mediator (Doc 08 §5.3 vocabulary) | Later intervention witness (DQ5/DQ6) |
|---|---|---|---|
| C1 | Scope activation + isolation | Irrelevant rule activation | Moving one rule across a scope boundary changes only in-scope conclusions |
| C2 | Factorization from ContextKey only | Active structural context size | Adding inactive-scope rule leaves semantic projection unchanged |
| C3 | Forest + acyclicity topologies | Determinism/termination (guard) | Cycle fixtures F14 fail closed |
| C4 | Scope+stratum indexing | Irrelevant rule activation | Activation-set difference observable in audit |
| C5 | Path-permission inheritance + pre-materialization blocks | Invalid candidate propagation | Removing a block propagates exactly the formerly blocked property |
| C6 | Grounded-instance exceptions | Invalid candidate propagation | Removing one exception produces predicted over-propagation; sibling groundings unchanged |
| C7 | Post-filter priority instantiation | Avoidable branching | Reversing one priority edge flips only the targeted conflict |
| C8 | Pre-inference optional enumeration | Avoidable branching | Removing optionality collapses exactly the declared alternatives |

Every row must map to at least one golden fixture (F01–F16) and one metamorphic mutation before M0 Freeze (Doc 08 §13 causal traceability contract).

---

# 4. Derivability and Non-Discretionary Compilation

Each target structure is produced by Compile_T from the neutral bundle under §2:

- scopes ← partition of neutral `ContextKey` values plus theory-declared applicability contexts;
- activation conditions ← request-context predicates and `GLOBAL` fact references present in \(B\);
- inheritance edges, permissions, blocks, exceptions, priorities, optional groups ← direct compilations of corresponding \(T\) statements;
- strata ← the signed dependency-graph algorithm fixed in Doc 08 §10.1.

No stage may consult queries, runtime context, gold data, or item-level human judgment. Violations are INVALID_INSTANCE or compiler-defect, never silent repair.

---

# 5. Inspiration Provenance (Non-Normative)

| Generic constraint (normative, §2) | Historical inspiration (non-normative) | Status after kill-screen subtraction |
|---|---|---|
| scope_policy | adhikāra-style governing context | Covered by agenda-groups/contextual LP; inspiration only |
| inheritance_policy | anuvṛtti-style context carry-over | Covered by inheritance networks/F-logic; inspiration only |
| exception_policy | utsarga–apavāda default-with-exception | Covered by defeasible logic/ASPIC+ undercutting; inspiration only |
| priority_representation | rule-order traditions | Covered by superiority relation/salience; inspiration only |
| optional_choice_representation | vā option markers | Covered by ASP choice rules; inspiration only (MC-5) |
| inheritance_policy.blocking | weak analogue: bādha-style override | No direct Aṣṭādhyāyī counterpart; proposed purely Generic pending MC-6 Relabel (MC-6) |
| carrier (held constant) | kāraka/event-role abstraction | Shared canonical carrier; no differential claim permitted (MC-7) |

Seven mapping cards (Doc 08 §16.3; see m0-artifacts/mapping_cards_v0.1.md) must cite the Sanskrit-computational prior art named in Kill Screen §4 (Huet Heritage engine, Saṃsādhanī simulator, Vidyut prakriyā) when documenting each mapping's computational correspondence.

---

# 6. Hash Manifest Structure

Frozen at M0 Freeze; placeholders until then:

~~~text
TreatmentSignatureHash := SHA256(CanonicalJSON(treatment_signature_block_above))
bound_to:
  compiler_specification_hash   # 11_M0_Compile_T_Specification
  mapping_table_hashes          # per-table SHA256, listed in Compile_T §5
  configuration_hash            # frozen compiler configuration
  source_schema_hash            # canonical source JSON Schema
  target_schema_hash            # compiled instance JSON Schema
~~~

Any change to §2 requires a new signature version, rehash, renewed reviews, and complete M1 replay (Doc 08 §23.5).

---

# 7. Reviewer Verification Checklist

1. Methods reviewer: confirm every §2 constraint is statable without Sanskrit terminology and none exceeds a generic compiler's expressive envelope (§6.1 relabel test — expected to pass *as Generic*).
2. Methods reviewer: confirm each §3 mediator prediction is falsifiable via the named fixture/mutation.
3. Sanskrit/Pāṇinian reviewer: confirm §5 accurately marks mappings as inspiration-only; approve or amend wording.
4. Implementation reviewer: confirm §4 derivability leaves no discretionary step.
5. Record ratification of the `attribution_label` in the M0 freeze package.

---

# 8. Amendment Log

| Version | Date | Change | Author | Status |
|---|---|---|---|---|
| 0.1 | 21 August 2026 | Initial signature on Generic route per Kill Screen v0.1 §6.2 | AI-drafted (opencode agent) | Draft — unverified |
