# DQ1 Mechanism Resolution Contract

## DQ1-M0 Specification Freeze and DQ1-M1 Deterministic Reference Interpreter

**Document version:** 0.2  
**Date:** 21 August 2026  
**Status:** Draft — Pass 2 red-team aligned; required artifacts and approvals remain missing; not Frozen  
**Governing question:** DQ1 — Mechanism Specification and Contribution Boundary  
**Current authority:** Document 06 journey order  
**Prospective DQ0 authority:** Document 07 Version 1 mission, exclusions, claim hierarchy, and falsification rules, effective only after DQ0 becomes Final/Yes

---

# 1. Purpose and Authority

This document defines the first two mechanism-resolution work packages required before DQ1 can pass:

- **DQ1-M0 — Mechanism Specification Freeze:** define exactly one executable candidate, its causal boundary, formal semantics, interfaces, costs, exclusions, fixtures, and review rules;
- **DQ1-M1 — Deterministic Reference Interpreter:** implement and test the frozen semantics without a language model.

These work packages are specification and feasibility work. They do not constitute a confirmatory experiment.

Document 07 records DQ0 as Provisional until the required approvals are entered. Therefore:

- this draft may be developed and reviewed;
- a reference implementation may be built as a feasibility artifact;
- no sealed confirmatory model comparison is authorized;
- neither M0 nor M1 may be described as proving usefulness, novelty, efficiency, reasoning improvement, or Sanskrit-specific causation.

While DQ0 remains unsigned, Document 06 controls journey order and this draft voluntarily conforms to Document 07 as the prospective mission authority. Once DQ0 becomes Final/Yes, Document 07 controls Version 1 scope, exclusions, public claims, and falsification. Any unresolved conflict pauses the affected decision.

---

# 2. Identifier Namespace

The identifiers **S0** and **S1** are not used for these work packages.

They already denote:

- Sanskrit text-only and Sanskrit-plus-serialized-structure conditions in the pilot; and
- different cumulative levels in the legacy structural ladder.

This document reserves:

| Identifier | Meaning |
|---|---|
| DQ1-M0 | Mechanism Specification Freeze |
| DQ1-M1 | Deterministic Reference Interpreter |
| DQ1-M2 | Reserved follow-on: information-equivalent formulations, prior-art closure, and complete DQ1 decision |

M0 and M1 are not new experimental phases. They are pre-confirmatory mechanism-resolution work packages under DQ1.

---

# 3. Compact Glossary

| Term | Meaning in this contract |
|---|---|
| neutral source bundle | Condition-independent typed objects, facts, analyses, request context, complete task theory, and queries |
| task theory | Every task-relevant rule, condition, exception claim, block claim, priority claim, and optionality claim before condition-specific compilation |
| target organization profile | Deterministic, hashed policy that maps the neutral theory into the PDSGRO organization |
| compiled instance | Condition-specific representation produced from the neutral source bundle |
| model payload | Pre-solution structure lawfully visible to a later model; never an answer, proof, or evaluator record |
| execution audit | Evaluator/compiler-only result of running the reference interpreter, including consequences and proof traces |
| request context | Observable runtime context and one compiled scope anchor; never hand-selected relevant fact or rule IDs |
| governing scope | Declared context in which a fact or control object may apply |
| inherited context | Properties transmitted over explicit permitted inheritance paths |
| exception | A grounded control that defeats one named grounded default application |
| block | A grounded control that prevents one property from traversing specified inheritance paths |
| conflict | Opposite-polarity ground literals supported in one retained branch without lawful resolution |
| ambiguity | Retained branches have different query states under the frozen aggregation policy |
| optionality | A frozen choice constraint that creates multiple legal pre-execution branches |

---

# 4. DQ1 Completion Boundary

Document 06 requires all of the following before DQ1 can close:

1. a formal mechanism specification;
2. an executable toy implementation;
3. a worked input-output example containing ambiguity and exceptions;
4. a component-by-component prior-art and non-duplication matrix;
5. information-equivalent universal and generic formulations;
6. a claim-to-implemented-layer traceability table.

M0 and M1 provide only part of this evidence:

| Required evidence | Primary work package | Closure status after M1 |
|---|---|---|
| Formal mechanism specification | M0 | Can be complete |
| Executable toy implementation | M1 | Can be complete |
| Ambiguity-and-exception worked example | M0 specification; M1 execution | Can be complete |
| Prior-art and non-duplication matrix | M0 kill screen, then full M2 matrix | Still open |
| Universal and generic equivalents | M2 formal formulations; DQ3 implementation | Still open |
| Claim-to-implemented-layer traceability | Started in M0; audited in M2 | Still open |

Accordingly:

> **M1 Pass means “the candidate is executable.” It does not mean “DQ1 Pass.”**

---

# 5. The Candidate to Be Frozen

## 5.1 Working name

**Pāṇinian-Derived Scope-Gated Rule Organizer, version 0.1**

Abbreviation: **PDSGRO-0.1**

The abbreviation is an engineering identifier, not a novelty or historical-authenticity claim.

## 5.2 Exact executability claim

> A finite, typed representation of governing scope, inherited context, defaults, protected exceptions, property-specific blocking, explicit precedence, and optional alternatives can be specified completely enough to produce deterministic output that explicitly represents every retained alternative, a complete audit for completed instances, a deterministic trace prefix for exhausted instances, and bounded resource accounting.

M0 specifies this claim. M1 attempts to demonstrate it.

## 5.3 Engineering mediation hypothesis

> Given identical canonical task facts and event-role relations, scope-gated rule organization may reduce irrelevant rule activation, invalid candidate propagation, active structural context, or avoidable branching while preserving every valid conclusion and protected exception.

This is a hypothesis for later graph-only and model experiments. M0 and M1 may measure diagnostic counters, but they cannot validate an LLM-efficiency claim.

## 5.4 Sanskrit/Pāṇinian attribution estimands

The programme estimates two different contrasts:

1. **Semantic-equivalence estimand:** fix the neutral source bundle and permitted consequence set while allowing representation size and execution cost to differ.
2. **Resource-equivalence estimand:** fix declared bits, compute, parameters, latency, and tuning budget while reporting any loss of semantic coverage or fidelity.

No contrast may be described as satisfying both estimands unless both audits independently pass.

> Under the semantic-equivalence estimand, the frozen Pāṇinian-derived organization may produce an incremental advantage over the strongest competent information-equivalent universal or generic organization. Under the resource-equivalence estimand, it may produce an advantage over the strongest budget-matched control while every semantic coverage or fidelity loss is reported.

This hypothesis belongs to later controlled comparisons. M1 does not test it.

## 5.5 Null hypotheses

The programme must retain all three nulls:

1. **Executability null:** the proposed semantics cannot be made deterministic while explicitly preserving every admissible branch, terminating, and reproducible without manual judgment.
2. **Engineering null:** explicit scope, exception, blocking, precedence, and optionality do not improve any relevant cost-correctness mediator over competent simpler alternatives.
3. **Attribution null:** competent universal or generic organization fully explains any observed benefit.

---

# 6. Target Organization Profile and Treatment Locus

## 6.1 Required non-terminological signature

M0 must freeze:

- a deterministic target compiler, **Compile_T**;
- a machine-readable **TreatmentSignature**;
- every mapping table and configuration used by Compile_T;
- hashes for the compiler specification, mappings, and configuration.

The TreatmentSignature must state the complete target-only constraints on:

- scope construction;
- scope nesting and factorization;
- rule grouping and indexing;
- inheritance-path organization;
- exception-to-default organization;
- block placement;
- priority representation;
- optional-choice representation;
- the predicted mediator changed by each constraint.

Every target structure must be derivable from the neutral source bundle without item-level discretionary judgment.

If the TreatmentSignature:

- is empty;
- cannot be stated without Sanskrit terminology;
- is representationally and organizationally isomorphic to the strongest identified prior generic compiler, leaving no residual target-only factorization, topology, indexing, or mediation constraint after prior-art subtraction; or
- adds no testable constraint beyond a generic compiler,

the candidate is relabelled **Generic Sanskrit-inspired scope machinery** before M1. Engineering may continue under that downgraded attribution.

Semantic equivalence with competent controls is required for fairness and is not a Generic relabelling criterion. The residual hypothesis, if any, concerns organization under matched denotation—not permission to derive different logical answers.

Package effects and primitive effects are different estimands. A later package-level result may not be attributed to scope, inheritance, exception, blocking, precedence, optionality, or any interaction unless that primitive or interaction has its own preregistered contrast.

## 6.2 What is being varied

The candidate treatment is:

> **the organization and compilation of task-relevant rules into governing scopes, inherited contexts, default-exception relations, blocking boundaries, precedence relations, and optional-choice groups.**

## 6.3 What is held constant

For a matched comparison, the following are shared:

- canonical entities, events, concepts, facts, and explicit negative facts;
- candidate analyses and predicate-participant/event-role relations;
- task request and target query;
- the complete representation-neutral task theory and permitted logical operations;
- evaluator-only expected consequences;
- execution interface;
- model backbone and native tokenizer in later frozen-model work;
- capacity and resource ceilings defined by DQ2.

The event/fact graph is the **carrier** for M0 and M1. It is not itself the singular rule-organization treatment.

Separate experiments may later test morphology, derivation, compounds, kāraka/event roles, or other layers. Their effects may not be silently bundled into the M0/M1 result.

## 6.4 Generic execution machinery

The following are initially classified as generic engineering:

- typed graph storage;
- schema validation;
- finite rule evaluation;
- graph traversal and indexing;
- canonical serialization;
- branch enumeration;
- trace production;
- resource counters;
- test harnesses;
- any later graph encoder, adapter, or fusion layer.

A competent generic engine given semantically identical compiled rules should return the same logical answers as the target engine.

Therefore:

> If target and generic implementations return different logical answers under genuinely identical information and semantics, the first presumption is an implementation defect or failed information equivalence—not Sanskrit superiority.

Potential advantages must arise later from organization, factorization, learnability, noise tolerance, active-context size, or bounded-computation behaviour, not from secretly granting the target a more capable executor.

---

## 6.5 Attribution Ledger

Every retained component must receive one initial attribution label.

| Component | Initial attribution | Permitted M0/M1 description |
|---|---|---|
| Predicate-participant/event-role carrier | Pāṇinian-informed linguistic representation, held constant here | Shared canonical carrier |
| Governing scope | Adhikāra-inspired engineering hypothesis | Pāṇinian-derived candidate mapping |
| Inherited context | Anuvṛtti-inspired engineering hypothesis | Pāṇinian-derived candidate mapping |
| Default and protected exception | Utsarga–apavāda-inspired engineering hypothesis | Pāṇinian-derived candidate mapping |
| Explicit precedence | Pāṇinian-informed and broadly procedural | Candidate organization, not unique primitive |
| Optional alternatives | Pāṇinian-informed and broadly procedural | Candidate organization, not unique primitive |
| Property-specific blocking | Pāṇinian/Sanskrit-informed and generic non-monotonic control | Candidate organization, not unique primitive |
| Finite rule interpreter | Generic symbolic AI | Generic executor |
| Typed graph and serialization | Generic engineering | Generic infrastructure |
| Trace and telemetry | Generic engineering | Generic infrastructure |
| Tokenizer | Absent from M0/M1 | Separate DQ4 path |
| Graph encoder or adapter | Absent from M0/M1 | Later ordinary neural engineering |
| Writable memory and rollback | Excluded | Later DQ12 only |

This ledger is deliberately conservative. The Pāṇinian mappings are research hypotheses, not claims that the implementation literally reproduces the Aṣṭādhyāyī or that these computational primitives originated uniquely in Sanskrit.

---

# 7. Frozen System Boundary

## 7.1 Included

M0 and M1 include:

- a language-independent canonical symbolic instance;
- finite typed entities, concepts, events, and values;
- positive and explicit negative ground facts;
- candidate analyses and event-role bindings;
- a finite acyclic scope graph;
- inherited context;
- strict rules;
- defeasible defaults;
- protected exceptions targeting named grounded default applications;
- property-specific inheritance blocks;
- explicit, acyclic precedence;
- bounded optional-choice groups;
- ambiguity and unresolved-conflict preservation;
- deterministic validation and execution;
- canonical output ordering;
- complete derivation and suppression traces;
- read-only active-context construction;
- representation, execution, and development telemetry.

## 7.2 Excluded

M0 and M1 exclude:

- raw-text tokenization claims;
- custom tokenizers;
- Sanskrit surface-language advantage;
- full normalization, Sandhi, morphology, derivation, or compound parsing;
- full sentence, discourse, Vedic, Chandas, kāvya, manuscript, recitation, or prosodic systems;
- learned parsing or automatic structure prediction;
- external retrieval or tools that supply answers;
- neural encoders, embeddings, adapters, attention, or LLM calls;
- model training or weight changes;
- persistent memory writes;
- update transactions, expiry, rollback, or consolidation;
- fast weights, durable model editing, dynamic routing, or self-assimilation;
- claims of reduced real model tokens, model compute, training cost, or deployment cost;
- claims of improved model accuracy or reasoning;
- claims of algorithmic novelty or Sanskrit-specific superiority.

## 7.3 Meaning of scope

In M0 and M1, **scope** means:

> the declared context in which a fact, inheritance relation, rule, exception, block, priority, or optional alternative is applicable during one read-only execution.

It does not mean a persistent knowledge-update scope. M1 starts from an immutable instance and produces no durable state change.

## 7.4 Excluded legacy mappings

The following legacy ideas are not part of PDSGRO-0.1:

- writable-memory dependency and rollback links;
- it-marker-like hidden control semantics as a claimed Sanskrit contribution;
- asiddha-like temporary-state isolation as a claimed Sanskrit contribution;
- propagation into durable model memory.

Generic rule stratification may be used to ensure finite evaluation. It must not be relabelled as evidence for an asiddha-specific contribution.

## 7.5 Claim boundary relative to the pilot

PDSGRO-0.1 licenses only a **rule-organization and scope** claim. It is not the pilot's four-layer S2 Sanskrit Structural Stack and cannot support claims about:

- tokenizer efficiency;
- morphology or derivation;
- compound analysis;
- event-role superiority;
- cross-layer organization; or
- a benefit caused by interaction among those layers.

Any broader candidate requires a new, versioned DQ1 mechanism extension with at least two named implemented layers connected by a frozen mechanism, plus preregistered layer-main-effect and interaction contrasts. Until then, the pilot's cross-layer language is outside the M0/M1 evidence boundary and must not be used to interpret an M1 result.

---

# 8. Canonical Objects

## 8.1 Canonical source bundle

The language-independent source bundle is:

\[
B=(\Sigma,V,F_N,A_N,K_N,T,Q)
\]

where:

- \(\Sigma\) is a finite typed signature containing the permitted predicates, constants, value types, relation types, and total non-generative comparisons;
- \(V\) is a finite set of typed constants and objects;
- \(F_N\) is a finite set of positive or explicit negative ground facts tagged only with representation-neutral `ContextKey` values;
- \(A_N\) is a finite set of representation-neutral analysis-assignment groups; one complete branch selects exactly one compatible member from every mutually exclusive group;
- \(K_N\) is observable request context, including exactly one semantic `AnchorIntent`, domain, time, register, or fictional-world context where relevant;
- \(T\) is the complete representation-neutral task theory;
- \(Q\) is one or more queries.

`ContextKey` and `AnchorIntent` identify semantic applicability without naming a target, universal, or generic scope. The reserved `GLOBAL` context contains only facts lawfully visible before scope activation.

The task theory \(T\) contains every permitted:

- strict rule and defeasible default;
- applicability condition;
- hard constraint;
- exception claim;
- inheritance permission;
- property-specific block claim;
- priority claim;
- optional-choice claim.

The source bundle contains no gold answer, evaluator label, hidden proof, or test-derived consequence.

If any task-relevant rule, condition, relation, literal, or consequence appears after compilation but was absent from \(B\), the compiled condition contains extra information and cannot support a causal attribution claim.

## 8.2 Compiled mechanism instance

For mechanism or control \(m\), the compiler produces:

\[
I_m=Compile_m(B)=(\Sigma,V,F_m,A_m,K_m,S_m,H_m,R_m,E_m,X_m,P_m,O_m,Z_m,Q)
\]

where:

- \(F_m,A_m,K_m\) are condition-specific facts, analyses, and request records in which neutral context keys and the single anchor intent have been mapped to condition-local scope identifiers;
- \(S_m\) is a finite rooted scope forest in which each non-root scope has exactly one parent;
- \(H_m\) is a finite directed acyclic inheritance graph;
- \(R_m\) is a finite set of range-restricted rules;
- \(E_m\) is a finite set of grounded-exception specifications;
- \(X_m\) is a finite set of property-specific block specifications;
- \(P_m\) is an acyclic conditional precedence relation over matched grounded applications;
- \(O_m\) is a finite set of non-overlapping bounded optional-choice groups;
- \(Z_m\) is a finite set of hard constraints.

Every compiled fact, event, role edge, analysis, request mapping, scope, inheritance edge, rule, exception, block, priority, optional group, and constraint carries one or more `source_refs` into \(B\), including the relevant statement in \(T\) where applicable.

Every \(Compile_m\) must be:

- total over its declared input domain;
- deterministic;
- gold-blind;
- versioned and hashed;
- semantics-preserving over the declared consequence language.

A compiler may normalize, factor, index, rename, or reorder source theory. It may not author, infer, retrieve, delete, or add a task predicate, literal, condition, relation, or consequence.

Compilation of structure is query- and runtime-context-independent. Replacing \(Q\) or \(K_N\) while holding \(\Sigma,V,F_N,A_N,T\) fixed must leave every compiled structural field unchanged except copied request-context, mapped anchor, and query fields. Runtime context may activate an already compiled scope during interpretation; it may not create, delete, rank, or reorder facts, rules, analyses, or control objects.

Any query-conditioned selector is a separately named, hashed, intervened-on, and fully costed component. It receives equivalent query access and a matched implementation in every control. It cannot be hidden inside `Compile_T`.

M0 defines the declared consequence language, reference denotation, target decoder `Decode_T`, and exact target obligation:

\[
Decode_T(Compile_T(B)) \equiv B
\]

This includes the explicit context-mapping obligation:

\[
Decode_T(F_T,A_T,K_T) \equiv (F_N,A_N,K_N)
\]

The obligations must pass exact public and frozen generated target cases over the declared M0 domain before M0 freezes. These are formal conformance cases, not the hidden M1 acceptance set.

M2 supplies `Decode_U`, `Decode_G`, and corresponding exact formal witnesses for universal and generic formulations. Quantitative empirical competence thresholds remain for DQ2 and DQ3, but formal round-trip over each formulation's declared domain is exact.

Any manually authored target-only structure is condition input, not compiler output. It must be exposed in the information ledger, supplied equivalently where the estimand requires it, and fully costed.

M1 prohibits:

- function symbols;
- rule-generated object identifiers;
- arbitrary executable code inside rules;
- unbounded recursion;
- negation as failure;
- disjunctive or existential heads;
- arithmetic or value generation;
- implicit negation from missing information;
- hidden tie-breaking by rule identifier or file order.

These restrictions make termination and auditability testable.

---

# 9. Minimum Machine-Readable Schema

The normative schema will be produced as a separate artifact before M0 can become Frozen. It must support at least the following objects.

| Object | Required fields |
|---|---|
| CompilerManifest | compiler_id, version, source_schema_hash, target_schema_hash, mapping_hashes, configuration_hash, implementation_hash |
| TreatmentSignature | version, scope_policy, factorization_policy, topology_constraints, indexing_policy, inheritance_policy, exception_policy, predicted_mediators |
| Signature | version, predicates, constants, types, relation_types, permitted_comparisons |
| ContextKey | id, representation_neutral_definition, provenance_ref |
| AnchorIntent | id, observable_semantic_context, context_key_refs, provenance_ref |
| Entity | id, entity_type, attributes, provenance_ref |
| Concept | id, concept_type, language_independent_definition_ref |
| NeutralEvent | id, predicate_concept_id, participant_edges, context_key, provenance_ref |
| NeutralRoleEdge | id, event_id, entity_or_event_id, role_type, context_key, provenance_ref |
| NeutralAnalysisGroup | id, selection_cardinality_equals_one, member_analysis_ids |
| NeutralAnalysis | id, group_id, bindings, compatibility_constraints, context_key_refs, provenance_ref |
| NeutralFact | id, predicate, arguments, polarity, context_key, provenance_ref |
| NeutralRequest | id, request_context, anchor_intent_id, query_ids, resource_config_id |
| CompiledEvent | id, predicate_concept_id, participant_edges, scope_id, source_refs, provenance_ref |
| CompiledRoleEdge | id, event_id, entity_or_event_id, role_type, scope_id, source_refs, provenance_ref |
| CompiledAnalysisGroup | id, selection_cardinality_equals_one, member_analysis_ids, source_refs |
| CompiledAnalysis | id, group_id, bindings, compatibility_constraints, scope_id, source_refs, provenance_ref |
| CompiledFact | id, predicate, arguments, polarity, scope_id, source_refs, provenance_ref |
| CompiledRequest | id, request_context, scope_anchor, query_ids, resource_config_id, source_refs |
| Scope | id, parent_id_or_null, activation_condition, source_refs, provenance_ref |
| InheritanceEdge | id, source_scope_or_object, target_scope_or_object, permitted_properties, condition, scope_id, provenance_ref |
| Rule | id, kind, body, head, scope_id, stratum, source_refs, provenance_ref |
| Exception | id, condition, target_rule_id, target_substitution_pattern, scope_id, evaluation_stratum, source_refs |
| Block | id, property_or_relation, target_edge_ids_or_path_pattern, condition, evaluation_stratum, source_refs |
| PriorityEdge | id, higher_rule_id, lower_rule_id, higher_substitution_pattern, lower_substitution_pattern, shared_argument_alignment, condition, scope_id, evaluation_stratum, source_refs |
| OptionalGroup | id, member_rule_ids, minimum_choices, maximum_choices, source_refs, provenance_ref |
| Constraint | id, condition, scope_id, evaluation_stratum, source_refs |
| Query | id, proposition, aggregation_policy_id=`skeptical-v1` |
| ResourceConfig | id, logical_step_limit, grounded_application_limit, inheritance_path_limit, branch_limit, trace_limit |
| TraceEvent | step, branch, operation, inputs, rule_or_control, result, suppression_reason |

## 9.1 Rule kinds

The only M1 rule kinds are:

- strict;
- default.

Exception, Block, PriorityEdge, OptionalGroup, and Constraint are separate control objects. Optionality enables or disables named rule IDs before inference; it is not a rule kind.

## 9.2 Literal and condition grammar

A literal is:

- a predicate from \(\Sigma\);
- applied to typed constants or universally quantified variables;
- with explicit positive or negative polarity.

A rule or condition body is a finite conjunction of literals plus a frozen list of total, non-generative comparisons from \(\Sigma\).

Variables:

- are universally quantified;
- range only over constants already present in \(V\);
- must be type-correct;
- wherever they occur in a rule or control condition, must also occur in a positive relational body literal or an explicit finite typed-domain binder;
- must occur in a positive body literal if they occur in a rule head.

Every rule has exactly one literal head.

One grounded application is created for each satisfying total substitution over all variables in the rule or control. Partial substitutions are invalid.

M1 permits no:

- negation as failure;
- disjunction;
- existential head;
- arbitrary callback;
- object generation;
- unbounded arithmetic;
- comparison whose value depends on external state.

Analysis-compatibility and scope-activation conditions use this grammar but may reference only request context, neutral or compiled facts sourced from `ContextKey=GLOBAL`, and the branch's analysis bindings. Inheritance, exception, block, priority, and constraint conditions use the same grammar and name the strictly lower-stratum snapshot on which they are evaluated.

## 9.3 Truth and absence

- Facts have explicit positive or negative polarity.
- Absence of a fact means unknown, not false.
- A body literal is satisfied if and only if that exact-polarity ground literal has support in the named snapshot.
- Support for the opposite polarity does not cancel it: `BOTH` satisfies both the positive and explicit-negative occurrences.
- A conjunction is satisfied if and only if every literal and total comparison in it is satisfied.
- Conflict is paraconsistent: support for both polarities does not entail an unrelated literal.
- Explicitly contradictory source facts make the affected branch conflicted.
- A default is never treated as a strict fact.
- Source, materialized-inheritance, and strict conclusions are indefeasible.
- Opposite source, materialized-inheritance, or strict literals produce CONFLICT.
- Defaults never defeat source, materialized-inheritance, or strict conclusions.
- Exceptions and priorities operate only on grounded default applications.
- An exception targets \((rule\_id, substitution)\), not every grounding of a schematic rule.
- Equal or incomparable opposite defaults produce CONFLICT.

Every query is one type-correct ground literal. Its exact complement has the same predicate and arguments with polarity inverted.

## 9.4 Optional-group restrictions

Optional groups may not overlap in M1. Every member belongs to at most one group.

Optional choices are enumerated before inference. An inapplicable selected member remains selected but produces no grounded application. Its selection and inapplicability remain visible in the execution audit.

## 9.5 Visibility classification

Every field must be classified as exactly one of:

| Class | Who may access it |
|---|---|
| model-visible | Future model condition and its lawful runtime |
| compiler-visible | Compiler or validator, but not a future model payload unless separately declared |
| evaluator-only | Scoring and adjudication only |
| provenance-only | Audit and lineage only |

Gold answers, proof steps, evaluator labels, expected consequences, and hidden-fixture properties are evaluator-only.

No single record may mix model-visible fields with evaluator-only gold fields in a payload supplied to the compiler or interpreter.

---

# 10. Operational Semantics

The separate semantics artifact must refine, but may not contradict, the rules below. An implementer may optimize evaluation only when the canonical semantic and deterministic-audit projections remain identical.

## 10.1 Validation and static stratification

Before branch construction, the validator rejects:

- duplicate identifiers, unknown references, invalid types or arities, and unbound variables;
- a non-finite signature or any operation capable of creating a new object;
- scope or inheritance cycles, a scope with more than one parent, or a compiled anchor outside the rooted scope forest;
- overlapping optional groups or impossible choice bounds;
- a cycle in the unconditional priority supergraph, or a priority pattern that is not type-safe and capable of matching exact-complement default heads under its declared argument alignment;
- an analysis-compatibility or scope-activation condition that reads a non-`GLOBAL` fact;
- evaluator-only data in a compiler, model, or interpreter input;
- a compiled object without valid `source_refs` into the neutral task theory;
- a dependency graph that cannot satisfy the stratification rule below.

The validator constructs a signed predicate-dependency graph. Positive strict dependencies may point to the same or a lower stratum only inside a strict-only region. If predicate \(p\) is default-derivable at stratum \(s\), every strict rule consuming \(p\) must have its head in a stratum strictly higher than \(s\); no same-stratum strict dependency path may begin at a default-head predicate. Every default body, inheritance-control condition, exception condition, block condition, priority condition, and hard-constraint dependency must be settled strictly below the head, propagated property, targeted application, or constraint-evaluation stratum. Any cycle containing a defeasible or control dependency is invalid. The formal schema must state the graph-construction algorithm and the stratum of every predicate and control.

Invalid input yields `execution_status=INVALID_INSTANCE`. The interpreter must not guess a repair.

## 10.2 Complete branch construction

Before inference, construct the exact Cartesian product of:

- one member from every complete, mutually exclusive `CompiledAnalysisGroup`; and
- every legal selection from each non-overlapping `OptionalGroup`.

Reject only combinations that violate an explicit compatibility condition present in the neutral source bundle. Preserve the rejected combination and reason in the execution audit. No analysis may be selected, merged, or discarded because it produces a convenient query answer.

If exact construction would exceed the frozen deterministic branch limit, return `execution_status=RESOURCE_EXHAUSTED`; do not sample, rank, or silently prune branches.

## 10.3 Branch-local scope activation

M1 accepts exactly one compiled `scope_anchor` per Request. A request requiring a different anchor is a separate Request. Because `S_m` is a rooted forest with at most one parent per non-root scope, the anchor has at most one root-to-anchor path.

Evaluate that path from root to anchor. A scope is active only when:

- its parent is active, or it is a root; and
- its activation condition is true using only compiled request context, that branch's analysis bindings, and compiled facts whose neutral source `ContextKey` is `GLOBAL`.

A scoped fact may not help activate the scope that makes the fact visible. Naming an anchor never bypasses its own or an ancestor's condition. The anchor is usable only if the complete unique root-to-anchor path is active; otherwise reject the branch with reason `INACTIVE_ANCHOR`.

A control object at scope \(s\) may consume only `GLOBAL` facts plus facts at \(s\) or its active ancestors on the unique path. Ancestor controls may not consume descendant facts, and off-path sibling scopes never exchange facts implicitly. Every activation decision is recorded.

## 10.4 Inheritance-path semantics

For each branch, subcontext, property, and target, enumerate every active inheritance path allowed by `InheritanceEdge.permitted_properties`.

- A property reaches a target if and only if at least one permitted path is unblocked.
- A block removes only the matching property on the matching edge or path described by its grounded specification.
- A second unblocked path continues to transmit the property.
- Every supporting and blocked path remains in the execution audit.
- Opposite-polarity properties, or unequal values for a declared singleton-valued property, produce an explicit conflict.

Once all applicable blocks are evaluated, an inherited property supported by an unblocked path is committed as indefeasible branch support at its declared stratum. It can be prevented only by a matching block before materialization; defaults and priorities cannot defeat it.

There is no implicit child override, parent-order priority, shortest-path preference, or file-order preference.

## 10.5 Stratified branch evaluation

Evaluate each retained branch independently, in ascending stratum order. In every stratum:

1. evaluate all grounded inheritance permissions and property blocks whose conditions use the settled lower-stratum snapshot;
2. enumerate permitted paths and materialize only conclusions supported by at least one unblocked path;
3. compute the least positive closure of applicable strict rules, allowing only positive same-stratum recursion;
4. instantiate defaults whose bodies are true in the settled lower-stratum snapshot;
5. evaluate every grounded exception from that same frozen snapshot and mark each exactly matched `(rule_id, substitution)` default application defeated;
6. suppress a default opposed by a source fact, materialized-inheritance conclusion, or strict conclusion;
7. after exception and indefeasible-support filtering, instantiate applicable grounded priority edges among the remaining default applications;
8. compute the transitive closure as an ordering relation; defeat a lower grounded application only when that closure pair's endpoints have exact-complement heads—same-polarity closure pairs may order applications but never defeat them;
9. if undefeated opposite defaults remain equal or incomparable, record both and mark the ground literal conflicted;
10. commit every other undefeated default head;
11. evaluate hard constraints at their declared evaluation stratum and reject every matching branch.

A blocked inheritance conclusion is recorded as a counterfactual path in `ExecutionAudit`; it is never committed or consumed by a rule. A strict consequence of a newly committed default can fire only in a later stratum, before that later stratum's defaults are resolved. A committed lower-stratum conclusion is never retracted. Exceptions and priorities may defeat only grounded default applications identified as `(rule_id, substitution)`; they never defeat source facts or strict rules. A property block affects inheritance, not rule defeat. Narrower scope, later file position, confidence, identifier order, and traversal order are never implicit priorities.

A `PriorityEdge` is instantiated only after exception and indefeasible-support filtering and only between two remaining applicable grounded default applications whose heads are exact polarity complements and whose substitutions match the frozen higher/lower patterns and shared-argument alignment. Compatible heads, unmatched substitutions, and different ground entities are never defeated by that edge.

Every applicable exception and indefeasible-opposition ground is recorded even when another such ground already defeats the application. Priority grounds are recorded only for applications that remain after those filters. Grounds are canonically sorted by control class and identifier; no incidental evaluation order changes the audit.

## 10.6 Conflict semantics

A conflict is support for opposite-polarity ground literals in one retained branch. Source facts, materialized-inheritance conclusions, and strict conclusions are indefeasible. Opposite indefeasible conclusions therefore remain visible as conflict. Defaults cannot defeat them. Undefeated opposite defaults also remain conflict unless the frozen priority relation orders the corresponding grounded applications.

Conflict is query-specific at aggregation time: a branch has query state `BOTH` only when it supports both the query literal and its explicit opposite. Unrelated conflicts remain reported but do not silently alter another query's state.

## 10.7 Deterministic resource exhaustion

Semantic completion is governed only by frozen deterministic counters: grounded applications considered, inheritance paths enumerated, branches constructed, trace events emitted, and logical steps executed. Their counting rules and limits are part of `ResourceConfig`.

Wall time, CPU time, peak memory, hardware, and operating-system behaviour are telemetry; they must not change semantic status. On a deterministic limit breach, return `execution_status=RESOURCE_EXHAUSTED`, the exact counter and limit, and the canonical deterministic trace prefix. No partial query answer is reported as complete.

## 10.8 Query aggregation: `skeptical-v1`

M1 supports one aggregation policy, `skeptical-v1`. Item authors may not select a different policy.

For every retained branch and proposition \(q\), define:

- `TRUE` when the branch supports \(q\) but not explicit \(\neg q\);
- `FALSE` when it supports explicit \(\neg q\) but not \(q\);
- `NEITHER` when it supports neither;
- `BOTH` when it supports both.

When `execution_status=COMPLETE`, aggregate in this exclusive order:

1. no retained branch → `NO_VALID_ANALYSIS`;
2. any retained branch is `BOTH` → `CONFLICT`;
3. every retained branch is `TRUE` → `ENTAILED`;
4. every retained branch is `FALSE` → `CONTRADICTED`;
5. every retained branch is `NEITHER` → `UNKNOWN`;
6. every other mixture → `AMBIGUOUS`.

`analysis_status` is separately `NONE`, `SINGLE`, or `MULTIPLE`. Several retained analyses with the same query state do not by themselves make the query ambiguous.

## 10.9 Output separation

Compilation produces a pre-solution `ModelPayload`. Interpretation produces an evaluator-facing `ExecutionAudit`. Runtime measurements produce a separate `TelemetryManifest`.

- `ModelPayload` contains only lawful pre-inference source or compiled structures.
- `ExecutionAudit` contains query results, branch dispositions, derived consequences, firing and defeat outcomes, conflicts, proofs, and the deterministic trace.
- A complete run emits a complete deterministic audit. A resource-exhausted run emits only its deterministic prefix and exhaustion reason.
- `TelemetryManifest` contains non-semantic runtime and environment measurements.

The three artifacts have separate schemas and hashes. Section 15 fixes their visibility boundary.

---

# 11. Semantic Invariants

M0 is not complete until every invariant below maps to an automated M1 test.

1. **Concept independence:** canonical concepts do not depend on Sanskrit labels.
2. **Open-world discipline:** absence is not negation.
3. **Scope safety:** no rule or fact escapes its declared active scope.
4. **Property-local blocking:** a block suppresses only the declared property or relation.
5. **Exception locality:** an exception defeats only its named grounded default application.
6. **Explicit precedence:** no semantic tie is resolved by incidental execution order.
7. **Ambiguity preservation:** multiple valid analyses remain visible.
8. **Optionality preservation:** optional alternatives remain live unless an explicit constraint removes them.
9. **Conflict visibility:** unresolved mandatory conflicts remain visible.
10. **Trace completeness:** every derived, blocked, defeated, or rejected item has a machine-readable reason.
11. **Path completeness:** all permitted inheritance paths are considered, and blocking one path never blocks another implicitly.
12. **Grounding locality:** exception or priority against one grounding never defeats another grounding implicitly.
13. **Stratified stability:** a lower-stratum committed conclusion is never retracted by a higher stratum.
14. **Order invariance:** permutation of semantically unordered records does not change the semantic projection.
15. **Non-semantic renaming invariance:** after applying the inverse identifier bijection, changing labels or identifiers with no declared semantics does not change the semantic projection.
16. **Irrelevance locality:** adding an inactive or disconnected fact or rule does not change the affected semantic projection.
17. **Termination:** every valid M1 instance terminates or returns `RESOURCE_EXHAUSTED` under deterministic logical limits.
18. **No evaluator leakage:** evaluator-only data never enters compiler, interpreter, or model inputs.
19. **Payload separation:** no derived query consequence, branch verdict, firing result, proof, or oracle field enters `ModelPayload`.
20. **Read-only execution:** an M1 run changes no persistent model or knowledge state; ordinary output artifacts are allowed.
21. **No derivational truth leap:** derivational or etymological plausibility is never treated as empirical truth.
22. **Control expressibility:** the representation-neutral interface does not prevent a generic control from representing the same task-relevant information and operations.

---

# 12. Complete Dataflow and Later Boundary

## 12.1 M0/M1 dataflow

~~~text
Language-independent canonical source bundle
        ↓
Condition compiler: target, universal, or generic
        ↓
Validated pre-solution compiled instance
        ├──────────────→ ModelPayload
        │                 lawful pre-inference structure only
        ↓
Deterministic reference interpreter
        ├──────────────→ ExecutionAudit
        │                 consequences, decisions, proofs, deterministic trace
        └──────────────→ TelemetryManifest
                          runtime and environment measurements
~~~

`ModelPayload`, `ExecutionAudit`, evaluator oracle, and telemetry are physically separate artifacts. Only `ModelPayload` is eligible for later model input.

## 12.2 Future experimental dataflow

M0 freezes the interface boundary for later work:

~~~text
ModelPayload
        ↓
DQ5 graph-only task and corruption diagnostics
        ↓
fixed structural serialization or encoder input
        ↓
capacity-matched adapter on an identical frozen backbone
        ↓
verified task output
        ↓
DQ6 causal intervention and DQ7 specificity contrasts
~~~

The future interface does not authorize its implementation in M1. DQ5 may use `ExecutionAudit` only as evaluator-side diagnostic evidence; it may not pass any audit field to the evaluated model.

The frozen-model phase retains the backbone's native tokenizer. Any custom-tokenizer candidate remains a separate DQ4 path and joins only in later integrated training if it independently earns entry.

## 12.3 Full end-to-end boundary required before DQ1 closes

M2 must provide a condition-specific crosswalk for the complete later path:

~~~text
raw input
  → native tokenization
  → parser / annotation or oracle structure source
  → neutral source bundle
  → condition compiler
  → ModelPayload
  → serialization / encoder / adapter / fusion
  → frozen or trained backbone
  → any retrieval or external tool
  → decoder / generated output
  → verifier / evaluator
  → token, compute, latency, storage, and labour meters
~~~

Before DQ1 closes, every transition must have a hashed versioned interface specification, named owner, planned implementation gate, visibility class, attribution class, cost boundary, and planned matched-control counterpart. Any component already implemented must also have an implementation hash. DQ1 freezes the design and traceability obligations; DQ3, DQ5, DQ6, and later gates add the actual implementation hashes before their respective executions. Any later implementation change that alters the frozen treatment boundary, lawful information, or claimed causal path reopens DQ1. The crosswalk must distinguish the DQ4 tokenizer path and the DQ8 oracle-versus-predicted-structure path. M0 and M1 specify only the symbolic segment and cannot close this requirement by themselves.

---

# 13. Causal Traceability Contract

Every claimed primitive must have:

- one schema element;
- one execution transition;
- one positive witness;
- one negative or ablated witness;
- one target-output prediction;
- one non-target invariance prediction;
- one later DQ5 diagnostic;
- one later DQ6 intervention;
- one relevant DQ7 control contrast.

| Primitive | M1 state change | M1 observable | Later intervention prediction | Required non-target invariance |
|---|---|---|---|---|
| Governing scope | Changes active rules and facts | Active-set difference | Moving one rule across a scope boundary changes only in-scope conclusions | Sibling and inactive scopes remain unchanged |
| Inherited context | Materializes permitted properties | Inheritance path and affected set | Removing an inheritance edge removes only dependent conclusions | Independent source facts remain unchanged |
| Protected exception | Defeats a named grounded default application | Defeated application and reason | Removing the exception produces predicted over-propagation | Unrelated defaults remain unchanged |
| Property block | Stops one inherited property | Blocked path | Removing the block propagates exactly the formerly blocked property | Other inherited properties are unchanged |
| Precedence | Selects among conflicting applicable grounded defaults | Winning and defeated grounded default applications and priority path | Reversing priority flips only the targeted conflict | Non-conflicting applications remain unchanged |
| Optionality | Preserves several admissible branches | Live alternatives | Removing optionality collapses the declared alternatives | Mandatory conclusions common to all branches remain unchanged |
| Ambiguity | Retains compatible analyses | Analysis set and query aggregation | Adding one discriminating scope constraint removes only the incompatible analysis | Facts shared by analyses remain unchanged |

If a primitive has no target-specific and non-target prediction, it is not yet a causal mechanism; it is descriptive metadata.

---

# 14. Information and Leakage Contract

## 14.1 Separate records

M1 uses physically separate artifacts:

| Artifact | Permitted content |
|---|---|
| neutral source bundle | condition-independent facts, task theory, analyses, request context, and queries |
| ModelPayload | lawful pre-solution compiled structures eligible for later model input |
| ExecutionAudit | evaluator/compiler-only consequences, branch decisions, proofs, and deterministic trace |
| evaluator oracle | expected status, expected conclusions, forbidden conclusions, expected trace properties |
| TelemetryManifest | runtime, resource, environment, and labour measurements |
| provenance manifest | authors, sources, review, licenses, timestamps, hashes |
| hidden acceptance manifest | encrypted or access-controlled fixture IDs, properties, custodian, unseal event |

## 14.2 Prohibited fields in execution input

Execution input must not contain:

- gold answer;
- correct analysis label;
- gold proof;
- evaluator rationale;
- expected update consequence;
- expected blocked set;
- benchmark split label;
- hidden scoring key;
- any field derived from sealed test outputs.

## 14.3 Compiler limitation

A lawful compiler may normalize or transform declared source information.

If it independently solves the target task, performs query-result selection, or injects test-derived consequences, later performance cannot be attributed to model reasoning. The result may be reported only as a fully costed external-reasoner or tool-system outcome.

## 14.4 Incremental leakage probe and sequence

M2 specifies the information-equivalence witnesses and candidate leakage tests. DQ2 freezes the leakage dataset, estimator, thresholds, custody, and invalidation rule. DQ3 implements the condition compilers and runs the frozen tests before any causal interpretation.

The probe must:

- measure label predictability from the structural side channel alone;
- measure incremental label predictability conditional on the lawful baseline input;
- test field-removal and provenance-based explanations for unexpected predictive power;
- invalidate any fixture whose gold information entered any compiler, payload, cache, training artifact, or selection rule.

A side channel that appears harmless alone may still reveal a key jointly with the baseline input. Passing only a side-channel-only probe is insufficient.

---

# 15. ModelPayload, ExecutionAudit, and Telemetry Boundary

## 15.1 ModelPayload: eligible for later model input

`ModelPayload` is created before reference inference. It may contain only:

| Field family | Permitted content |
|---|---|
| source objects and facts | Lawful deployment-time entities, events, roles, facts, and explicit negatives |
| candidate analyses | Every pre-inference candidate and compatibility condition, without a selected or rejected label |
| unsolved task theory | Strict/default rules, exceptions, blocks, priorities, constraints, and optional groups |
| organization | Scope and inheritance topology produced by the frozen compiler |
| request | Observable request context, one compiled scope anchor, and the unsolved query |
| provenance | Only fields declared model-visible and available symmetrically to controls |

It must exclude:

- query status or gold answer;
- derived query consequences;
- selected, retained, or rejected analysis verdicts;
- fired, defeated, suppressed, or winning-rule outcomes;
- resolved conflicts;
- proof paths or execution traces;
- evaluator, hidden-fixture, or scoring fields.

`Request` never contains hand-selected fact IDs, rule IDs, proof hints, or a computed relevance set. If query-conditioned filtering is later used, every control receives equivalent filtering and its full computation and labour cost is included.

## 15.2 ExecutionAudit: evaluator/compiler only

`ExecutionAudit` may contain:

- execution and query statuses;
- retained and rejected branches with reasons;
- active and derived facts;
- inherited and blocked paths;
- grounded fired, defeated, or suppressed applications;
- optional selections;
- conflicts, proofs, and the deterministic trace;
- deterministic representation counters.

These fields are evaluator-only or compiler-visible as individually declared. No later evaluated model may consume them.

## 15.3 TelemetryManifest: non-semantic measurements

Runtime, CPU, memory, timestamps, environment, hardware, and labour records live in `TelemetryManifest`, not in the canonical semantic output. Every field receives its own visibility class; record-level classification is insufficient.

If a downstream model receives any post-inference `ExecutionAudit` field, that condition is a fully costed external-reasoner/tool system and cannot support an LLM-reasoning attribution.

---

# 16. M0 Golden-Fixture Contract

## 16.1 Required public development fixtures

| Fixture ID | Mechanism isolated | Required behaviour |
|---|---|---|
| DQ1-M0-F01-scope-inactive | Governing scope | Selecting an anchor cannot bypass a false activation condition, and sibling facts do not leak |
| DQ1-M0-F02-inherited-context | Inheritance | A permitted parent property reaches the child |
| DQ1-M0-F03-property-block | Blocking | One path/property stops while an unrelated property and a second unblocked path still propagate |
| DQ1-M0-F04-default-only | Default | An undefeated applicable default produces a defeasible conclusion |
| DQ1-M0-F05-protected-exception | Exception | One grounded exception defeats only its named grounded default application |
| DQ1-M0-F06-precedence-chain | Precedence | The transitive closure of an acyclic priority chain resolves the declared default conflict |
| DQ1-M0-F07-precedence-tie | Conflict | Incomparable opposite defaults yield `CONFLICT` |
| DQ1-M0-F08-optionality | Optionality | Every permitted optional selection becomes a pre-inference branch |
| DQ1-M0-F09-ambiguity | Ambiguity | Different retained query states aggregate as `AMBIGUOUS` |
| DQ1-M0-F10-two-analysis-groups | Branch construction | Two independent groups produce the exact Cartesian product |
| DQ1-M0-F11-no-valid-analysis | Constraint | Rejection of every branch yields `NO_VALID_ANALYSIS` |
| DQ1-M0-F12-conflict-matrix | Truth hierarchy | Opposite source, strict, and default combinations obey the frozen conflict and defeat rules |
| DQ1-M0-F13-derived-constraint | Constraint timing | A constraint activates only at its declared stratum and rejects exactly the matching branch |
| DQ1-M0-F14-malformed-cycles | Validation | Scope, inheritance, priority, and defeasible/control dependency cycles fail closed |
| DQ1-M0-F15-resource-bound | Deterministic exhaustion | The same logical limit produces the same deterministic trace prefix and exhaustion reason |
| DQ1-M0-F16-combined-clean-room | Interaction | Analysis, inheritance, blocking, exception, strict negation, and optionality interact in one trace |

## 16.2 Combined clean-room fixture

The combined fixture uses a fictional library world to prevent pretraining knowledge from determining the expected result.

Required source facts:

- the nonce expression **vel** has two candidate senses: ordinary manual and rare codex;
- the request describes a borrowing event with a doctoral researcher as agent and vel as affected entity; there is no direct registered-member fact for that researcher;
- doctoral researchers inherit registered-member status;
- the rare-codex analysis classifies vel as a library item;
- library items inherit both `catalogued` and `circulating` through declared paths;
- rare codices block only the `circulating` property and continue to inherit `catalogued`;
- registered members may borrow catalogued items by default;
- one exception grounded to the rare codex defeats that borrowing-default application;
- one strict special-collections rule derives explicit `not may_borrow` for rare codices;
- `OptionalGroup {view_on_site, request_scan}` has `minimum_choices=1` and `maximum_choices=1`;
- one explicit compatibility constraint rejects the ordinary-manual sense in special collections;
- the request context activates special collections.

The frozen query is:

~~~text
Q1 = may_borrow(researcher, vel)
aggregation_policy_id = skeptical-v1
~~~

Required output properties:

- the original two-sense ambiguity appears in the trace;
- the explicit compatibility constraint rejects only the ordinary-manual analysis;
- registered-member status is inherited;
- catalogued remains inherited;
- circulating is blocked;
- the general borrowing default is generated and then defeated;
- the strict negative conclusion is retained;
- `Q1` is exactly `CONTRADICTED`;
- exactly two retained optional branches remain, one for view-on-site and one for request-scan;
- no ordinary-manual branch remains;
- no unrelated fact changes;
- every decision has a trace path.

This fixture satisfies the formal ambiguity-and-exception requirement but does not validate the Pāṇinian historical mapping.

## 16.3 Sanskrit/Pāṇinian microfixture

Before M0 can become Frozen, a Sanskrit/Pāṇinian domain reviewer must author or approve at least one compact attested microfixture that:

- exercises one or more claimed mappings;
- contains a real ambiguity or protected exception;
- separates the source analysis from the engineering analogy;
- identifies the grammatical source and interpretive assumptions;
- states competing analyses where scholarly disagreement exists;
- does not insert the expected benchmark answer into the mechanism payload.

This document intentionally does not invent a classical example without domain review.

Every Pāṇinian-labelled attribution-ledger row and every claimed target-only `TreatmentSignature` constraint also requires a separate mapping card containing:

- primary or authoritative source citation and translation;
- interpretive assumptions and competing scholarly analyses;
- the exact computational correspondence and its limits;
- the residual claim after prior-art subtraction; and
- the Sanskrit/Pāṇinian reviewer's Approve, Relabel, or Reject decision.

Unsupported rows are relabelled broadly linguistic or Generic. The attested microfixture is illustrative; it cannot substitute for per-claim mapping approval.

## 16.4 Hidden acceptance fixtures

Before M0 freezes, an independent reviewer must freeze a hidden-fixture generation and custody specification containing:

- the generator and independent denotational oracle specifications;
- supported domain sizes, scope depths, inheritance widths, strata, and branch counts;
- an operator-combination and boundary/adversarial coverage matrix;
- sample count per stratum and the exact acceptance threshold;
- random-seed generation, escrow, and custody;
- the mutation operator set and minimum mutation score;
- disjointness rules for development, M1 acceptance, and DQ5–DQ10 scored items.

Exact semantic conformance is 100%: every valid in-domain case must match the independent oracle and every invalid case must fail closed. Percentage thresholds may govern only non-semantic diagnostic coverage or mutation sampling; they may not waive a semantic mismatch.

After M0 freezes and before M1 acceptance, the custodian generates and seals the hidden fixtures and manifest. The reference oracle or formal model checker must be independently written and may not share production evaluator code.

The implementer may know:

- the schema;
- operator inventory;
- fixture families;
- required invariants;
- resource bounds.

The implementer may not see:

- hidden instance contents;
- gold outputs;
- hidden mutation choices;
- acceptance result details until the declared unseal event.

The first unseal is immutable. Once failure details from a hidden set are disclosed, that set becomes development data. A rerun requires a newly generated, independently sealed set; repeated hidden sets do not become unrecorded lottery tickets, and their result history remains in the decision record.

---

# 17. DQ1-M0 Required Artifacts

M0 cannot become Frozen until all artifacts below exist.

| Artifact | Required content | Current status |
|---|---|---|
| M0 normative contract | This document after review | Draft |
| TreatmentSignature | Non-terminological target-only organization constraints and predicted mediators | Missing |
| target compiler package | `Compile_T`, mapping tables, configuration, manifests, and hashes | Missing |
| canonical source JSON Schema | \(B=(\Sigma,V,F_N,A_N,K_N,T,Q)\) | Missing |
| target representation JSON Schema | \(I_m=(\Sigma,V,F_m,A_m,K_m,S_m,H_m,R_m,E_m,X_m,P_m,O_m,Z_m,Q)\) | Missing |
| operational semantics | Normative transition and aggregation rules | Draft within this document; separate artifact missing |
| target denotation and decoder | Declared consequence language, reference denotation, `Decode_T`, and exact target round-trip witness | Missing |
| ModelPayload schema | Frozen pre-solution later-integration interface | Draft within this document; separate artifact missing |
| ExecutionAudit schema | Status, branches, consequences, conflicts, proofs, deterministic trace | Missing |
| TelemetryManifest schema | Runtime, resources, environment, and labour | Missing |
| attribution ledger | Sanskrit/Pāṇinian, linguistic, generic, neural, excluded | Draft within this document |
| mapping-card set | Source, translation, interpretation, computational correspondence, prior-art residual, and reviewer decision for every retained Pāṇinian-labelled claim | Missing |
| claim traceability table | Claim to field, transition, fixture, intervention, control | Draft within this document |
| public fixture set | DQ1-M0-F01 through DQ1-M0-F16 | Missing |
| evaluator-only oracle set | Expected outputs and trace properties | Missing |
| hidden-fixture generation and custody specification | Generator, independent oracle, coverage, sample sizes, seeds, custodian, unseal rule | Missing |
| cost-counter specification | Representation, execution, labour, environment | Draft within this document |
| representation-neutral compiler interface | Same canonical source, round-trip obligation, no target-only mandatory state | Draft within this document |
| control-development charter | Families, independent builders, competence-test specifications, budgets, access, and veto rights | Missing |
| prior-art kill-screen matrix | Closest systems, matching components, residual computational claim, and relabelling decision | Missing |
| review checklist | Formal, historical, methodological, implementation | Missing |
| version/hash manifest | Hash of every M0 artifact | Missing |

The status column is an audit record. It must not be changed to Complete without the named artifact.

---

# 18. DQ1-M0 Review and Exit Rule

## 18.1 M0 Pass

M0 passes only when:

- one exact treatment locus and causal chain are frozen;
- `Compile_T`, the `TreatmentSignature`, every mapping table, and every configuration are deterministic and hashed;
- the target consequence language, reference denotation, `Decode_T`, and exact target round-trip witness pass over the declared M0 domain;
- every claimed term has a machine-level meaning;
- every schema validates every public golden fixture;
- no unresolved semantic choice remains in prose;
- no behavioural TBD remains;
- an independent engineer can implement M1 without asking the mechanism author to decide semantics;
- an independent reviewer can manually derive every public fixture result;
- independent universal and generic control builders approve a minimal representation-neutral input/output contract;
- the common interface makes no target-specific internal state mandatory for a control;
- the control charter names mandatory comparator families, independent builders, absolute competence-test specifications, symmetric expert/data access, resources sufficient to reach competence, equal post-freeze search budgets, round-trip tests, and baseline-challenge veto rights;
- pre-freeze target engineering is disclosed and cannot be used to justify under-resourcing a baseline;
- a prior-art kill screen covers scoped Datalog/ASP, default and defeasible logic, argumentation, inheritance networks, production-rule systems, grammar formalisms, and graph query engines;
- the closest prior mechanism and any residual computational constraint are recorded;
- all included and excluded layers are explicit;
- every input field has one visibility class;
- no evaluator-only field enters execution input;
- termination, ambiguity, conflict, exception, blocking, precedence, and optionality behaviours are fixed;
- the complete cost boundary is specified;
- the attribution label is no stronger than the implemented mechanism;
- the Sanskrit/Pāṇinian reviewer approves every retained mapping card; unsupported mappings are relabelled or removed;
- the independent methods reviewer approves the causal boundary;
- all required artifacts are hashed;
- all four reviewers approve the same normative hash and meet the independence rules.

M0 freezes the target semantics and the representation-neutral comparison interface. M2 completes the formal universal and generic formulations. DQ2 freezes quantitative competence and leakage rules; DQ3 builds and tests the controls. The target and every control must be frozen before any DQ5 development outcome is inspected.

## 18.2 M0 Repair

M0 remains Draft or Reviewed when:

- the candidate appears coherent but one or more semantic decisions are unresolved;
- required schemas, fixtures, reviews, or hashes are missing;
- the public claim is broader than the implementation boundary;
- the control interface cannot yet express the same operations.

Repair work may continue, but M1 acceptance cannot begin against an unfrozen semantic contract.

## 18.3 M0 Relabel or Stop

Relabel the candidate **Generic Sanskrit-inspired scope machinery** and continue to M1 when:

- it is representationally and organizationally isomorphic to the strongest identified prior generic compiler after prior-art subtraction;
- the residual distinction cannot be stated without Sanskrit terminology; or
- prior art fully explains the proposed computational operators.

The permitted public description is then:

> Generic executable scope machinery inspired and populated by Pāṇinian analysis, with no algorithmic-uniqueness claim.

Stop the rule-scope work package when:

- behaviour depends on undefined authenticity, hidden human judgment, or item-level discretionary compilation;
- the mechanism requires a Version 1 exclusion such as writable memory or full discourse;
- it relies on pretrained Sanskrit label semantics;
- it cannot specify finite execution, conflict, or optionality without hidden heuristics;
- gold answers or test-derived consequences enter the execution or model payload and cannot be removed; or
- information-equivalent controls cannot receive the same task theory and lawful operations.

Genericity is an attribution result, not an engineering failure. Unformalizability, leakage, unmatched information, or hidden judgment are stop conditions.

---

# 19. DQ1-M1 Implementation Contract

## 19.1 Purpose

M1 implements the Frozen M0 semantics as a small, deterministic, non-LLM reference interpreter.

Its only scientific question is:

> Can the proposed candidate be executed reproducibly, without hidden human or model judgment, while preserving scope, exceptions, blocking, optionality, ambiguity, conflict, and a complete audit trace?

## 19.2 Non-normative implementation choice

A small Python reference implementation with JSON inputs and outputs is recommended for auditability.

The programming language is not normative. The M0 schemas, semantics, fixtures, and expected properties are normative.

## 19.3 Required modules

The implementation must separate:

1. source-bundle loader;
2. target compiler;
3. schema and invariant validator;
4. complete analysis/optional branch constructor;
5. branch-local scope activator;
6. inheritance and blocking evaluator;
7. strict/default rule evaluator;
8. exception and precedence resolver;
9. constraint evaluator;
10. `skeptical-v1` query aggregator;
11. `ModelPayload` serializer;
12. deterministic audit and trace emitter;
13. telemetry collector;
14. projection-specific canonical serializer and hasher;
15. test runner.

No module may call an LLM, use learned parameters, or access evaluator-only files during execution.

## 19.4 Required artifacts and projections

The pre-inference artifact contains:

~~~text
ModelPayload
├── schema_version
├── mechanism_version
├── compiler_version
├── source_bundle_hash
├── lawful_source_and_compiled_structures
├── candidate_analyses[]
├── request_context
├── scope_anchor
├── unsolved_queries[]
└── model_payload_hash
~~~

The post-inference deterministic artifact contains:

~~~text
ExecutionAudit
├── schema_version
├── mechanism_version
├── execution_status
├── evaluation_state
├── exhaustion_reason_or_null
├── validation_errors[]
├── query_results[{query_id, query_status, branch_states}]
├── analysis_status
├── branches[]
│   ├── branch_id
│   ├── analysis_assignment
│   ├── optional_selection
│   ├── scope_anchor
│   ├── disposition_and_reason
│   ├── query_states[]
│   ├── active_and_derived_facts[]
│   ├── grounded_applications[{rule, substitution, status, reasons[]}]
│   ├── supporting_and_blocked_paths[]
│   ├── conflicts[]
│   └── trace_refs[]
├── trace[]
└── canonical_output_hash
~~~

Top-level query and analysis fields are deterministic summaries of the branch-local records; they never replace those records.

The result schema is a tagged union:

- `COMPLETE`: `evaluation_state=EVALUATED`, complete branch records, and complete query results;
- `INVALID_INSTANCE`: `evaluation_state=NOT_EVALUATED`, empty query results and branches, one or more validation errors, and only the deterministic validation trace;
- `RESOURCE_EXHAUSTED`: `evaluation_state=NOT_EVALUATED`, empty query results, a deterministic incomplete branch/audit prefix marked `PARTIAL`, and the exact exhausted counter and limit.

Neither failure variant may carry a completed or partial query answer.

Runtime and environment fields are stored separately in `TelemetryManifest` with its own run-manifest hash.

M1 defines three projections:

1. `semantic_projection`: statuses, branch query states, retained semantic consequences, and conflicts;
2. `deterministic_audit_projection`: the semantic projection plus deterministic branch dispositions, paths, grounded applications, reasons, and trace;
3. `telemetry_projection`: runtime, memory, environment, hardware, timestamps, and labour.

All deterministic records are canonically sorted before hashing. The output hash is:

\[
canonical\_output\_hash = SHA256(CanonicalJSON(deterministic\_audit\_projection \setminus canonical\_output\_hash))
\]

The hash field is therefore omitted from the object being hashed. Telemetry never enters this hash.

The other integrity hashes are:

\[
model\_payload\_hash = SHA256(CanonicalJSON(ModelPayload \setminus model\_payload\_hash))
\]

\[
telemetry\_manifest\_hash = SHA256(CanonicalJSON(TelemetryManifest \setminus telemetry\_manifest\_hash))
\]

Each hash field is omitted from its own preimage. The telemetry hash verifies one run manifest; it does not imply that measured values repeat across runs.

Semantic results must not depend on:

- source-file order;
- object order;
- hash-map order;
- incidental traversal order;
- lexicographic identifier order.

Identifiers may stabilize presentation only after semantic resolution. Identical input and configuration must produce byte-identical semantic and deterministic-audit projections and hashes. Telemetry need only be complete, well-formed, and separately hashed; its measured values need not be byte-identical.

---

# 20. M1 Test Contract

## 20.1 Unit and integration tests

M1 must include:

- schema-validation tests;
- malformed-reference tests;
- scope, inheritance, priority, and defeasible/control dependency-cycle rejection;
- one unit test per operator;
- public golden tests for every M0 fixture;
- combined end-to-end trace validation;
- hidden clean-room acceptance fixtures;
- independent small-instance exhaustive-oracle comparison;
- canonical serialization and hash tests;
- resource-exhaustion tests.

The exhaustive-oracle test uses the frozen generator, declared finite domain bounds, escrowed seeds, and an independently implemented denotational oracle. Production interpreter code may not serve as its own oracle.

## 20.2 Metamorphic tests

The following transformations must preserve the semantic projection:

- permutation of node, fact, edge, rule, and scope order;
- replacement of non-semantic Sanskrit relation labels by arbitrary identifiers;
- renaming of object identifiers, after applying the inverse bijection to the result;
- addition of an inactive-scope rule;
- addition of a disconnected irrelevant fact;
- addition of unrelated provenance metadata.

Audit identifiers, provenance records, and telemetry may differ under a lawful rename or metadata addition. Literal byte or hash identity is required only when the canonical deterministic-audit input is identical.

The following compiler metamorphisms must preserve every compiled structural field:

- replace the query while holding \(\Sigma,V,F_N,A_N,K_N,T\) fixed;
- replace runtime context or `AnchorIntent` while holding \(\Sigma,V,F_N,A_N,T,Q\) fixed, except for copied request-context and mapped-anchor fields.

Execution may respond to a different query or activate a different already-compiled scope from changed runtime context; compilation may not create an answer-relevance topology in response.

The following transformations must produce the preregistered target-specific change:

- removing a protected exception;
- removing one property block;
- moving one rule across a governing-scope boundary;
- reversing one precedence edge;
- removing optionality from one declared group;
- adding one discriminating constraint to an ambiguous analysis;
- applying one type-preserving structural corruption.

Every target-specific mutation also declares which non-target outputs must remain invariant.

## 20.3 Mutation adequacy

The test suite must kill mutations that disable or invert:

- scope checks;
- inheritance permissions;
- blocking;
- default defeasibility;
- exception matching;
- precedence;
- optionality;
- ambiguity preservation;
- conflict emission;
- leakage rejection;
- canonical ordering.

If disabling a claimed operator does not fail any test, that operator is not demonstrated by M1 and must be removed from the M1 claim or given a valid witness.

## 20.4 No fixture hard-coding

The interpreter must not:

- branch on fixture identifiers;
- embed gold conclusions;
- identify hidden fixtures by hash;
- special-case nonce labels;
- depend on comments or evaluator metadata.

Static inspection and hidden renamed variants must test this condition.

---

# 21. M1 Telemetry and Cost Ledger

Every run reports:

## 21.1 Representation

- source objects by type;
- compiled objects by type;
- relations by type;
- rules by kind;
- input bytes;
- compressed input bits under a named, versioned frozen compressor, or `NOT_CONFIGURED`;
- compiled representation bytes;
- trace bytes;
- output bytes;
- optional diagnostic tokens under a named, versioned frozen tokenizer, or `NOT_CONFIGURED`.

Diagnostic token counts are not LLM token-efficiency results.

## 21.2 Execution

- candidate analyses before and after constraints;
- active and inactive scopes;
- applicable, fired, defeated, and blocked rules;
- inherited and blocked properties;
- live branches;
- conflicts;
- strict-closure rounds by stratum;
- deterministic logical steps and limit by counter type;
- maximum frontier size;
- validation CPU time;
- compilation CPU time;
- execution CPU time;
- wall time;
- peak resident memory;
- storage;
- resource-limit events.

## 21.3 Environment

- operating-system identity;
- runtime and dependency versions;
- CPU identity;
- available memory;
- configuration hash;
- schema hash;
- mechanism hash;
- fixture hash;
- source revision or archive hash.

## 21.4 Development and expert labour

Report separately by condition, stage, role, and frozen rate-sheet version:

- mechanism-design hours;
- neutral-theory construction, annotation, and adjudication hours;
- `Compile_T`, mapping-table, and `TreatmentSignature` engineering hours;
- universal and generic control-compiler engineering hours;
- interpreter engineering hours;
- fixture-authoring hours;
- hidden generator, independent oracle, custody, and audit hours;
- data licensing, acquisition, normalization, and translation hours and fees;
- Sanskrit/Pāṇinian review hours;
- methods-review hours;
- independent baseline-challenge and reproduction hours;
- recurring maintenance and rebuild hours;
- failed implementation and test runs.

Tag every entry as shared, target-specific, universal-control-specific, or generic-control-specific, and as exploratory, reproducible-build, or recurring-maintenance. Freeze the allocation rule for shared labour before comparisons. Report exploratory and reproducible-build totals separately. “Exploratory” is a stage label, not permission to omit treatment-specific work from a later fully loaded programme-cost sensitivity.

M1 does not amortize these into a system-cost claim. It records them so later accounting cannot erase treatment-specific development effort. The accepted implementation must also be reproducible from the frozen raw source bundle, schemas, compiler mappings, configuration, and build instructions.

## 21.5 Mandatory zero fields

For M1:

- model calls = 0;
- generated model tokens = 0;
- accelerator use is prohibited in an acceptance run and accelerator time = 0;
- persistent model or knowledge-state writes = 0; ordinary result, trace, and manifest files are allowed;
- model-weight changes = 0.

---

# 22. DQ1-M1 Exit Rule

## 22.1 M1 Pass

M1 passes only when:

- every valid public fixture produces the frozen result;
- every invalid fixture fails closed;
- every valid in-domain hidden instance agrees exactly with the independent oracle and every invalid hidden instance fails closed; any semantic mismatch is M1 Fail;
- repeated runs produce byte-identical semantic and deterministic-audit projections and hashes;
- telemetry is complete and valid but is not required to contain identical measured values;
- permuted inputs produce identical semantic projections;
- the exhaustive small-instance oracle agrees;
- every claimed operator is exercised and mutation-tested;
- the combined ambiguity-and-exception trace is independently reviewed;
- the Sanskrit/Pāṇinian microfixture is approved;
- no evaluator-only content enters execution;
- no manual or model judgment is required during execution;
- complete telemetry and reproducibility hashes are produced;
- an independent reviewer reproduces the build and results from the frozen raw artifacts;
- `ModelPayload` contains no post-inference or evaluator field;
- no semantic choice is hidden in implementation code.

`PDSGRO-0.1` remains the immutable artifact identifier even if its attribution is downgraded. The only permitted M1 result is therefore:

> **Artifact PDSGRO-0.1 is executable under the frozen M0 semantics. Frozen attribution label: Pāṇinian-derived residual hypothesis / Generic Sanskrit-inspired machinery.**

Exactly one attribution label must be selected from the Frozen M0 record. Neither label is a DQ7 `Specific` result.

## 22.2 M1 Inconclusive

M1 is Inconclusive when:

- infrastructure fails without testing semantics;
- hidden fixtures are corrupted or leaked;
- the exhaustive oracle is defective;
- the run manifest or hashes are incomplete;
- the implementation cannot be reproduced for reasons not attributable to the mechanism.

An Inconclusive result does not become Pass through interpretation.

## 22.3 M1 Fail

M1 fails when:

- the engine requires manual or model judgment for a claimed core case;
- conflict resolution depends on arbitrary tie-breaking;
- ambiguity or optionality is silently collapsed;
- a scope or protected exception is violated;
- output depends on serialization order or non-semantic identifiers;
- the implementation contains fixture-specific logic;
- the compiler or payload leaks evaluator information;
- execution cannot terminate or lawfully report resource exhaustion;
- the implementation cannot realize the Frozen M0 semantics.

After failure, the programme must:

1. distinguish implementation defect from semantic-contract defect;
2. repair implementation defects without changing M0;
3. reopen M0 under a new version if semantics must change;
4. replay all public tests and use a fresh independently generated sealed acceptance set once hidden failure details have been disclosed;
5. narrow the cross-layer rule-scope claim if a bounded repair cannot make the core executable.

---

# 23. Seal, Custody, and Amendment Rules

## 23.1 Status progression

Allowed M0 statuses:

~~~text
Draft → Reviewed → Frozen
   ↘ Rejected
Frozen → Superseded by a new version
~~~

Only Frozen M0 may govern M1 acceptance.

## 23.2 Required approvals

| Role | M0 responsibility | M1 responsibility |
|---|---|---|
| Mechanism owner | Completeness and implementation feasibility | Declares implementation conformance |
| Sanskrit/Pāṇinian reviewer | Historical and linguistic mapping | Reviews the attested microfixture and claim language |
| Independent methods reviewer | Treatment boundary, leakage, controls, stop rules | Reviews hidden acceptance and result label |
| Independent implementation reviewer | Confirms semantics are independently implementable | Reviews code, tests, reproducibility, and no hard-coding |

The three reviewers other than the mechanism owner must be independent of target implementation and outcome-dependent authorship. All four roles must approve the same normative artifact hash; approval of different revisions does not form a quorum.

## 23.3 Freeze package

The M0 freeze package includes hashes for:

- normative contract;
- `TreatmentSignature`;
- `Compile_T` specification or implementation, mapping tables, and configuration;
- source and target schemas;
- operational semantics;
- declared consequence language and reference denotation;
- `Decode_T` specification and exact target round-trip witness;
- ModelPayload, ExecutionAudit, and TelemetryManifest schemas;
- public fixtures and evaluator oracles;
- hidden-fixture generation specification;
- attribution and traceability ledgers;
- cost-counter specification;
- compiler-interface contract;
- review records.

## 23.4 Hidden-fixture custody

Before M1 acceptance:

- name the hidden-fixture custodian;
- register the contract version, generator version, seed commitment, fixture hashes, and oracle hash in one cryptographic manifest;
- define implementer access rights;
- define the exact unseal event and authorized custodians;
- log every access;
- record any leak or replacement;
- retain the complete result and replacement history across contract versions;
- invalidate the acceptance run if the implementer accessed evaluator-only contents.

## 23.5 Amendments

Any change to:

- schema meaning;
- operator inventory;
- rule ordering;
- aggregation;
- exception, blocking, precedence, optionality, ambiguity, or conflict semantics;
- fixture expected properties;
- resource-exhaustion behaviour;
- treatment boundary;

requires:

- a new document version;
- new hashes;
- renewed review;
- regeneration or pre-unseal revalidation of hidden fixtures;
- complete M1 replay.

An exposed hidden fixture is never revalidated as hidden evidence. Any post-unseal rerun uses a fresh seed commitment and independently generated sealed set, while preserving the earlier result in the history.

Typographic changes that cannot alter interpretation may use a patch version but still require a new file hash and amendment entry.

---

# 24. What M0 and M1 May and May Not Establish

| Stage | Maximum warranted conclusion |
|---|---|
| M0 Frozen | One candidate is precisely specified and independently implementable |
| M1 Pass | The candidate executes reproducibly under the frozen semantics |
| DQ1 Final after successful M2 adjudication | Contribution boundary, prior-art status, equivalent controls, and traceability are defensible enough to test |
| DQ5 | Structure contains comparative graph-only signal |
| DQ6 | A frozen model gains practical value and causally uses the structure |
| DQ7 | Incremental Sanskrit/Pāṇinian value survives competent generic and universal controls |
| DQ8 | Non-oracle structure is practically obtainable at acceptable net cost |
| DQ9 | A retained candidate improves the integrated small-model training frontier |
| DQ10 | The complete system achieves its contracted efficiency outcome |

M0 or M1 must not be cited as evidence that:

- fewer LLM tokens are consumed;
- accuracy or reasoning improves;
- a generic formalism cannot match the mechanism;
- the mechanism is algorithmically novel;
- Sanskrit is uniquely computational;
- the full thesis is supported.

---

# 25. Route After M1

~~~mermaid
flowchart TD
    A["DQ0 mission status checked"] --> B["DQ1-M0: specify one mechanism"]
    B --> C{"M0 review"}
    C -->|"Unformalizable, leaky, or judgment-dependent"| D["Stop this architecture claim; narrow to mechanism or resource work"]
    C -->|"Generic only"| E["Relabel as generic Sanskrit-inspired engineering"]
    C -->|"Repair required"| B
    C -->|"Pāṇinian-labelled residual candidate Frozen"| F["DQ1-M1: deterministic reference interpreter"]
    E --> F
    F --> G{"M1 result"}
    G -->|"Fail: implementation defect"| F
    G -->|"Fail: semantic defect"| B
    G -->|"Fail after bounded repair"| D
    G -->|"Inconclusive"| H["Repair custody or infrastructure; rerun"]
    H --> F
    G -->|"Pass: executable"| I["DQ1-M2: prior art, equivalent controls, complete traceability"]
    I --> J{"Complete DQ1 decision"}
    J -->|"Formalized; generic attribution"| K["DQ2: freeze measurement, fairness, leakage, and cost contract"]
    J -->|"Formalized; residual computational hypothesis"| K
    J -->|"Cannot implement equivalent fair controls"| L["DQ1 remains Not Ready"]
    K --> M["DQ3: data, annotation, compiler, and tool readiness"]
    M --> P["Launch DQ4 token audit and DQ5 structural diagnostic independently in parallel"]
    P --> Q4["Final DQ4 record"]
    P --> Q5["Final DQ5 record"]
    Q4 --> X["AND barrier: both Final records exist"]
    Q5 --> X
    X --> Y{"Paired pilot outcome"}
    Y -->|"Structural component retained"| Q6["DQ6 frozen-model practical and causal value"]
    Y -->|"Only token component retained"| Q9["Token-only DQ9 path"]
    Y -->|"Both rejected"| N["Narrow to resources, tooling, or negative result"]
~~~

The generic branch remains scientifically and practically valid. It cannot use Sanskrit-unique language. DQ4 and DQ5 start only after DQ1, DQ2, and DQ3 are Final/Yes, and DQ6 cannot start until both parallel records are Final.

---

# 26. DQ1-M2 Boundary

M2 is named here only to prevent M1 from being mistaken for DQ1 completion.

M2 must later provide:

- component-by-component prior-art and non-duplication matrix;
- information-equivalent universal formal formulation;
- information-equivalent generic formal formulation;
- anonymized-label formulation;
- well-formed counterfactual formulation;
- type-preserving corruption formulation;
- expressibility and round-trip witnesses for every formulation;
- competence-test specifications for every control;
- the complete condition-specific raw-input-to-output dataflow required by Section 12.3;
- a versioned bill of materials and component genealogy from the neutral source bundle to every claimed model input, including hashed interface specifications, owner, planned implementation gate, and later hash-append obligation;
- complete claim-to-implemented-layer audit;
- a complete DQ1 decision record and honest contribution label.

M2 specifies the equivalent formulations and tests; it does not use DQ5 outcomes to choose them. DQ2 then freezes quantitative competence, leakage, resource, and fairness rules. DQ3 independently implements and tests the condition compilers and tooling. Independent baseline builders may challenge the candidate pool and veto an unfair interface.

DQ1 may become Final only when all six requirements in Section 4 pass. M1 Pass alone leaves `DQ1 status = Unanswered` and `DQ1 readiness = Not Ready`.

---

# 27. Immediate Work Order

The proposed feasibility work order is:

1. obtain formal-semantics, Sanskrit/Pāṇinian, methods, and independent-implementation review of this same version;
2. resolve every blocking review item and record the disposition;
3. complete the prior-art kill screen and, if required, relabel the candidate Generic before implementation;
4. obtain independent control-builder approval of the representation-neutral interface and control-development charter;
5. create the canonical source, target representation, ModelPayload, ExecutionAudit, and TelemetryManifest schemas;
6. author DQ1-M0-F01 through DQ1-M0-F16 and evaluator-only oracles;
7. commission the Sanskrit/Pāṇinian microfixture;
8. complete and review one mapping card for every retained Pāṇinian-labelled claim;
9. freeze the hidden-fixture generator, independent oracle, coverage, thresholds, seed custody, and unseal rule;
10. complete the M0 traceability, cost, review, and hash artifacts;
11. have all four approvers sign the same hash and freeze M0;
12. have the custodian generate and seal the hidden M1 acceptance set;
13. only then implement and accept M1;
14. before DQ1 becomes Final or DQ5 launches, publish an executable pilot revision that chooses the integrate-or-narrow route, physically separates every gold/evaluator field, and aligns conditions, controls, gates, and thresholds with Documents 06 and 07.

Implementation before Step 11 may be used only as disposable feasibility exploration. It cannot determine or silently modify the Frozen semantics. Acceptance implementation begins only after the Step 12 sealed set exists and remains inaccessible to the implementer.

---

# 28. M0 Work-Package Record

| Field | Current value |
|---|---|
| Work-package ID | DQ1-M0 |
| Candidate | Pāṇinian-Derived Scope-Gated Rule Organizer, version 0.1 |
| M0 readiness | Draft / Not Frozen |
| DQ1 status | Unanswered |
| DQ1 readiness | Not Ready |
| Treatment locus | Rule organization and compilation into scope, inheritance, default-exception, blocking, precedence, and optional-choice structures |
| Shared carrier | Language-independent canonical facts, analyses, and event-role relations |
| Executor classification | Generic |
| Memory mode | Read-only, single execution |
| Tokenizer | None; DQ4 remains separate |
| Strongest null | Competent generic organization and ordinary engineering explain any later benefit |
| Next decision | Review and complete the M0 artifact set |

---

# 29. M1 Work-Package Record Template

| Field | Value to be completed after acceptance |
|---|---|
| Work-package ID | DQ1-M1 |
| DQ1 status | Unanswered until successful M2 adjudication |
| DQ1 readiness | Not Ready |
| M0 version and hash |  |
| Interpreter version and hash |  |
| Public fixture manifest hash |  |
| Hidden fixture manifest hash |  |
| Environment manifest hash |  |
| Result | Pass / Fail / Inconclusive |
| Semantic conformance |  |
| Leakage audit |  |
| Determinism audit |  |
| Mutation adequacy |  |
| Independent reproduction |  |
| Permitted conclusion | Executable / Not executable / Inconclusive |
| Prohibited conclusion | No statement of usefulness, efficiency, novelty, or Sanskrit specificity |
| Next step | M2 / repair / reopen M0 / narrow |

---

# 30. DQ1 Decision Record Template

This is the journey-level record that M2 must complete; it is distinct from the M0 and M1 work-package records.

| Field | Value |
|---|---|
| Question ID | DQ1 |
| Status | Unanswered / Provisional / Final |
| Outcome | Formalized-residual-computational-hypothesis / Formalized-generic / Mixed / Cannot formalize |
| Hypothesis and null hypothesis |  |
| Primary estimand and contrast |  |
| Evidence required | Six requirements in Section 4 |
| Strongest competing explanation |  |
| Baselines and controls |  |
| Minimum practically important effect | Not adjudicated by DQ1; cross-reference DQ2 |
| Non-inferiority margin and cost ceiling | Not adjudicated by DQ1; cross-reference DQ2 |
| Joint acceptance and confidence-interval rule | Not adjudicated by DQ1; cross-reference DQ2 |
| Multiplicity, sequential testing, and alpha-spending rule | Not adjudicated by DQ1; cross-reference DQ2 |
| Discovery, selection, and sealed-confirmation datasets |  |
| Uncertainty or confidence interval | Not applicable to formal closure unless an empirical subclaim is used |
| Cost and resource implications |  |
| Decision | Continue / Pivot / Narrow / Pause / Stop |
| Decision owner and independent reviewer |  |
| Date, evidence links, and next review date |  |

---

# 31. Signatures

This Draft becomes Frozen only through recorded approval.

| Role | Name | Decision | Signature or recorded approval | Date |
|---|---|---|---|---|
| Mechanism owner |  | Approve / Amend / Reject |  |  |
| Sanskrit/Pāṇinian reviewer |  | Approve / Amend / Reject |  |  |
| Independent methods reviewer |  | Approve / Amend / Reject |  |  |
| Independent implementation reviewer |  | Approve / Amend / Reject |  |  |

---

# 32. Amendment Log

| Version | Date | Change | Reason | Approval status |
|---|---|---|---|---|
| 0.1 | 20 August 2026 | Initial M0/M1 mechanism-resolution contract | Resolve DQ1 underspecification before architecture expansion | Draft |
| 0.2 | 21 August 2026 | Added neutral task theory, target signature, formal branch semantics, payload/audit separation, fair-control governance, prior-art kill screen, and repaired journey route | Independent formal, methodological, and cross-document red-team review | Draft; Pass 2 aligned |

---

# 33. Source Crosswalk

| Source | Normative or technical role in this document |
|---|---|
| Document 06, DQ1 | Required evidence, contribution boundary, consequences, and journey position |
| Document 07 | Version 1 mission, minimal rule-scope requirement, exclusions, information/leakage contract, public-claim limits, and DQ0 signature status |
| Document 03, Sections 6.11, 16, and 18 | Candidate Pāṇinian-to-engineering mappings, strong generic controls, and representation-before-model sequencing |
| Document 05 | Warning against flat root-centred structure, attribution overreach, and premature architecture expansion |
| Pilot, Sections 2, 11, 13, 14, 20, and 21 | Funding thesis, minimal-stack contradiction, condition namespace, information-equivalence requirement, controls, and co-primary success claims |
| Document 02 | Broader legacy rule-scope and propagation-locality concepts retained only as technical background |

---

# 34. Final Governing Statement

> DQ1-M0 and DQ1-M1 exist to make the proposed mechanism precise enough to fail before expensive model work begins. A coherent and executable mechanism earns the right to face strong controls; it does not earn a claim of usefulness, efficiency, novelty, or Sanskrit-specific causation.
