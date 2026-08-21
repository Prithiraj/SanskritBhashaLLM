# Sanskrit-Derived Efficient LLM
## Mission and Falsification Contract

**Document type:** Binding DQ0 programme contract  
**Version:** 0.3  
**Date:** 20 August 2026  
**Decision status:** Ready for DQ0 mission signature; numerical schedules remain Provisional until DQ2  
**Governing register:** 06_Sanskrit_Derived_Efficient_LLM_Research_Question_Register_and_Decision_Tree.md

---

# 1. Contract Authority

Upon DQ0 mission signature, this contract governs the Version 1 mission, branch logic, claim hierarchy, and stop rules. Its numerical schedules become binding only when confirmed or replaced in the separately signed DQ2 threshold appendix. It supersedes conflicting classifications of primary, secondary, and exploratory objectives in Documents 01-05 and in the pilot. Companion documents remain technical sources, but they do not override the signed portions of this contract.

This contract operationalizes DQ0 in Document 06. If the two documents conflict, this contract controls the Version 1 mission, numerical thresholds, evidence labels, and falsification rules; Document 06 controls journey order and gate routing. Any residual conflict pauses the affected decision until a versioned amendment resolves it.

No threshold, endpoint, baseline, cost boundary, or success label may be changed after sealed confirmatory results are opened. A later change requires a versioned amendment, an explicit rationale, new signatures, and a fresh sealed evaluation set.

A result is classified from this contract; this contract is not rewritten to fit a result.

---

# 2. Binding Core

## Mission

> **Engineering mission:** develop a research-scale general or multilingual LLM that improves the verified accuracy-and-reasoning versus complete-cost frontier through one or more representations or inductive biases originating in Sanskrit and Pāṇinian analysis.

> **Scientific mission:** determine causally whether any gain comes from Sanskrit surface form, morphology, Pāṇinian organization, structured information generally, privileged supervision, or ordinary engineering choices.

## Primary target

The Version 1 target is an English-capable, open-weight multilingual model whose user interface can accept and return English while Sanskrit or Pāṇinian structure may operate internally. Users must not need to know Sanskrit.

Sanskrit is also a user-facing evaluation language and experimental testbed. Until DQ11 passes its breadth contract, the system must be described as a Sanskrit-English cross-lingual research prototype, not a general or multilingual production LLM.

## Intended users and setting

The initial users are ML researchers, computational linguists, Sanskrit scholars, and research engineers evaluating model efficiency and causal mechanisms. Version 1 is not a public, high-stakes, legal, medical, scientific-authority, educational-certification, or government-deployment system.

## Model class and development sequence

Version 1 uses:

- one open multilingual decoder backbone in the approximately 1-3 billion parameter range for the first frozen-model experiment;
- matched structural encoders, adapters, and control capacity;
- a second distinct backbone for confirmation before a reusable architecture claim;
- a small integrated training experiment only after the token or structural candidate earns entry through the journey gates.

The first phase freezes principal backbone weights. A custom tokenizer is evaluated in the token audit and later integrated training experiment, not retrofitted into the frozen-backbone causal comparison.

## Version 1 includes

- a matched token and representation audit;
- a graph-only structural diagnostic;
- a frozen-model practical and causal comparison;
- a minimal rule-scope core covering defaults, precedence, optionality, blocking, and exceptions whenever the public claim invokes those mechanisms;
- Sanskrit/Pāṇinian versus universal, generic, learned, controlled-language, anonymized, and corrupted controls;
- usable-structure testing whenever deployed inference predicts, constructs, or consumes explicit structure;
- a small integrated-model experiment for components that survive;
- complete-system token, information, training, deployment, and lifecycle accounting;
- clean-room, modern technical, and attested natural evaluation material.

## Version 1 excludes

- persistent self-assimilation;
- writable institutional memory;
- fast weights, durable model editing, and base-weight rewriting;
- unrestricted continual pretraining;
- full discourse, Vedic, Chandas, kāvya, manuscript, recitation, and prosodic systems unless separately approved;
- national-scale corpus construction;
- large-model or national-deployment claims;
- claims that the model “thinks in Sanskrit”;
- claims of universal Sanskrit superiority;
- claims that external evidence or retrieval is unnecessary.

## Binding success hierarchy

1. **Tier A system win:** tokens and complete-system cost both fall while accuracy and out-of-distribution reasoning both improve, with every floor satisfied.
2. **Tier B engineering-frontier win:** quality improves at non-higher cost, or cost falls with non-inferior quality.
3. **Mechanism-only result:** tokenization, morphology, structure, tools, or resources help without a Tier A or Tier B system win.
4. **No validated architecture result:** neither retained component improves the confirmatory frontier.

The **full Version 1 core thesis** requires, within one preregistered retained system line:

- a Tier A system win;
- a DQ7 Specific result for at least one Sanskrit/Pāṇinian-derived component actually used by the Tier A configuration;
- a DQ9-DQ10 ablation or competent-replacement contrast showing that this component makes a positive incremental contribution meeting its DQ2 practical margin, with its 95% confidence interval excluding no benefit, to at least one Tier A token, cost, accuracy, or reasoning conjunct while the retained configuration satisfies every Tier A conjunct;
- the DQ11 breadth contract; and
- independent DQ14 replication.

Results from different candidates, dropped components, non-overlapping workloads, or separate system configurations may not be combined to obtain the full-thesis label. Anything less receives the narrower label specified in this contract.

---

# 3. Evaluation Scope

## 3.1 Evaluation worlds

The confirmatory evaluation must include three separately reported worlds:

1. **Clean-room fictional world:** nonce entities, unseen rule combinations, counterfactual relations, and no plausible pretraining memorization.
2. **Modern technical world:** science, mathematics, algorithms, code explanation, law-like rules, and contemporary dialogue.
3. **Attested natural Sanskrit world:** real inflection, derivation, compounds, polysemy, lexicalization, ambiguity, and protected exceptions.

A positive result confined to engineered terminology cannot establish the core thesis.

## 3.2 Task families

The evaluation must cover:

1. novel-expression understanding;
2. low-shot concept acquisition;
3. event and paraphrase reasoning;
4. general reasoning that cannot be solved through morphology alone, including arithmetic, logic, causal inference, rule execution, elementary science, and algorithms.

For Tier A and the Tier B quality-win route, apply the family-direction rule separately to each co-primary endpoint: accuracy and OOD reasoning must each have a positive preregistered point estimate in at least three of the four task families, and both must be positive in the general-reasoning family. Every remaining endpoint-by-family cell must stay within its 2-point non-inferiority floor. A Tier B cost win does not require positive gains in three families, but both endpoints must remain within the 2-point floor in every family.

## 3.3 Primary accuracy endpoint

The accuracy endpoint is the equal-weight macro average of exact, numerical, executable, or unit-tested correctness across the preregistered world-by-task cells outside the OOD reasoning pool.

Accuracy and reasoning must use disjoint scored item pools. If an item necessarily serves both analyses, it is counted only once in the joint gate and its assignment is frozen before evaluation.

Where deterministic verification is impossible, blinded adjudication rules and inter-rater agreement must be frozen before evaluation.

Fluency, explanation length, Sanskrit terminology, and structural-trace plausibility are not accuracy evidence.

## 3.4 Primary reasoning endpoint

The reasoning endpoint is a separate equal-weight macro score of verified correctness on held-out composition, counterfactual causal inference, and multi-step rule, numerical, and algorithmic execution. Its preregistered stress-test strata include:

- held-out compositional combinations;
- counterfactual rule execution;
- algorithm execution;
- paraphrase consistency;
- robustness to irrelevant distractors;
- nonce entities and reversed correlations.

Each item must have a deterministically checkable or blinded outcome. Reasoning-item construction and evaluation must be independent of the team that constructs the Sanskrit/Pāṇinian treatment. Generated chain-of-thought is counted as cost and may be analyzed diagnostically, but it is not evidence of reasoning unless its causal faithfulness is independently demonstrated.

Mechanism interventions belong to DQ7 and are not scored again as reasoning items.

## 3.5 Secondary measures and floors

Report calibration, abstention, coverage, factual groundedness, sample efficiency, retrieval use, per-family performance, latency, memory, and safety-relevant regressions separately.

The provisional planning floors are:

- no more than 2 percentage points absolute loss on any preregistered unrelated general-capability aggregate;
- no more than 2 percentage points absolute loss on any protected major task family;
- at least 95% answer coverage unless the task explicitly evaluates abstention;
- selective comparisons at matched coverage;
- p95 latency no more than 5% above the strongest baseline for Tier A;
- peak deployed memory no more than 10% above the strongest baseline for Tier A;
- p95 latency and peak deployed memory no more than 10% above the strongest baseline for Tier B;
- no material safety or calibration regression defined by DQ2.

---

# 4. Baseline and Information Contract

## 4.1 Primary reference

The reference is the preregistered Pareto frontier of ordinary models selected from a frozen candidate pool under an equal search budget. Quality comparisons use the strongest ordinary model at matched total execution cost. Cost comparisons use the cheapest ordinary model reaching matched accuracy, reasoning, coverage, and latency. Integrated training additionally requires parameter-matched and training-compute-matched references.

Before sealed evaluation, freeze every model identity and size plus the implementation, version, maintainer, recipe, selection objective, hyperparameter-search space, tuning allocation, stopping rule, and competence test for every baseline and control. All comparisons use the same semantic workload, hardware, coverage, context, output, and applicable resource boundary. A post-result baseline substitution requires a new sealed evaluation and cannot rescue the original claim.

Frozen-model causal tests use the identical backbone for all conditions.

## 4.2 Required comparison families

DQ2 must contain a signed applicability matrix covering every condition below; a condition cannot become “not applicable” after results are visible. The final relevant experiment must include every condition marked applicable:

- ordinary English text;
- ordinary Sanskrit text;
- serialized structure;
- off-sequence Pāṇinian-derived structure;
- universal linguistic structure;
- generic executable structure;
- controlled descriptive English;
- learned latent structure;
- anonymized structural labels;
- type-preserving shuffled or corrupted structure;
- well-formed counterfactual structure;
- no-structure and extra-capacity controls.

Every structural control must pass an empirical competence threshold showing that it can express and execute the same task-relevant facts, rules, exceptions, and scope relations before comparative results are unsealed. Controls receive equal tuning and expert-engineering budgets and are calibrated by reviewers independent of the treatment implementation.

## 4.3 Information equivalence

Matched-semantic-content and matched-resource-budget comparisons are separate estimands.

For every condition, report:

- all model-visible facts, relations, labels, decompositions, and supervision;
- input, retrieved, cached, tool-mediated, and generated tokens across all calls;
- raw bytes and compressed bits;
- graph nodes, edges, vectors, and transfer bytes;
- total and trainable parameters;
- vocabulary, embedding, and output-head costs;
- parser, compiler, teacher, translation, and annotation supervision.

Gold answers, proof steps, test-derived consequences, and evaluator labels remain evaluator-only.

A side-channel-only adversarial probe must test whether answers, proof steps, or task decompositions can be recovered without the model input. Evaluator or sealed-test leakage invalidates the run. A lawful preprocessing or compiler path that itself produces the answer invalidates attribution to model reasoning, but it may remain a separately labelled and fully costed tool-system result.

## 4.4 Causal estimands and exposure control

No single surface-language-by-structure comparison may be interpreted as isolating all proposed contributions. The attribution plan must separately identify, or explicitly leave unresolved:

- surface language;
- tokenizer and encoding;
- morphology and lexical decomposition;
- Pāṇinian rule organization;
- label semantics and annotation richness;
- availability of structure at training or inference;
- added teacher, compiler, supervision, parameter, and tuning capacity;
- prior language exposure in the backbone.

A two-factor design estimates only its named factors and interaction, conditional on everything else held fixed. Any unfactored contribution receives an Unresolved or narrower label.

Run two distinct estimands:

1. **Controlled exposure:** matched-from-scratch, synthetic, or isomorphic encodings with item-level parallel semantics, counterbalancing, matched exposure, and measured translation or compilation error.
2. **Ecological deployment:** the same real pretrained backbone across conditions, with its native tokenizer retained in the frozen-model comparison.

An identical frozen backbone controls weights but does not erase unequal pretraining exposure. Therefore, the ecological estimand alone cannot establish a causal surface-language advantage.

Training-only, joint, or distilled structure must compare matched students trained with authentic Pāṇinian, universal or generic, anonymized, well-formed counterfactual, and shuffled supervision while holding teacher, data, student, and tuning budgets fixed. Unless mediation through the claimed organization is demonstrated, the surviving label is **training-signal-derived**, not a runtime Pāṇinian reasoning mechanism.

---

# 5. Cost and Lifecycle Contract

## 5.1 Separate ledgers

The programme maintains four ledgers:

1. **Representation:** all tokens, bits, graph objects, and transferred bytes.
2. **Model development:** data, annotation, grammar and compiler engineering, tokenizer training, model training, tuning, failed runs, compute, energy, wall time, and money. Partition this into the reproducible build of the frozen candidate and exploratory R&D; report both, but amortize only the reproducible build in the primary lifecycle comparison.
3. **Deployment:** translation, normalization, parsing, graph construction, inference, retrieval, tools, retries, verification, storage, maintenance, latency, energy, and money.
4. **Lifecycle:** reproducible candidate-construction and recurring costs under the fixed usage scenario below. Exploratory R&D remains a separately reported programme cost and cannot be silently moved into an appendix or omitted.

No unweighted scalar may hide different cost units.

## 5.2 Primary lifecycle scenario

The Version 1 planning scenario is:

- one declared end-to-end reproducible construction cycle for the retained configuration, including every tokenizer, adapter, parser, compiler, and small-model training step it requires;
- 100,000 attempted evaluation-equivalent requests over 12 months;
- equal planned weight across the three evaluation worlds and four task families, subject to preregistered not-applicable cells;
- primary batch size 1 and secondary throughput batch size 16;
- nominal fixed-budget analysis at up to 1,024 input or retrieved tokens and 256 generated tokens;
- at least 95% answer coverage;
- a frozen hardware configuration, software stack, compiler settings, and price or energy conversion sheet.

Training and one-time system-construction costs are amortized over 100,000 requests only for the lifecycle result. They are also reported unamortized.

Report lifecycle sensitivity at 10,000 and 1,000,000 requests and the measured break-even volume. These are diagnostics; 100,000 requests remains the primary denominator.

The sealed DQ10 workload must also contain preregistered short- and long-context strata and low- and high-retrieval strata within the supported context window. Results are reported separately by stratum; every regression floor applies within each stratum, and a full-thesis claim requires the Tier A quality and efficiency directions to reproduce without a DQ2-defined material reversal in any stratum.

## 5.3 Primary recurring deployment and lifecycle cost

The primary deployment-cost measure is hardware-normalized execution cost per 1,000 attempted requests:

- measured accelerator-seconds multiplied by a frozen rate;
- measured CPU-seconds multiplied by a frozen rate;
- storage and network transfer under a frozen rate;
- all initialization, model loading, translation, parsing, graph, retrieval, retry, and verification work included under the declared request schedule.

The primary lifecycle cost is the reproducible construction cost plus all deployment and maintenance cost in the 100,000-request scenario. Tier rules below state whether deployment cost, lifecycle cost, or both must pass; neither may be described generically as “complete cost” without naming the ledger.

Also report the raw cost vector, energy where measurable, FLOPs where measurable, cost per correct result at fixed coverage, p50 and p95 latency, peak memory, and KV-cache use.

---

# 6. Threshold Sheet

All numerical values in §§3.5, 5.2, 6, and 7 are **provisional planning values pending DQ2**. DQ2 must confirm or replace them using baseline distributions, power and measurement-reliability analysis, resource constraints, and a justified lifecycle workload. DQ0 locks the mission, estimands, branch logic, and direction of every inequality; confirmatory work may not begin until the separately signed DQ2 threshold appendix is Final.

After DQ2 signature, no number may change because of observed confirmatory results. A later change requires a versioned amendment, a fresh sealed set, and new signatures.

For programme decisions, this schedule supersedes the pilot's 25% raw-language token target and 50% oracle-retention proposal. Until DQ2 confirms or replaces them, the 20% token candidate threshold and 70% runtime-retention threshold below are planning values, not empirically justified constants.

## 6.1 Tier A — Full Version 1 system win

All conditions must hold on the same sealed workload mix against the primary reference:

| Measure | Minimum practical effect |
|---|---:|
| Total sequential tokens across all calls | At least 20% lower |
| Primary accuracy endpoint | At least 5 percentage points higher |
| Primary OOD reasoning endpoint | At least 5 percentage points higher |
| Primary recurring deployment cost | At least 20% lower |
| Lifecycle cost including amortized training and recurring operation | At least 20% lower |
| Integrated small-model training frontier | DQ9 pass under §6.4 |
| Capability, coverage, latency, memory, safety, and information floors | All satisfied |

A large vocabulary, hidden side channel, external tool, or parser cannot create a token win by moving uncounted information or cost outside the token stream.

## 6.2 Tier B — Engineering-frontier win

A Tier B result requires either:

### Tier B cost win

- primary lifecycle cost at least 20% lower;
- primary deployment-cost point estimate no higher, with its confidence bound inside the DQ2 measurement-tolerance margin;
- accuracy no worse than 2 percentage points;
- OOD reasoning no worse than 2 percentage points;
- all coverage, latency, memory, safety, information, and protected-capability floors satisfied.

### Tier B quality win

- accuracy at least 5 percentage points higher;
- OOD reasoning at least 5 percentage points higher;
- primary deployment- and lifecycle-cost point estimates each no higher, with their confidence bounds inside the DQ2 measurement-tolerance margins;
- all coverage, latency, memory, safety, information, and protected-capability floors satisfied.

Tier B does not establish the full token-plus-accuracy-plus-reasoning thesis.

## 6.3 Token or representation mechanism result

A token-count candidate is retained for DQ9 when semantically equivalent content uses at least 20% fewer total sequential tokens under matched tokenizer capacity, with non-inferior semantic fidelity across tokenizer families and reproduction on both natural-language and modern-domain material. Bytes, compressed bits, vocabulary and output-head memory, compute, and deployment cost are mandatory separate measurements.

The stronger label **representation compression** additionally requires that compressed bits fall by the DQ2 margin and vocabulary, memory, and compute costs do not erase the claimed benefit. Fewer UTF-8 bytes are not required for the narrower token-count label.

If token count falls but complete-system cost does not, report only a token, representation, or context-compression result.

## 6.4 Integrated training-frontier result

DQ9 passes only when one frozen candidate is evaluated at at least two preregistered modest model sizes and at least three preregistered training-budget points per size, and the frozen final comparison satisfies one of these routes:

- **training-cost route:** at least 20% lower total reproducible training cost to reach the reference target, with accuracy and reasoning each no worse than 2 percentage points; or
- **training-quality route:** accuracy and reasoning each at least 5 percentage points higher, with total reproducible training cost no more than 5% higher.

Training tokens, examples, accelerator and CPU time, FLOPs where measurable, energy, wall time, and failed confirmatory runs are reported separately. No budget point or stopping target may be selected after sealed results are opened.

## 6.5 Specific Sanskrit/Pāṇinian attribution

A DQ7 result is Specific only when all of the following hold:

- every Pāṇinian layer named in the claim is implemented and competence-tested, including the minimal rule-scope core when defaults, precedence, optionality, blocking, scope, or exceptions are claimed;
- on the identified structural contrast, the Pāṇinian-derived condition exceeds the strongest competent universal, generic, controlled-language, learned-latent, and well-formed alternative representation by at least 3 percentage points on the reasoning endpoint;
- it is non-inferior on accuracy within 2 percentage points and satisfies all protected floors;
- the point estimate meets the practical margin and the confidence interval excludes no incremental benefit;
- type-preserving shuffle, corruption, or well-formed counterfactual replacement removes at least half of the incremental advantage;
- preregistered interventions produce the predicted target-specific change in verified output or calibrated probability while preserving non-target behaviour; latency, retrieval activity, or an unspecified behavioural change cannot alone satisfy causality;
- the controlled-exposure comparison meets the 3-point Specific threshold, while the ecological pretrained comparison has the same direction and its 95% confidence interval excludes harm worse than 2 percentage points;
- the Pāṇinian-minus-strongest-control point estimate is positive separately on modern technical and attested natural material;
- the English-input to internal-Pāṇinian-structure to English-output comparison has the same direction and excludes harm beyond the 2-point margin.

“Specific” means incremental value over the preregistered tested alternatives. It does not mean metaphysical uniqueness or universal Sanskrit superiority.

If the minimal rule-scope core is not implemented, the attribution claim is automatically narrowed to the implemented lexical, derivational, compound, and event-role layers; the full cross-layer exception-and-scope thesis is unavailable.

## 6.6 Usable structure

Where runtime structure is required:

- the oracle effect must first deliver at least a 3-point reasoning gain, a 5-point accuracy gain, or a 20% deployment-cost reduction with accuracy and reasoning each within 2 points, and its confidence interval must exclude a null or harmful effect;
- before unsealing, freeze one primary oracle route, metric, baseline, and retention formula; for a higher-is-better endpoint, retention equals `(usable - baseline) / (oracle - baseline)`, while for a cost reduction it equals `(baseline - usable) / (baseline - oracle)`;
- usable predicted, ensemble, or jointly predicted structure must preserve at least 70% of the oracle gain, with a bootstrap 95% lower confidence bound above 50%;
- after every runtime cost is included, the predicted-structure condition must itself satisfy at least one oracle practical-effect route above and every applicable floor;
- complete deployment cost must remain no more than 5% above the matched no-structure reference, unless the claimed mechanism is itself a cost win, in which case the applicable 20% reduction governs.

The usable and oracle effects must use the identical workload, units, and baseline. A different oracle route may not be selected after results are visible; if multiple oracle benefits are claimed, each claimed benefit is tested separately. A retention ratio is invalid when the oracle denominator is tiny, negative, or too uncertain.

A point estimate from 50% to below 70% is a tooling or claim-narrowing result, not an architecture-readiness pass. A point estimate below 50% fails DQ8 unless a bounded tool-improvement or internalization plan was approved before unsealing.

---

# 7. Statistical and Confirmation Rule

- Discovery, candidate selection, and sealed confirmation use disjoint data.
- One final candidate and all baselines are frozen before the sealed run.
- Use at least five random seeds per primary confirmatory condition on each backbone.
- Tier A uses an intersection rule: every conjunct must pass.
- For improvement claims, the point estimate must meet the practical-effect threshold and the 95% confidence interval must exclude no improvement.
- For non-inferiority claims, the 95% confidence bound must remain inside the stated margin.
- Co-primary accuracy and reasoning endpoints both pass; one cannot compensate for the other.
- Secondary families use a preregistered multiplicity correction.
- Sequential component screening uses a preregistered alpha-spending or selective-inference rule.
- A second backbone is confirmation, not another opportunity to choose the better result.
- The full thesis requires the preregistered principal Tier A and Specific effects to reproduce on the second backbone and in an independent DQ14 replication; pooling a failure with a success does not pass.
- A result that meets a point threshold but has an interval crossing the null is Inconclusive.
- Statistical significance without the practical margin is not a pass.

---

# 8. Falsification, Pause, and Pivot Rules

## 8.1 Full thesis not supported

The full Version 1 thesis is not supported if any Tier A conjunct fails on the sealed confirmatory evaluation.

The programme must not relabel a Tier B, attribution-only, tokenizer-only, or structural-tool result as the full thesis.

## 8.2 Stop or narrow the architecture claim

Stop or substantially narrow the model-architecture claim when any applicable condition holds:

- neither the token path nor the structural path survives its bounded pilot;
- DQ9 fails to improve the integrated small-model training frontier;
- DQ10 yields neither Tier A nor Tier B;
- structural interventions show that the model ignores the structure;
- authentic and type-preserving shuffled structure perform equivalently and no independently positive generic structural system remains;
- general reasoning or a protected capability breaches its floor;
- runtime parsing or structural construction destroys net benefit and no preregistered training-only, distilled, or tooling route remains;
- the apparent gain comes from hidden information, extra parameters, extra supervision, or unmatched tuning;
- end-to-end cost overwhelms the measured benefit.

Datasets, tools, parsers, negative results, and valid narrower components must still be preserved and reported.

## 8.3 Downgrade Sanskrit-specific attribution without killing engineering value

Classify the result as Generic, Surface-associated, or Inconclusive rather than Specific when:

- universal linguistic or generic executable structure matches the target;
- controlled English or another well-formed representation matches the target;
- anonymization removes the gain and pretrained label semantics explain it;
- shuffled, counterfactual, or corrupted organization does not remove the advantage;
- the controlled-exposure experiment fails while the pretrained experiment wins;
- translation or compilation fidelity explains the contrast;
- power or control competence is insufficient to separate mechanisms.

A negative attribution result does not terminate a Tier A or Tier B engineering result. It terminates the claim that Sanskrit/Pāṇinian organization is the incremental cause.

Failure to reproduce on natural Sanskrit or modern technical material routes the result to DQ11 for a narrower world or domain label; it does not erase an independently validated benefit in the world where it occurred. A runtime-feasibility failure routes to the DQ8 training-only, distilled, or tooling branch when such a route was preregistered.

Within this contract version, DQ9 No, DQ10 No, or failure of a Tier A conjunct is terminal for the corresponding Version 1 claim. DQ11 may assign only a narrower destination; it cannot upgrade or revive a rejected efficiency or attribution claim. Revival requires a materially new mechanism, a new contract version, fresh sealed data, and an explicitly new hypothesis, not reinterpretation of the failed run.

## 8.4 Pause rather than interpret

Pause and repair before opening or interpreting confirmatory results when:

- semantic or information equivalence is not established;
- a required baseline fails its competence test;
- evaluation contamination or leakage is detected;
- sample size or measurement reliability cannot resolve the practical margin;
- parser, translation, or annotation error is unmeasured;
- implementation differs across conditions beyond the preregistered treatment;
- the sealed set was exposed during development.

Only one bounded repeat is permitted when its trigger and scope were authorized before unsealing. Otherwise the result is Inconclusive and a new version is required.

## 8.5 Allowed destinations

The DQ11 breadth contract is binding:

- **Multilingual** requires Sanskrit plus at least three non-Sanskrit languages spanning at least two language families and two scripts, including at least one non-Indic language.
- **General** requires at least three user-valued domains and all four independently constructed reasoning task families.
- Either label requires at least two backbone or model families, natural and clean-room material, fixed regression floors, and evaluators independent of dataset and terminology construction.

Before these conditions pass, the strongest permitted description is a cross-lingual or cross-domain pilot.

| Evidence outcome | Required destination label |
|---|---|
| Tier A + Specific + breadth + replication | Full Sanskrit-derived efficient-LLM thesis |
| Tier A without Specific, with DQ11 breadth | Strong efficient general or multilingual system; Sanskrit was a scaffold or source |
| Tier A without Specific, without DQ11 breadth | Strong efficient system at the demonstrated cross-lingual or domain scope; Sanskrit was a scaffold or source |
| Tier B + Specific | Partial Sanskrit-derived engineering result |
| Tier B without Specific | Efficient generic structured system or component |
| Token result only | Sanskrit tokenization or representation result |
| Frozen structural result only | Structural adapter, retrieval, or augmentation system |
| Sanskrit tasks only | Sanskrit NLP or Sanskrit-native model |
| Selected domains only | Domain-specific structured reasoning system |
| Tools or data only | Sanskrit NLP infrastructure |
| No reproducible benefit | Negative architecture result and artifact release |

---

# 9. Public-Claim Restrictions

Before a positive result, the programme may say only:

> We are testing whether Sanskrit-derived representations or Pāṇinian structural mechanisms can improve token consumption, verified accuracy, out-of-distribution reasoning, and complete-system cost, while separating Sanskrit-specific effects from generic structure and ordinary engineering.

The programme must not use “demonstrates,” “proves,” “Sanskrit is uniquely computational,” “general LLM,” or “multilingual efficiency” until the corresponding gate and breadth requirements pass.

Even a Tier A pilot does not establish national-scale readiness, high-stakes reliability, safe self-assimilation, lifelong learning, or universal superiority.

---

# 10. DQ0 Decision Record

| Field | Contracted value |
|---|---|
| Question ID | DQ0 |
| Status | Mission and branch logic Provisional until DQ0 signatures; numerical schedule Provisional until DQ2 signature |
| Outcome sought | Yes: operational mission and decision rule locked |
| Engineering hypothesis | A retained Sanskrit/Pāṇinian-derived component can produce a Tier A or Tier B general/cross-lingual system result |
| Scientific hypothesis | A controlled experiment can distinguish Pāṇinian structure from surface, generic structure, privileged information, and ordinary engineering |
| Engineering null | No retained component improves the preregistered quality-cost frontier |
| Attribution null | Competent universal or generic alternatives explain any observed gain |
| Primary estimands | Tier A system contrast; Tier B frontier contrast; DQ7 incremental attribution contrast |
| Strongest competing explanations | Tokenizer choice, pretraining exposure, translation quality, extra supervision, side-channel leakage, generic structure, extra capacity, benchmark alignment |
| Decision | Sign and proceed to DQ1, or amend before any confirmatory work |
| Next gate | DQ1 — Mechanism Specification and Contribution Boundary |

---

# 11. Signatures and Amendment Control

By signing, the parties accept that a culturally meaningful or elegant architecture is not evidence, that negative results are publishable outcomes, and that success labels cannot be renegotiated after unsealing.

| Role | Name | Decision | Signature or recorded approval | Date |
|---|---|---|---|---|
| Project owner |  | Approve / Amend / Reject |  |  |
| ML research lead |  | Approve / Amend / Reject |  |  |
| Sanskrit or Pāṇinian domain reviewer |  | Approve / Amend / Reject |  |  |
| Independent methods reviewer |  | Approve / Amend / Reject |  |  |

**DQ0 mission and branch logic become Final/Yes only when the project owner and independent methods reviewer approve this version. The numerical threshold schedule becomes Final only through the separately signed DQ2 appendix.**

Amendment log:

| Version | Date | Section changed | Reason | New sealed data required? | Approvals |
|---|---|---|---|---|---|
| 0.1 | 20 August 2026 | Initial contract | Establish DQ0 | Yes | Superseded by 0.2 |
| 0.2 | 20 August 2026 | Authority, endpoint separation, causal controls, Pareto baselines, cost definitions, provisional thresholds, DQ8-DQ11 routing, and replication | Close Pass 1 audit loopholes | Yes | Superseded by 0.3 |
| 0.3 | 20 August 2026 | Same-system-line evidence join, endpoint-family gate, context and retrieval strata, oracle formula, two-size DQ9 rule, and destination labels | Close Pass 2 audit loopholes before DQ0 mission signature | Yes | Pending |
