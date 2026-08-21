# Sanskrit Structural Efficiency and Novelty-Isolation Pilot
## Controlled First Experiment for the Śāstrīya-Bhāṣā Foundation Model Programme

**Document type:** First-experiment design and funding-readiness protocol  
**Programme:** Śāstrīya-Bhāṣā Foundation Model Programme  
**Working architecture:** Sanskrit Structural Self-Assimilating Foundation Model, with a Pāṇinian grammatical core  
**Version:** 1.1  
**Date:** August 2026  
**Status:** Legacy pilot-design source — sealed execution on hold pending DQ0-DQ3 and the DQ1 mechanism decision

---

# 1. Purpose

This document defines the **first experiment** that should be run before attempting a large Sanskrit-native foundation model, a national knowledge commons, persistent self-assimilation, dynamic routing, fast-weight adaptation, or base-model consolidation.

The experiment has two equally important objectives:

1. determine whether the approach provides **practical value** through lower token use, stronger reasoning, higher answer accuracy, and better sample efficiency;
2. determine whether any improvement is caused by a **genuinely distinctive Sanskrit structural mechanism**, rather than by a better tokenizer, additional annotation, descriptive terminology, generic graph structure, or extra parameters.

The programme should not advance to a large public funding request merely because the Sanskrit condition performs well. It should advance only if the first experiment demonstrates both **usefulness** and **mechanism-level novelty**.

## DQ1 execution hold

This document is not, by itself, an executable preregistration. Document 06 governs the programme route; Document 07 will govern the mission upon DQ0 signature; Draft Document 08 specifies the current DQ1-M0/M1 work, while only its Frozen version will govern acceptance and the mechanism boundary.

No sealed run of Track 1 or Track 2 may begin until DQ0, DQ1, DQ2, and DQ3 have the required Final records. In particular, the current Track 2 definition invokes cross-layer organization, inheritance, exceptions, and scope while Section 11 implements only lexical/inflectional, derivational, compound, and event-role layers and says the pilot need not depend on the full rule-scope architecture.

Before this pilot can become executable, a new version must take exactly one of two routes:

1. **Integrate the mechanism:** add the Frozen DQ1 rule-scope core to S2 and to information-equivalent universal and generic controls; revise the schemas, conditions, costs, competence tests, ablations, and claim-to-layer traceability accordingly.
2. **Narrow the claim:** remove the S-E exception/scope condition and every funding, novelty, causal, and success statement that attributes a benefit to cross-layer inheritance, exceptions, or scope; limit the pilot to the four implemented representational layers.

Until one route is approved, S2 cannot be interpreted as evidence for the cross-layer exception-and-scope thesis. This hold does not reject the token audit or four-layer representation study; it prevents them from being used to support a mechanism they do not implement.

---

# 2. Funding Thesis

Efficiency by itself is insufficient as a strong research novelty claim.

A Sanskrit-native tokenizer may reduce sequence length, and a Sanskrit-capable model may improve Sanskrit tasks. Those outcomes would be useful, but they would not independently distinguish the programme from existing work in:

- Sanskrit language modelling;
- Sanskrit-specific and Indic tokenization;
- byte-level Sanskrit morphology;
- computational Pāṇinian analysis;
- generic semantic graphs;
- structured retrieval;
- persistent memory;
- continual-learning and model-editing systems.

The fundable hypothesis is narrower:

> **A compact Sanskrit-native token stream, combined with an off-sequence executable Sanskrit Structural Stack, produces a superior accuracy–token–compute trade-off, and that advantage is specifically caused by Sanskrit’s cross-layer organization, inheritance, exception, and scope mechanisms rather than by structured information generally.**

This creates two independent funding gates.

## Gate A — Practical Value

The approach should demonstrate one or more of the following:

- fewer tokens for equivalent semantic content;
- higher answer accuracy at the same token budget;
- equal accuracy at lower end-to-end compute;
- better reasoning and compositional generalization;
- fewer examples required to acquire a new concept;
- lower retrieved-context consumption;
- stable performance on modern technical material, not only classical Sanskrit.

## Gate B — Mechanism Novelty

The target Sanskrit structural condition should outperform strong matched alternatives and lose a meaningful portion of its advantage when its authentic organization is removed, shuffled, corrupted, or replaced.

Passing Gate A means the system is useful.

Passing both Gate A and Gate B means the system may be scientifically distinctive and suitable for a stronger institutional funding proposal.

---

# 3. Primary Research Questions

The pilot should answer four questions.

## RQ1 — Token Efficiency

> Does fair Sanskrit-native tokenization represent semantically equivalent modern content using fewer tokens than a matched English tokenizer?

## RQ2 — Reasoning and Accuracy

> Does selected explicit Sanskrit structural information improve reasoning quality and answer accuracy over Sanskrit text alone?

## RQ3 — Accuracy–Efficiency Frontier

> Does the target Sanskrit structural condition provide more correct answers per token and per unit of end-to-end compute?

## RQ4 — Novelty Isolation

> Is the improvement specifically caused by the authentic Sanskrit structural organization, rather than by generic linguistic structure, executable rules, descriptive terminology, additional information, or greater trainable capacity?

The first three questions establish practical value. The fourth establishes novelty.

---

# 4. Experiment Overview

The first experiment consists of two linked tracks.

```text
Track 1 — Matched Token-Efficiency Audit

Track 2 — Structural Reasoning, Accuracy, and Novelty Isolation
```

Both tracks use semantically aligned material and shared evaluation domains, but they answer different causal questions.

- Track 1 measures the efficiency of language and tokenizer representation.
- Track 2 measures reasoning, accuracy, sample efficiency, and whether Sanskrit-specific structure creates the gain.

The experiment should deliberately exclude:

- persistent self-assimilation;
- fast-weight adaptation;
- model editing;
- base-weight rewriting;
- unrestricted continual pretraining;
- national-scale corpus construction;
- full Vedic, Chandas, kāvya, manuscript, or recitation modules;
- large-scale government deployment claims.

---

# Part I — Track 1: Matched Token-Efficiency Audit

# 5. Objective

Determine whether semantically equivalent Sanskrit content can be represented in substantially fewer tokens than English when both languages receive fair, matched tokenizers.

This track does not require training a full language model.

---

# 6. Parallel Evaluation Corpus

Construct a human-reviewed parallel corpus of approximately **5,000–10,000 aligned items**.

The corpus should cover at least:

| Domain | Representative content |
|---|---|
| General prose | Explanations, descriptions, narratives |
| Science | Physics, biology, computer science |
| Mathematics | Definitions, proofs, worked explanations |
| Algorithms | Procedures, complexity, data structures |
| Legal and government | Rules, formal statements, policies |
| Dialogue and instructions | Questions, answers, task instructions |
| Code explanation | Natural-language explanations of source code |

Every Sanskrit–English pair must express equivalent content. The sealed test set should be reviewed by:

- a Sanskrit specialist;
- a domain expert;
- an independent alignment reviewer for a sample of the data.

Machine translation alone is not acceptable for the final hidden evaluation set.

The corpus must label whether Sanskrit text is:

- attested;
- translated;
- expert-proposed;
- institution-standardized;
- model-generated.

Model-generated frequency must never be treated as independent attestation.

---

# 7. Tokenizer Conditions

Use the same tokenizer family and matched vocabulary budgets.

Recommended vocabulary sizes:

```text
8,000
16,000
32,000
```

## T-E — English-Native Statistical Tokenizer

Trained on the English side with the same tokenizer algorithm and vocabulary budget.

## T-S — Sanskrit-Native Statistical Tokenizer

Trained on the Sanskrit side with matched corpus size, domain distribution, normalization policy, and vocabulary budget.

## T-SS — Sanskrit Structural Tokenizer

A Sanskrit-native tokenizer informed by selected structural information, including:

- script and canonical phonological identity;
- Sandhi boundaries;
- lexical forms;
- recurrent inflectional units;
- selected derivational units;
- compound preservation or decomposition where justified.

The experiment should not measure Sanskrit primarily through an English-dominant commercial tokenizer. That would primarily measure tokenizer mismatch.

---

# 8. Track 1 Metrics

## 8.1 Sequence Compression

For every aligned item, calculate:

\[
\text{Compression Ratio}
=
\frac{\text{Sanskrit token count}}
{\text{English token count}}
\]

Report:

- mean;
- median;
- quartiles;
- per-domain distribution;
- results by document length;
- results by vocabulary size;
- Devanāgarī and transliteration variants where relevant.

## 8.2 Semantic Capacity

Measure:

- propositions per 1,000 tokens;
- concepts per 1,000 tokens;
- percentage of aligned passages fitting within fixed 4K, 8K, and 32K contexts;
- equivalent semantic content per fixed token window.

## 8.3 Engineering Proxies

Estimate, but do not overclaim:

- sequence-length reduction;
- KV-cache requirements;
- prompt-processing workload;
- effective content capacity within a fixed context window.

Token reduction should not be directly converted into guaranteed total-cost reduction. End-to-end compute is measured in Track 2.

---

# 9. Track 1 Success Thresholds

A promising result is:

> Median Sanskrit token consumption is at least **25% lower** than matched English across most tested domains.

A strong result is:

> A **35–50% reduction** that persists in modern scientific, algorithmic, legal, dialogue, and code-explanation material.

A result confined to classical poetry or highly compressed verse is insufficient for the intended architecture.

---

# Part II — Track 2: Structural Reasoning, Accuracy, and Novelty Isolation

# 10. Objective

Determine whether explicit Sanskrit structural information improves reasoning, answer accuracy, and sample efficiency over Sanskrit text alone—and whether the improvement is specifically attributable to Sanskrit’s authentic structural organization.

The experiment should use:

- one open multilingual base model;
- a frozen backbone in the first phase;
- matched adapter and encoder capacities;
- the same tasks, examples, and update information across all conditions.

---

# 11. Minimal Sanskrit Structural Stack

Do not implement the full Version 2 architecture in this first pilot.

Use the four structural mechanisms most likely to influence reasoning and scope.

## 11.1 Lexical Identity and Inflection

Represent:

- canonical form;
- lexeme or lemma;
- paradigm identity;
- nominal case, number, and gender;
- verbal person, number, tense or mood, and voice where relevant.

## 11.2 Derivational Structure

Represent:

- root or stem;
- prefix;
- derivational suffix;
- derivational class;
- candidate inherited meaning;
- alternative derivations where necessary.

## 11.3 Compound Structure

Represent:

- constituents;
- nested hierarchy;
- head and modifier relations;
- candidate semantic relation;
- vigraha where available;
- lexicalization and inheritance-blocking flags.

## 11.4 Kāraka and Event-Role Structure

Represent:

- predicate or process;
- agent;
- affected entity;
- instrument;
- source;
- recipient;
- location;
- other task-relevant roles.

Basic script normalization and Sandhi analysis may be used to identify expressions, but the first pilot should not depend on the full discourse, rule-scope, Vedic, prosodic, or plastic-memory architecture.

---

# 12. Base Model and Trainable Components

Choose an open multilingual decoder model in approximately the **1–3 billion parameter range** with:

- acceptable Devanāgarī handling;
- reproducible local inference;
- research-compatible licensing;
- accessible hidden states or adapter interfaces;
- sufficient baseline Sanskrit competence.

Freeze all principal model weights.

Train only capacity-matched components such as:

- structural encoder;
- retrieval head;
- fusion or cross-attention adapter;
- confidence head;
- optional update-scope predictor.

All structural conditions must receive the same:

- trainable-parameter budget;
- encoder depth and width;
- training steps;
- optimization policy;
- retrieval budget;
- context-token budget;
- compute ceiling.

The experiment tests the representation, not which condition received more engineering capacity.

---

# 13. Experimental Conditions

| ID | Condition | Purpose |
|---|---|---|
| **E0** | English text-only | Strong conventional reference |
| **S0** | Sanskrit text-only | Isolate Sanskrit language and tokenizer effects |
| **S1** | Sanskrit plus serialized structure | Test whether additional structural information helps when supplied as text |
| **S2** | Sanskrit plus off-sequence structural side channel | Target architecture |
| **U1** | Sanskrit plus universal linguistic structure | Test explicit linguistic structure generally |
| **X1** | Sanskrit plus generic executable grammar | Test rules, inheritance, scope, and exceptions generally |
| **CE1** | Controlled descriptive English plus matched structure | Test descriptive terminology as the explanation |
| **N1** | Learned neural latent structure | Test whether scholar-defined structure is necessary |
| **S-A** | Sanskrit structure with anonymized relations | Test topology versus traditional labels |
| **S-R** | Randomly rewired Sanskrit structure | Test whether authentic organization matters |
| **S-E** | Sanskrit structure without exception/scope relations | Test the value of inheritance boundaries |
| **S-P** | Automatically predicted Sanskrit structure | Test practical feasibility |

The decisive competitors are not text and vector memory alone. They are:

```text
S2 Sanskrit structural side channel
versus
U1 universal linguistic structure
versus
X1 generic executable grammar
versus
CE1 controlled descriptive English
versus
N1 learned neural structure
```

---

# 14. Canonical Information-Equivalence Record

Before constructing any language-specific representation, create a language-independent canonical record.

```text
Concept ID
Definition
Concept type
Inputs and outputs
Agent and affected entity
Instrument, source, destination, location
Cause and result
Related and confusable concepts
Domain and temporal scope
Evidence
Positive inheritance relations
Protected exceptions
```

Store evaluation-only information in a physically separate, access-controlled record:

```text
Evaluator-only item ID
Gold answers
Gold update consequences
Expected proof properties
Expected inherited and blocked sets
Correct analysis labels
Scoring and adjudication fields
```

Every experimental condition receives the same lawful facts and task-relevant relations. No condition compiler, structural payload, training artifact, retrieval index, model input, or cache may contain or derive a gold answer, gold update consequence, proof, expected block, correct-analysis label, or scoring key. Hash the canonical source record and evaluator oracle separately and log access to the latter.

The Sanskrit condition must not receive richer knowledge merely because scholars provided more detailed annotation.

An independent baseline team should design or audit U1, X1, CE1, and N1. That team should be encouraged to produce the strongest possible alternatives rather than confirm the Sanskrit hypothesis.

---

# 15. Evaluation Worlds

Use three distinct evaluation worlds.

## W1 — Clean-Room Fictional Concepts

Create fictional concepts that cannot exist in the base model’s pretraining data.

Recommended pilot scale:

- 100–150 concept families;
- 8–15 related expressions per family;
- explicit positive and negative inheritance relations;
- controlled exceptions and misleading structural alternatives.

This world is the cleanest test of sample efficiency and structural generalization.

## W2 — Reviewed Modern Technical Concepts

Use approximately 50–100 concepts from tightly bounded domains such as:

- elementary algorithms;
- linear algebra;
- mechanics;
- computer networks;
- formal logic;
- introductory electronics.

Each concept should include:

- canonical definition;
- reviewed Sanskrit expression or alternatives;
- structural analysis;
- equation, algorithm, code, or formal relation where applicable;
- neighbouring and confusable concepts;
- domain and evidence;
- gold answers.

## W3 — Attested Natural Sanskrit

Use approximately 100 natural families containing:

- real inflectional variation;
- derivational relations;
- compounds;
- polysemy;
- lexicalized meanings;
- context-sensitive interpretation;
- protected exceptions.

This world tests whether gains survive beyond engineered terminology.

---

# 16. Task Families

## Task A — Novel Expression Understanding

Test unseen:

- inflectional forms;
- derivational combinations;
- compounds;
- structurally related technical expressions.

Measure whether the model identifies and applies the intended concept without merely recalling the exact form.

## Task B — Low-Shot Concept Acquisition

Introduce concepts using:

```text
1 example
2 examples
4 examples
8 examples
16 examples
```

Then test:

- definition;
- paraphrase recognition;
- discrimination from nearby concepts;
- novel application;
- related unseen expression;
- rejection of unsupported structural inference.

## Task C — Event and Paraphrase Reasoning

Express the same event using:

- different word order;
- active and passive voice;
- nominalization;
- omitted participant;
- different case realization;
- Sanskrit and English paraphrases.

Measure whether the model recognizes the shared event and answers correctly.

## Task D — General Reasoning

Include tasks that cannot be solved through morphology alone:

- arithmetic word problems;
- logical inference;
- causal reasoning;
- sequence and rule application;
- elementary scientific reasoning;
- algorithmic reasoning.

This prevents improved linguistic analysis from being mislabeled as improved general reasoning.

---

# 17. Accuracy and Reasoning Metrics

Reasoning quality should be judged primarily through outcomes.

Measure:

- exact answer accuracy;
- numerical correctness;
- executable correctness;
- unit-test pass rate;
- consistency across paraphrases;
- novel-composition accuracy;
- application accuracy;
- calibration under ambiguity;
- refusal or abstention quality when evidence is insufficient.

For mathematics, code, and algorithms, use deterministic verification wherever possible.

A fluent structural explanation is not evidence of correct reasoning.

---

# 18. Efficiency Metrics

## 18.1 Raw Token Consumption

Report input, retrieved-context, and output tokens separately.

## 18.2 Accuracy at Fixed Token Budget

Examples:

```text
Input budget: 1,024 tokens
Output budget: 256 tokens
```

Measure how many items each condition solves correctly within the same budget.

## 18.3 Correct Answers per Token

\[
\text{Token-Normalized Performance}
=
\frac{\text{Correct Answers}}
{\text{Total Input + Retrieved + Output Tokens}}
\]

This metric must always be reported with raw accuracy.

## 18.4 Correct Answers per Unit Compute

Measure:

- GPU time;
- wall-clock latency;
- prompt-processing time;
- structural-analysis overhead;
- graph-encoder overhead;
- memory use;
- retrieval operations;
- tokens generated per second.

Report accuracy at a fixed compute budget and, where useful, correct answers per GPU-minute.

## 18.5 Sample Efficiency

Plot accuracy against concept exposures and report:

- area under the learning curve;
- examples needed to reach a target accuracy;
- relative exposure reduction versus S0, U1, X1, and CE1.

---

# 19. Primary Presentation: Accuracy–Token–Compute Frontier

The central presentation should be a Pareto frontier.

```text
x-axis: total tokens or end-to-end inference compute

y-axis: answer accuracy
```

The target Sanskrit structural system is compelling when it provides:

- higher accuracy at the same token or compute budget;
- the same accuracy using fewer tokens or less compute;
- or both.

Illustrative result only:

| Condition | Accuracy | Tokens per item | Relative compute |
|---|---:|---:|---:|
| English text | 76% | 1,100 | 1.00× |
| Sanskrit text | 69% | 700 | 0.78× |
| Universal structure | 76% | 720 | 0.90× |
| Generic executable grammar | 77% | 730 | 0.92× |
| Sanskrit structural side channel | **82%** | **690** | **0.91×** |

The table above is not a forecast. It demonstrates the kind of evidence required.

---

# 20. Novelty Controls

## 20.1 Controlled Descriptive English

Use English expressions designed to expose the same semantic components as the Sanskrit term.

If CE1 matches S2, the result may show that descriptive terminology helps, not that Sanskrit’s structural organization is uniquely beneficial.

## 20.2 Universal Linguistic Structure

Translate the same information into language-neutral features such as:

```text
lemma
inflection
process
agent
patient
instrument
head
modifier
domain
exception
```

If U1 matches S2, the result supports explicit linguistic structure generally.

## 20.3 Generic Executable Grammar

Provide equivalent mechanisms for:

- default;
- inheritance;
- exception;
- scope;
- precedence;
- optionality.

If X1 matches S2, procedural structure is the likely cause.

## 20.4 Anonymized Sanskrit Relations

Replace Sanskrit relation names with arbitrary IDs while preserving structure.

This tests whether the topology matters more than the traditional labels.

## 20.5 Shuffled Sanskrit Structure

Preserve graph size, relation frequency, and degree statistics while rewiring the authentic relations.

If S-R performs similarly to S2, authentic Sanskrit organization is not driving the gain.

## 20.6 Remove Exceptions and Scope

S-E should normally propagate more aggressively and commit more locality errors.

If removing exception and scope relations has no measurable effect, those mechanisms are likely decorative.

## 20.7 Oracle versus Predicted Structure

Compare:

- scholar-validated oracle structure;
- rule-generated structure;
- neural-predicted structure;
- ensemble structure;
- deliberately noisy structure.

Possible interpretations:

| Outcome | Interpretation |
|---|---|
| Oracle and predicted both win | Strong mechanism and feasible tooling |
| Oracle wins, predicted fails | Representation may help; tools are inadequate |
| Neither wins | Structural architecture is not adding sufficient value |
| Predicted wins only on linguistic tasks | Useful Sanskrit NLP, not yet stronger reasoning |

---

# 21. Co-Primary Success Criteria

The experiment should pre-register two co-primary endpoints.

## Endpoint 1 — Accuracy–Efficiency

The target condition S2 must achieve at least one of:

- **5 percentage points higher accuracy** at the same token budget;
- equivalent accuracy using **20% fewer total tokens**;
- equivalent accuracy using **20% less end-to-end compute**;
- the same target accuracy with **20% fewer learning examples**.

It should also:

- improve at least three of the four task families;
- avoid losing more than two points on general reasoning;
- preserve gains in modern technical content.

## Endpoint 2 — Mechanism Novelty

S2 must also:

- outperform the strongest of U1, X1, CE1, and N1 by a meaningful pre-registered margin;
- lose a substantial portion of its advantage under shuffled or corrupted structure;
- show that exception removal harms locality;
- retain at least half of the oracle improvement under predicted or ensemble structure;
- demonstrate causal dependence through structural interventions;
- reproduce on a second model backbone and at least two evaluation worlds.

Passing only Endpoint 1 establishes practical utility.

Passing both endpoints establishes a credible novelty signal.

---

# 22. Novelty Outcome Matrix

| Result | Defensible interpretation |
|---|---|
| S2 beats S0 | Explicit structure improves Sanskrit modelling |
| S2 beats text and vector memory | Structured representation helps |
| S2 matches U1 | Linguistic structure helps; Sanskrit-specific novelty is unproven |
| S2 matches X1 | Executable rules explain the gain |
| S2 matches CE1 | Descriptive composition explains the gain |
| S2 beats U1, X1, CE1, and N1 | Strong Sanskrit-structural novelty signal |
| S2 wins and S-R collapses | Authentic structural organization is causal |
| Oracle wins but predicted fails | Novel representation, immature tooling |
| S2 wins across two backbones | Reusable architectural mechanism |
| S2 wins only on engineered terms | Likely terminology-engineering or benchmark effect |
| S2 wins across fictional, technical, and attested worlds | Strong generalization evidence |

---

# 23. Causal-Use Tests

A displayed structural trace is not proof that the model used the structure.

For successful examples:

1. remove the structural side channel;
2. replace it with the shuffled structure;
3. corrupt one derivational or event relation;
4. add a false exception;
5. remove a valid exception;
6. exchange event roles;
7. patch a graph from another concept family;
8. measure changes in answer, confidence, retrieval, and latency.

The output should change predictably.

If the answer remains unchanged, the model may be ignoring the structure and relying on text or parametric memory.

---

# 24. Practical Go, Pivot, and Stop Rules

## Go

Proceed to a larger integrated experiment when:

- both co-primary endpoints pass;
- the gain appears in at least two evaluation worlds;
- confidence intervals exclude zero;
- results survive at least five random seeds;
- predicted or ensemble structure retains at least half the oracle gain;
- end-to-end cost remains proportionate to the benefit;
- a second backbone reproduces the principal effect;
- an independent group or internal red team reproduces the main result.

## Pivot

Narrow or redirect the claim when:

- Sanskrit beats text/vector but matches U1;
- Sanskrit matches X1;
- controlled English matches Sanskrit;
- only oracle structure succeeds;
- gains are confined to invented technical terminology.

Possible pivot:

> Structured continual-learning and efficient Sanskrit AI inspired by Sanskrit, without claiming a unique Sanskrit computational substrate.

## Stop the Architectural Claim

Stop or substantially narrow the architecture claim when:

- shuffled structure performs similarly to authentic Sanskrit structure;
- the canonical concept graph alone performs nearly as well;
- natural Sanskrit fails to reproduce controlled gains;
- general reasoning degrades materially;
- locality deteriorates;
- causal interventions show that the model ignores the structure;
- end-to-end cost overwhelms the practical benefit.

Negative results should still be released.

---

# 25. Six-Month Execution Plan

| Month | Work |
|---|---|
| **1** | Freeze hypotheses, canonical schema, conditions, metrics, budgets, and pre-registration |
| **2** | Build parallel token corpus and clean-room fictional concept families |
| **3** | Add reviewed technical and attested Sanskrit subsets; complete adjudication |
| **4** | Implement tokenizers, model conditions, structural side channel, and negative controls |
| **5** | Run development pilot, resolve protocol-defined implementation defects, then seal the final test |
| **6** | Run hidden evaluation, causal interventions, cost analysis, second-backbone confirmation where feasible, and publish the decision report |

Suggested focused team:

- one ML research lead;
- two NLP or graph engineers;
- one data engineer;
- two Sanskrit computational linguists or scholars;
- one independent baseline researcher;
- one part-time statistician and evaluation lead.

The baseline researcher should be explicitly tasked with making U1, X1, CE1, and N1 as competitive as possible.

---

# 26. Required Deliverables

The first grant or pilot should produce:

1. a formal non-duplication and prior-art boundary report;
2. a fair Sanskrit–English parallel token-efficiency benchmark;
3. matched English and Sanskrit tokenizers;
4. a hidden reasoning and compositional-generalization benchmark;
5. canonical information-equivalence records;
6. Sanskrit, universal, procedural, controlled-English, learned, anonymized, shuffled, and exception-removed representations;
7. oracle, predicted, ensemble, and noisy structural pipelines;
8. a frozen-model structural side-channel implementation;
9. accuracy–token–compute Pareto results;
10. low-shot sample-efficiency results;
11. causal-intervention results;
12. end-to-end compute, latency, storage, and token accounting;
13. open code, data, schemas, adapters, and evaluation harnesses;
14. a scale, pivot, or stop decision report;
15. negative and inconclusive findings.

---

# 27. Fundable Novelty Statement

Before results, the proposal may state:

> **The programme will test whether a compact Sanskrit-native representation combined with an off-sequence executable Sanskrit Structural Stack produces a superior accuracy–token–compute trade-off, and whether that advantage derives specifically from Sanskrit’s cross-layer organization, inheritance, and exception structure rather than from tokenization, additional annotations, descriptive terminology, or structured memory generally.**

After a strong positive result, the programme may state:

> **We demonstrate that a Sanskrit-derived multilayer structural representation improves reasoning accuracy and sample efficiency at lower token consumption than information-equivalent universal linguistic, generic procedural, controlled-English, learned-neural, and unstructured baselines, with causal ablations confirming that the authentic structural organization drives the gain.**

The second statement is not available until the experiment supports it.

---

# 28. What This First Experiment Can Establish

A successful first pilot can establish that:

- fair Sanskrit-native tokenization reduces sequence length;
- selected structural features improve reasoning or accuracy over Sanskrit text alone;
- the combined system improves correct answers per token or per unit compute;
- the improvement survives strong generic alternatives;
- authentic Sanskrit structural organization causally contributes to the result;
- practical automatic structural analysis preserves enough of the oracle benefit to justify further investment.

---

# 29. What This First Experiment Cannot Establish

Even a strong result will not yet prove:

- safe self-assimilation;
- lifelong learning;
- precise base-weight editing;
- legal, scientific, or government reliability;
- universal Sanskrit superiority;
- a fixed 50% compute reduction;
- national-scale readiness;
- that the model literally thinks in Sanskrit;
- that external evidence is unnecessary.

Those claims require separate later experiments.

---

# 30. Decision Rule

The project should seek substantial follow-on funding only when it can show both:

```text
PRACTICAL VALUE

higher accuracy, lower tokens, lower compute,
or stronger sample efficiency
```

and:

```text
MECHANISM NOVELTY

the authentic Sanskrit structural organization
outperforms strong information-equivalent alternatives
and loses its advantage under causal ablation
```

The first three practical questions establish that the system is useful.

The novelty-isolation question establishes that the programme is not merely recreating an efficient tokenizer, descriptive terminology system, generic graph, or structured-memory architecture under a Sanskrit label.

---

# 31. One-Sentence Experimental Definition

> **Use the same frozen model, information, tasks, trainable capacity, token budget, and compute budget across matched English, Sanskrit, universal-linguistic, generic-procedural, controlled-English, learned-neural, and ablated Sanskrit conditions; then measure whether the authentic Sanskrit Structural Stack produces more correct answers per token and compute, and whether that gain disappears when its true organization, inheritance, or exception structure is removed.**

---

# Companion Documents

This pilot should be read with:

1. `Shastriya_Bhasha_Foundation_Model_Concise_Proposal_v2.md`
2. `Sanskrit_Structural_Self_Assimilating_Model_v2.md`
3. `Sanskrit_Structural_Self_Assimilating_Model_V2_Research_Architecture_and_Protocol.md`
4. `Paninian_Grounded_Foundation_Model_Strategy.md`
5. `Paninian_Self_Assimilating_Model_Gap_Analysis_Refactored_v2.md`
6. `06_Sanskrit_Derived_Efficient_LLM_Research_Question_Register_and_Decision_Tree.md`
7. `07_Mission_and_Falsification_Contract.md`
8. `08_DQ1_Mechanism_Resolution_M0_M1_Contract.md`

Where they conflict, Documents 06 and 07 govern route and mission, and the Frozen version of Document 08 governs the rule-scope mechanism boundary.

---

# Revision Note

| Version | Date | Change | Status |
|---|---|---|---|
| 1.0 | August 2026 | Initial pilot design | Superseded by 1.1 |
| 1.1 | 21 August 2026 | Added the DQ1 execution hold and the integrate-or-narrow requirement for exception/scope claims | Design source; not executable |
