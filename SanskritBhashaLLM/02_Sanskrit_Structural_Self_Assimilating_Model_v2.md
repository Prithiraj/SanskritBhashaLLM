# Sanskrit Structural Self-Assimilating Foundation Model
## Version 2: A Multilayer Architecture for Internal Interpretation, External Grounding, and Controlled Knowledge Assimilation
### With a Pāṇinian Grammatical Core

**Document version:** 2.0  
**Status:** Authoritative conceptual and architectural paper  
**Date:** August 2026  
**Intended setting:** Institution-led, publicly funded, open-weight and open-research programme  
**Companion document:** `Sanskrit_Structural_Self_Assimilating_Model_V2_Research_Architecture_and_Protocol.md`

---

# Executive Idea

Most large language models obtain additional context through retrieval, search engines, databases, tools, or documents. In a conventional retrieval-augmented system, the retrieved material is placed into the current context, influences one answer, and then largely disappears. The model may use the material, but it does not necessarily interpret it through an explicit internal structure, preserve the resulting knowledge as a governed memory transaction, or determine precisely which related expressions and concepts should inherit the update.

The Sanskrit Structural Self-Assimilating Foundation Model proposes a different knowledge cycle.

The model first examines an input through an explicit, multilayer Sanskrit structural system. This system includes script and phonological identity, Sandhi and segmentation, lexical identity and inflection, derivational processes, compound structure, kāraka and event roles, sentence constraints, discourse links, lexical sense, register, domain, period, and rule scope. These layers jointly generate candidate interpretations, expose ambiguity, identify missing relations, and suggest where internal knowledge should be retrieved.

The model then aligns those candidates to a **language-independent canonical concept layer**. If the structural analysis is insufficient, uncertain, contradicted, empirically unsupported, or temporally unstable, it retrieves external evidence. External material is not merely appended to a prompt. It is preserved, decomposed into claims, aligned to concepts, compared with structural interpretations, assigned provenance, checked for contradiction, and converted into a reversible update proposal.

The model therefore operates through a knowledge metabolism:

```text
observe an expression or claim
        ↓
generate structural interpretations
        ↓
identify concepts and knowledge gaps
        ↓
retrieve external evidence where necessary
        ↓
reconcile structure, usage, context, and evidence
        ↓
predict where the knowledge should propagate
        ↓
protect exceptions and unrelated senses
        ↓
commit, quarantine, fork, supersede, or reject
        ↓
retain provenance and rollback
```

The core design principle is:

> **Sanskrit's structural system proposes and constrains interpretations. Canonical concepts remain independent of language. External evidence grounds or corrects the interpretation. Reversible institutional memory assimilates the result. Controlled model plasticity follows only after the structural mechanism has been validated.**

This is not simply:

- a Sanskrit chatbot;
- a Pāṇinian parser placed before an LLM;
- a morphology-aware tokenizer;
- ordinary retrieval-augmented generation;
- a generic knowledge graph;
- unrestricted self-modification;
- or a claim that linguistic elegance establishes empirical truth.

It is a proposal for an **open, institutionally governed, neuro-symbolic foundation-model architecture** in which a formal natural-language structure is tested as a causal mechanism for interpretation, retrieval, knowledge propagation, exception handling, and update locality.

---

# Document Role and Version Relationship

This paper is the conceptual and architectural successor to `Paninian_Self_Assimilating_Model.md`.

The earlier paper remains valuable as the point at which the central insight emerged:

```text
internal structure proposes
external evidence grounds or corrects
controlled memory reconciles
institutional governance consolidates
```

However, that paper organized the internal memory too heavily around dhātus and derivational families. Version 2 replaces that centre with a **multi-index Sanskrit structural stack**. Dhātus remain important, but they are one address among surface forms, phonological forms, paradigms, derivations, compounds, event roles, senses, discourse referents, concepts, and evidence records.

The document family now has distinct responsibilities:

| Document | Role |
|---|---|
| `Paninian_Self_Assimilating_Model.md` | Version 1 conceptual precursor and brainstorming record |
| `Paninian_Self_Assimilating_Model_Gap_Analysis_Refactored_v2.md` | Design review explaining why Version 1 required reconstruction |
| `Sanskrit_Structural_Self_Assimilating_Model_v2.md` | Authoritative Version 2 conceptual and architectural paper |
| `Sanskrit_Structural_Self_Assimilating_Model_V2_Research_Architecture_and_Protocol.md` | Controlled experimental protocol that tests the architecture |

This paper explains **what the model is, why it is structured this way, and what an institution would build**. The companion protocol specifies the detailed hypotheses, baselines, holdouts, metrics, statistics, stage gates, and stopping conditions.

---

# Part I — Foundations

# 1. From Context Augmentation to Knowledge Assimilation

## 1.1 The limitation of temporary context

A conventional LLM has at least two broad sources of knowledge:

1. **Parametric knowledge** encoded in model weights during training.
2. **Temporary context** supplied through prompts, retrieval, tools, or user messages.

Parametric knowledge is difficult to inspect, update, scope, and reverse. Temporary context is easy to provide, but it normally expires after the interaction and may not become a durable, structured memory.

A retrieved passage can answer a question without solving several deeper problems:

- What concept does the passage describe?
- Which linguistic expression or sense does it correspond to?
- Which parts of the passage are claims, examples, definitions, hypotheses, or instructions?
- Which source supports each claim?
- Does the new claim contradict existing evidence?
- Is the claim current, historical, local, domain-specific, or universal?
- Which related forms and concepts should inherit the update?
- Which homonyms, idioms, lexicalized forms, domains, or historical senses must remain unchanged?
- Can the update be reversed without destroying later dependent changes?

The proposed architecture treats these questions as part of the model rather than as optional metadata surrounding retrieval.

## 1.2 Assimilation rather than ingestion

The model does not equate reading with learning. External material passes through a structured process:

```text
source
→ preserved original
→ source-faithful semantic representation
→ canonical concept alignment
→ Sanskrit structural alignment
→ evidence assessment
→ conflict and scope analysis
→ reversible memory transaction
```

An external statement can therefore produce several outcomes:

- **Confirm** an existing interpretation.
- **Refine** it with greater precision.
- **Extend** it into a new relation or domain.
- **Override** a literal or default interpretation.
- **Fork** a separate sense, period, school, or domain.
- **Merge** duplicate concept records after review.
- **Supersede** an older claim while retaining its history.
- **Expire** a time-bounded claim.
- **Quarantine** an unresolved or unreliable claim.
- **Reject** material that is false, poisoned, irrelevant, or structurally incompatible.
- **Abstain** when the model cannot resolve the conflict safely.

Assimilation is therefore not a single weight update. It is a governed knowledge transaction.

## 1.3 The inward and outward loop

The system uses two complementary directions.

### Inward structural interpretation

The model asks:

- Which surface and phonological identity is present?
- Which Sandhi analyses and word boundaries remain possible?
- Which lexemes, inflections, and derivational histories are compatible?
- Is the expression a compound, and what are its possible internal relations?
- Which participants fill which event roles?
- Which sentence and discourse interpretations remain plausible?
- Which lexical sense, register, domain, and period apply?
- Which defaults, inherited contexts, exceptions, or precedence rules govern the interpretation?
- Which canonical concepts and prior evidence are structurally reachable?
- What information is still missing?

### Outward evidential grounding

The model asks:

- Does the asserted referent exist in the real world?
- How is it defined in the relevant domain?
- Which observations, measurements, equations, code, documents, or authorities support it?
- Is the information current?
- Does attested usage diverge from the literal structure?
- Do sources disagree?
- Is the evidence independent, reliable, and applicable to this domain, time, or jurisdiction?
- Should the internal interpretation be confirmed, narrowed, overridden, or rejected?

Neither direction is sufficient alone.

---

# 2. Why Sanskrit's Full Structural System Matters

## 2.1 The opportunity is not morphology alone

Sanskrit is often described as morphologically rich. That description is true but incomplete for this project. Other languages also have inflection, derivation, compounds, or flexible word order.

The computational opportunity lies in the **combination of multiple explicit structures with a highly developed procedural and analytical tradition**. Sanskrit offers not only texts but formal accounts of how many forms are generated, transformed, related, constrained, interpreted, inherited, and excepted.

The model therefore treats Sanskrit as a structural stack rather than as a collection of roots or a surface language for generation.

## 2.2 The Sanskrit structural stack

```text
script and source identity
        ↓
phonological representation and sound classes
        ↓
Sandhi transformations and segmentation alternatives
        ↓
lexical identity and inflectional paradigms
        ↓
derivational processes and intermediate states
        ↓
nested compound structure and vigraha candidates
        ↓
kāraka and predicate-centred event relations
        ↓
sentence constraints and missing-role expectations
        ↓
discourse, coreference, and exposition relations
        ↓
lexicalized sense, register, domain, and period
        ↓
rule scope, inheritance, defaults, exceptions, and precedence
        ↓
canonical concepts and externally warranted evidence
```

These layers are not a rigid one-way pipeline. Later information can revise earlier analyses. A sentence interpretation may reject a locally valid segmentation. A domain-specific lexical sense may override a literal derivation. External evidence may show that a grammatically elegant compound refers to nothing real.

## 2.3 Cross-layer constraint intersection

The model preserves several candidate interpretations and evaluates them under multiple constraints.

A candidate may be:

- phonologically possible;
- morphologically valid;
- derivationally plausible;
- and still be rejected because its compound relation is wrong, its event roles are incompatible, its lexical sense is unattested, its discourse referent is incorrect, or external evidence contradicts it.

Conversely, an expression may have an irregular or weak derivation while its conventional technical meaning is strongly attested and empirically supported.

The model's interpretation is therefore based on **constraint intersection**, not on one privileged root analysis.

Conceptually:

\[
P(I\mid X) = F(
C_{surface},
C_{phonology},
C_{sandhi},
C_{inflection},
C_{derivation},
C_{compound},
C_{event},
C_{sentence},
C_{discourse},
C_{sense},
C_{register},
C_{rule},
C_{evidence}
)
\]

This equation is a conceptual dependency statement, not a commitment to multiply independent probabilities. The actual combination must be learned and calibrated empirically.

## 2.4 What Sanskrit structure can provide

The structural stack can potentially provide:

- multiple explicit routes from surface variation to lexical identity;
- reusable paradigmatic and derivational relationships;
- hierarchical compound analysis;
- predicate-centred event representations that are less dependent on word order;
- explicit expectations for missing arguments or relations;
- rule-governed inheritance and protected exceptions;
- structured ambiguity rather than forced premature choices;
- inspectable derivation and update paths;
- better retrieval across related forms;
- more precise prediction of where knowledge should propagate;
- a natural setting for testing neuro-symbolic learning.

## 2.5 What Sanskrit structure cannot provide

The structural stack cannot by itself establish:

- empirical truth;
- current events;
- measurements;
- scientific mechanisms;
- historical facts;
- legal validity;
- causal claims;
- code behaviour;
- or the existence of a proposed referent.

A transparent expression can provide an **intensional prior**: a provisional indication of what a term could mean. It cannot provide complete **referential grounding**.

The architecture therefore keeps four things distinct:

```text
formation
≠
intended meaning
≠
canonical concept
≠
empirically warranted claim
```

That separation is an architectural invariant, not a rhetorical caution.

---

# 3. Scope and Intellectual Attribution

## 3.1 Why the project is called Sanskrit Structural

The complete architecture draws on more than the Aṣṭādhyāyī. Calling every layer directly “Pāṇinian” would be historically and technically imprecise.

The working designation is therefore:

> **Sanskrit Structural Self-Assimilating Foundation Model, with a Pāṇinian grammatical core.**

## 3.2 Layered attribution

| Structural layer | Primary intellectual or technical source |
|---|---|
| Morphology, derivation, compounds, kāraka, rule organization | Pāṇinian grammatical core |
| Phonology, sound classes, accent, recitational features | Śikṣā- and Prātiśākhya-informed traditions |
| Word sense, etymological proposals, attestation, conventional meaning | Nirukta and lexicographic traditions |
| Sentence expectancy, compatibility, connectedness, intended purport | Śābdabodha and verbal-cognition traditions |
| Structured exposition, objection, response, example, and conclusion | Tantrayukti and discourse traditions |
| Meter and prosodic constraints | Chandas traditions |
| Scientific concepts, formal definitions, code, measurements, current evidence | Modern domain and evidence governance |

These categories provide a responsible attribution model. They do not imply that every historical concept has already been converted into a precise computational formalism.

## 3.3 Initial Structural Stack v1 coverage

Within this Version 2 paper, **Structural Stack v1** means the first implementable coverage contract, not the document version. It focuses on Classical and contemporary prose and includes:

- Unicode and transliteration normalization;
- canonical phonological representation;
- selected varṇa and sound-class features;
- bidirectional Sandhi and segmentation candidates;
- benchmark-relevant subanta and tiṅanta features;
- kṛt, taddhita, selected sanādi, and other pilot-relevant derivations;
- nested samāsa structure, vigraha candidates, and lexicalization flags;
- vibhakti-to-kāraka and event-role mapping;
- selected sentence constraints, especially argument expectancy and compatibility;
- coreference and limited discourse relations;
- lexical sense IDs;
- domain, register, period, genre, and attestation status;
- pilot-relevant defaults, inherited scope, exceptions, precedence, and optionality;
- language-independent canonical concepts;
- evidence and provenance records;
- multi-index retrieval;
- reversible memory transactions.

## 3.4 Explicitly deferred modules

The first version does not claim complete coverage of:

- Vedic accent and morphology;
- recensional and oral-text variation;
- full Chandas;
- kāvya and alaṅkāra;
- complete śāstric discourse across traditions;
- manuscript restoration;
- multimodal recitation;
- unrestricted self-modifying weights;
- national-scale corpus or model training.

The architecture reserves extension points for these modules, but each requires specialist data, governance, evaluation, and independent validation.

## 3.5 Non-goals

The project does not assume that:

- every Sanskrit expression is compositionally transparent;
- morphology provides complete semantics;
- Sanskrit replaces external evidence;
- the model literally “thinks” in Sanskrit;
- a structural explanation is automatically causal;
- Sanskrit is best for every kind of knowledge;
- token or inference cost falls by a fixed percentage;
- explicit structure eliminates hallucination;
- one institution should replace existing Sanskrit tools or research groups.

---

# 4. Core Architectural Principles

The following principles govern every implementation.

## 4.1 Concept independence

Canonical concepts exist independently of Sanskrit labels, derivations, or compounds. A concept may be represented even when no adequate Sanskrit term exists.

## 4.2 Evidence separation

Structural plausibility and empirical warrant remain separate. A high-confidence derivation cannot compensate for weak evidence.

## 4.3 Alternative preservation

Ambiguous Sandhi splits, derivations, compound relations, lexical senses, discourse references, or scholarly interpretations remain live until context, evidence, or review justifies commitment.

## 4.4 Typed provenance

Every structural analysis, concept alignment, evidence claim, and update records its source, tool, version, confidence, licence, reviewer history, and supersession state.

## 4.5 Reversible updates

Every persistent update has an explicit scope, dependency set, evidence basis, version, rollback plan, and audit record.

## 4.6 Exception protection

Lexicalized, idiomatic, domain-specific, historical, metaphorical, school-specific, and competing senses can block or redirect inheritance.

## 4.7 Causal observability

A displayed structural trace is not accepted as an explanation merely because it is plausible. Interventions must show that the trace affects retrieval, confidence, output, or update scope.

## 4.8 External override

External evidence may reject a structural interpretation, establish an atomic concept, or preserve a conventional term whose derivation is weak or disputed.

## 4.9 Controlled plasticity

Structural retrieval and writable memory are validated before temporary adapters. Permanent weight consolidation is the final stage.

## 4.10 Open reproducibility

Schemas, adapters, model configurations, evaluation harnesses, non-sensitive datasets, provenance policies, and release decisions are documented under explicit licences.

---

# Part II — Model Architecture

# 5. High-Level Architecture

```text
INPUT + SOURCE PROVENANCE
        │
        ▼
SCRIPT / NORMALIZATION / PHONOLOGY
        │
        ▼
PROBABILISTIC SANDHI + SEGMENTATION LATTICE
        │
        ▼
LEXICAL IDENTITY + INFLECTIONAL PARADIGMS
        │
        ▼
DERIVATIONAL PROCESS GRAPH
        │
        ▼
NESTED COMPOUND HYPERGRAPH
        │
        ▼
KĀRAKA / EVENT-ROLE GRAPH
        │
        ▼
SENTENCE-CONSTRAINT + DISCOURSE GRAPH
        │
        ▼
LEXICAL SENSE + REGISTER + DOMAIN + PERIOD
        │
        ├─────────────────────┐
        ▼                     ▼
RULE-SCOPE ENGINE      CANONICAL CONCEPT GRAPH
        │                     │
        └─────────────── EVIDENCE / PROVENANCE GRAPH
                              │
                              ▼
                   CROSS-LAYER RECONCILIATION
                              │
                              ▼
                   MULTI-INDEX STRUCTURAL MEMORY
                              │
                              ▼
                    RETRIEVAL + RESPONSE ROUTER
                              │
                              ▼
                  REVERSIBLE UPDATE TRANSACTION
                              │
                              ▼
             ANSWER + STRUCTURAL / CONCEPT / EVIDENCE TRACE
```

This is a logical architecture, not a requirement that every layer use the same storage technology. Different layers may use:

- finite-state or neural transducers;
- typed process graphs;
- hypergraphs;
- predicate-centred event graphs;
- discourse relation graphs;
- versioned property graphs;
- vector indexes;
- neural encoders;
- rule objects;
- relational stores;
- or hybrid combinations.

The public interchange representation must abstract over those implementation choices.

## 5.1 Compact token stream and structural side channel

A Sanskrit-native tokenizer creates a real design tension. Treating a frequent compound as one compact token may reduce sequence length but hide its internal structure. Splitting every form into many morphological units may expose structure but increase token consumption.

Version 2 avoids forcing one representation to serve both goals:

```text
compact sequential token stream
+
off-sequence structural lattice
```

The token stream supports efficient contextual modelling. The structural side channel preserves Sandhi, paradigm, derivation, compound, event, sense, and rule information. The model may fuse them through cross-attention, gated adapters, graph encoders, or other controlled mechanisms.

This design allows token-efficiency and compositional-transparency hypotheses to be tested independently. A reduction in token count is not accepted as proof of better reasoning, and a more detailed structural graph is not allowed an uncounted compute budget.

## 5.2 Backbone and fusion strategy

The architecture supports two complementary model paths:

1. **Research-native model:** a relatively small Sanskrit-primary model trained with the structural stack to establish causality under controlled conditions.
2. **Capability model:** a strong open multilingual or Indian foundation-model backbone connected to the same structural memory, retrieval, and concept/evidence layers.

In the first controlled pilot, the language-model backbone remains frozen while the structural encoders and retrieval interface are tested. Joint training is introduced only after external structural retrieval demonstrates measurable value.

---

# 6. The Multilayer Sanskrit Structural Stack

## 6.1 Input and Source-Provenance Layer

Every interaction begins by preserving the original material before normalization or interpretation.

The layer records:

- original content;
- source language and script;
- author, institution, publication, date, and location where applicable;
- retrieval method;
- licence and permitted use;
- whether the material is user-provided, retrieved, translated, generated, attested, or institution-standardized;
- content hash or equivalent identity;
- trust, review, and quarantine state.

This distinction is essential because the model must never treat its own repeated output as independent external corroboration.

The source record remains attached to every downstream claim and interpretation. No normalization or Sanskritization step is permitted to erase the original wording or semantic representation.

---

## 6.2 Script, Normalization, and Phonological Identity

Sanskrit is not inherently bound to one script. The model must separate script identity from lexical identity.

This layer handles:

- Unicode normalization;
- Devanāgarī and transliteration conversion;
- provenance-preserving script mapping;
- canonical phonological representation;
- selected varṇa, place, manner, and sound-class features;
- optional pratyāhāra-class features where they provide measurable value;
- OCR and speech-noise hypotheses;
- visually or phonetically similar but lexically distinct forms.

Several surface strings may resolve to one canonical lexical candidate, while similar strings may need to remain separate. The model therefore stores both:

```text
surface identity
and
canonical phonological identity
```

This layer supports cross-script retrieval, robustness to noisy input, phonological transformation, and controlled tokenization. It does not by itself identify the intended lexeme or concept.

---

## 6.3 Sandhi and Segmentation Lattice

Sandhi maps between underlying lexical sequences and surface phonological forms. It may obscure boundaries and create several plausible analyses.

The architecture therefore represents Sandhi as a **bidirectional probabilistic lattice**, not as a one-time deterministic splitter.

A candidate contains:

```text
surface span
candidate boundaries
candidate canonical forms
generating rules or tools
local phonological score
morphological compatibility
sentence and discourse compatibility
contextual score
status: live / selected / rejected / unresolved
downstream dependencies
```

The model may delay commitment while later layers contribute evidence.

A wrong segmentation can otherwise create a cascade:

```text
wrong boundary
→ wrong lexeme
→ wrong inflection or derivation
→ wrong compound relation
→ wrong event structure
→ wrong concept
→ wrong persistent update
```

To contain this risk:

- multiple candidates remain live;
- confidence is tracked by layer;
- downstream objects retain dependency links;
- low-confidence analyses cannot create permanent updates;
- a corrected segmentation can invalidate and roll back dependent records.

---

## 6.4 Lexical Identity and Inflectional Paradigms

The model distinguishes:

- surface form;
- pada;
- lemma;
- stem;
- prātipadika;
- dhātu or verbal stem;
- lexeme;
- sense;
- concept.

These are related but not interchangeable.

The inflectional layer represents:

### Nominal forms

- stem;
- gender;
- case or vibhakti;
- number;
- paradigm identity;
- irregularity;
- syncretism;
- competing analyses.

### Verbal forms

- root or stem;
- class where relevant;
- person;
- number;
- tense or mood category;
- voice;
- pada where relevant;
- paradigm identity;
- ambiguity and irregularity.

Inflection supplies a clean form of update inheritance. A concept-level correction should normally become available through all valid forms of the same lexeme. It must not propagate merely because an unrelated form shares an ending or surface sequence.

This layer is therefore important not only for language analysis but for testing precise update scope.

---

## 6.5 Derivational Process Graph

Dhātus remain important, but derivation begins from both verbal and nominal bases and involves more than root lookup.

The process graph represents:

- dhātu and prātipadika bases;
- upasargas;
- kṛt suffixes;
- taddhita suffixes;
- selected sanādi formations;
- causatives;
- desideratives;
- intensives;
- feminine derivation;
- nominal-base derivation;
- intermediate states;
- inherited conditions;
- rule order;
- defaults and exceptions;
- multiple possible derivations of one surface form.

The graph records a derivational history rather than only a final decomposition.

```text
base
→ operation
→ intermediate state
→ conditioned operation
→ exception or precedence decision
→ surface form
```

Four identities must remain distinct:

```text
derivationally suggested meaning
≠
attested lexical sense
≠
canonical concept
≠
empirically supported claim
```

The derivational graph can generate a semantic hypothesis and identify related forms. Lexical and evidence layers decide whether the inheritance remains valid in actual usage.

---

## 6.6 Nested Compound Hypergraph

Samāsa can compress relations among several components, but the same surface compound may permit multiple analyses. Multi-component compounds may also have nested internal structure.

The compound layer represents:

- constituent spans;
- nested grouping;
- semantic head where applicable;
- modifier relations;
- exocentricity;
- vigraha candidates;
- candidate compound types;
- domain and register;
- lexicalization;
- attested and disputed interpretations;
- relation to canonical concepts;
- whole-compound and constituent-level inheritance permissions.

A hypergraph is preferable to a flat pairwise graph because one compound analysis may involve several constituents and a relation applying to the group as a whole.

The model retains alternative analyses such as:

```text
Candidate A: one internal grouping and relation
Candidate B: another grouping or relation
Candidate C: lexicalized whole with inheritance blocked
```

Context, event structure, lexical evidence, domain, and external sources determine which interpretation is preferred.

---

## 6.7 Kāraka and Event-Role Graph

The architecture separates surface vibhakti realization from underlying participant relations.

The event graph represents:

- predicate or state;
- agent-like participant;
- affected entity or object;
- instrument;
- recipient or beneficiary;
- source or point of separation;
- location;
- cause;
- result;
- other benchmark-relevant roles;
- omitted or implicit participants;
- active, passive, reordered, and nominalized variants.

This permits several surface expressions to map to one canonical event structure.

```text
teacher gives knowledge to student
knowledge is given to student by teacher
student receives knowledge from teacher
```

The expressions differ, but a substantial event structure may be shared.

This layer is central to knowledge propagation. A correction about the instrument, input, output, agent, or affected entity of a process should propagate to role-equivalent expressions, not merely to sentences with similar words.

---

## 6.8 Sentence-Constraint Layer

The sentence layer evaluates whether candidate analyses jointly form a coherent interpretation.

It models operational approximations of:

- unsatisfied argument expectancy;
- semantic compatibility;
- connectedness or relevant proximity;
- intended-purport signals where explicitly formalized;
- alternative dependency structures;
- ellipsis recovery;
- grammatically possible but semantically anomalous combinations.

The layer must not claim that complex philosophical categories such as tātparya have already been completely formalized. Only precise computational approximations may be implemented.

A major architectural use is **knowledge-gap generation**. If a candidate process requires an instrument or affected entity that remains unknown, the model can formulate a targeted external question rather than conducting broad surface search.

---

## 6.9 Discourse and Coreference Layer

Knowledge assimilation occurs across documents, not isolated sentences.

The discourse layer represents selected relations such as:

- coreference;
- pronoun resolution;
- ellipsis;
- quotation and attribution;
- cause and consequence;
- contrast and concession;
- objection and response;
- example and generalization;
- claim and supporting reason;
- conclusion;
- topic continuity;
- selected śāstric organizational structures.

It must preserve alternative discourse interpretations where evidence is insufficient.

The layer protects locality. A correction should reach genuine references to the same entity or concept while avoiding a nearby but non-coreferential expression.

---

## 6.10 Lexical Sense, Register, Domain, and Period Layer

Morphological relationship does not guarantee current semantic inheritance.

The model assigns stable sense identifiers and distinguishes:

- literal or compositionally suggested sense;
- attested conventional sense;
- lexicalized sense;
- domain-specific technical sense;
- historical sense;
- metaphorical or idiomatic sense;
- school-specific sense;
- institution-approved terminology;
- disputed or minority interpretation;
- deprecated term;
- borrowed or atomic label.

Every sense can carry:

- corpus attestations;
- dictionary provenance;
- source and reviewer history;
- domain;
- register;
- genre;
- period;
- jurisdiction where relevant;
- inheritance permissions;
- blocking exceptions;
- relation to canonical concepts.

This layer prevents a modern computer-science update from contaminating a classical philosophical sense, a poetic metaphor, or a historical usage.

---

## 6.11 Rule-Scope Engine

The rule-scope engine is a research hypothesis inspired by explicit grammatical organization. It is not a claim that a neural continual-learning system is literally identical to the Aṣṭādhyāyī.

The engine represents:

- governing scope;
- inherited context;
- defaults;
- protected exceptions;
- precedence among applicable rules;
- optional alternatives;
- applicability conditions;
- temporary-state isolation;
- internal control metadata;
- dependency and rollback links.

Candidate engineering analogies include:

| Grammatical mechanism | Candidate machine role |
|---|---|
| Adhikāra | Scope governing a family of transformations or updates |
| Anuvṛtti | Context inherited by related operations or descendants |
| Utsarga–apavāda | Default relation with an explicit protected exception |
| Rule precedence | Resolution among simultaneously applicable updates |
| Optionality | Preservation of several admissible analyses |
| It-marker | Internal control information not emitted as surface output |
| Asiddha-like isolation | Prevention of premature cross-stage contamination |

The engine must be compared with an information-equivalent generic executable rule system. Its value cannot be assumed from historical elegance.

---

# 7. Canonical Concept and Evidence Layer

## 7.1 Why concepts remain outside the Sanskrit stack

The architecture must not force reality into Sanskrit morphology.

A concept exists independently of the expression used to name it. One concept may have:

- several Sanskrit labels;
- labels in several other languages;
- disputed terminology;
- an opaque conventional label;
- or no satisfactory Sanskrit label at all.

The canonical concept graph therefore remains language-independent.

## 7.2 Canonical concept record

A concept record may contain:

```text
concept ID
type: entity / process / property / relation / event / proposition
definitions
formal relations
inputs and outputs
participant roles
equations or specifications
algorithms or code
examples and counterexamples
neighbouring and confusable concepts
multilingual labels
Sanskrit candidate labels and sense alignments
domain, jurisdiction, and temporal scope
evidence links
version and review history
```

The model supports:

```text
atomic concept
+ external definition
+ optional Sanskrit label
+ explicit derivation-insufficient status
```

A descriptive Sanskrit expression may help interpret a concept, but it does not become the concept's ontology.

## 7.3 Evidence and provenance graph

The evidence graph stores claim-level warrant:

- atomic claim;
- original source span;
- source identity;
- source date and retrieval date;
- support and contradiction relations;
- source dependencies;
- domain authority;
- temporal validity;
- reliability and review state;
- generated, translated, attested, or standardized status;
- applicability boundaries;
- supersession history.

The evidence graph preserves disagreement rather than forcing institutional uniformity where the evidence remains contested.

## 7.4 Structural confidence and evidential confidence are independent

A model may report:

```text
high structural confidence
moderate concept confidence
low evidence confidence
```

This means that the expression has a plausible analysis, but the claimed referent is weakly supported.

The opposite is also possible:

```text
low Sanskrit-formation confidence
high concept confidence
high evidence confidence
```

This means that the real-world concept is well established even though the Sanskrit terminology or analysis remains unsettled.

---

# 8. Cross-Layer Constraint Intersection

The reconciliation module evaluates candidate interpretations across the full stack.

For an input \(x\), the model constructs a set of candidates:

\[
\mathcal{S}(x)=\{s_1,s_2,\ldots,s_n\}
\]

Each candidate may contain:

- surface and script identity;
- phonological representation;
- Sandhi and segmentation;
- lexical and inflectional analysis;
- derivation;
- compound structure;
- event roles;
- sentence and discourse structure;
- lexical sense;
- domain, register, and period;
- rule-scope information;
- concept alignments;
- evidence links.

The model then estimates which concept and evidence apply:

\[
P(c,e\mid x,\mathcal{S}(x),d,t)
\]

where \(d\) is domain or register and \(t\) is temporal context.

The reconciliation module:

- ranks candidate structures;
- aligns candidates to concepts;
- compares literal structure with attested usage;
- detects contradictions;
- preserves legitimate alternatives;
- identifies missing roles or facts;
- decides whether external retrieval is required;
- proposes update scope;
- chooses a reconciliation outcome.

This layer is where symbolic and neural processing meet. No single grammar engine is treated as infallible. Deterministic tools, neural analyzers, lexical resources, context, and evidence provide candidates and signals whose reliability must be learned and calibrated.

---

# 9. Multi-Index Sanskrit Structural Memory

## 9.1 From one root address to many structural addresses

Version 1 described dhātus as addresses into semantic and derivational families. Version 2 retains that idea but generalizes it.

The memory is addressable through:

- surface and script variants;
- canonical phonological forms;
- Sandhi analyses;
- lexeme or lemma;
- paradigm membership;
- dhātu or prātipadika;
- derivational path;
- compound constituent and hierarchy;
- event role;
- sentence constraint;
- discourse referent;
- lexical sense;
- register, domain, and period;
- canonical concept;
- evidence claim.

A query may enter through any one path and reach the same concept through another.

## 9.2 Operational memory partitions

The structural memory is logically unified but operationally partitioned:

1. **Form and variant memory** — scripts, transliterations, phonological forms, Sandhi manifestations.
2. **Paradigm memory** — lexical identity and nominal or verbal forms.
3. **Derivation memory** — procedural histories, inherited conditions, exceptions, and related forms.
4. **Compound memory** — nested structures, constituent roles, whole-compound senses, lexicalization.
5. **Event and sentence memory** — predicates, roles, constraints, paraphrase relations.
6. **Discourse memory** — references, attribution, relations across sentences and sections.
7. **Lexical-sense and register memory** — conventional meanings, domains, periods, schools, and inheritance blocks.
8. **Rule and meta-rule memory** — scope, defaults, exceptions, precedence, optionality, and dependencies.
9. **Canonical concept memory** — language-independent concepts and formal relations.
10. **Evidence memory** — claims, sources, contradictions, dates, and warrant.
11. **Plastic working memory** — temporary, session-specific, or experimental updates.

Different partitions require different confidence thresholds, update frequencies, retention policies, review groups, and rollback mechanisms.

## 9.3 Retrieval-path observability

The model logs how a result was found.

For example:

```text
surface similarity
→ canonical form
→ paradigm
→ lexical sense
→ concept
```

or:

```text
compound constituent
→ event role
→ canonical concept
→ evidence claim
```

This allows evaluation of whether the structural mechanism genuinely contributed, rather than merely displaying an analysis after retrieving by vector similarity.

---

# 10. Retrieval and Knowledge-Gap Generation

## 10.1 Four operating modes

The router selects among four modes.

### Internal structural mode

Used when:

- the task is grammatical or compositional;
- the required concept is already grounded;
- structural confidence is sufficient;
- no unstable empirical claim is involved.

### External evidence mode

Used when:

- the question concerns current or changing facts;
- empirical evidence is required;
- the domain is high stakes;
- internal knowledge is unsupported or outdated;
- the concept has no adequate internal grounding.

### Reconciliation mode

Used when:

- structure and usage disagree;
- several analyses remain plausible;
- sources conflict;
- a domain-specific sense competes with a literal sense;
- an update crosses protected boundaries.

### Abstention or review mode

Used when:

- uncertainty exceeds policy thresholds;
- evidence remains contradictory;
- terminology requires scholar review;
- domain validation is necessary;
- a safe update scope cannot be established.

## 10.2 Structural knowledge-gap map

The model generates targeted external questions from unresolved constraints.

Example:

```text
Internally established:
- expression denotes a process
- process has backward orientation
- an affected quantity is implied

Still missing:
- identity of the quantity
- structure through which it moves
- formal rule governing movement
- initiating condition
- resulting state
```

The retrieval system searches for those missing relations instead of merely searching the surface term.

Potential advantages include:

- more focused retrieval;
- fewer irrelevant passages;
- lower retrieved-token consumption;
- clearer separation of linguistic and empirical uncertainty;
- better multi-hop evidence collection;
- explicit reasons for retrieval.

These benefits remain hypotheses and must be compared with generic semantic query decomposition.

---

# 11. The Structural Assimilation Compiler

## 11.1 Purpose

The Assimilation Compiler transforms external material into a reversible, structured memory proposal. It does not permit retrieved text to modify persistent knowledge directly.

## 11.2 Compiler stages

| Stage | Intermediate representation | Main result |
|---|---|---|
| IR-0 | Source Record | Original content, provenance, licence, and status |
| IR-1 | Normalized Source | Reversible language and script normalization |
| IR-2 | Source Semantic IR | Source-faithful entities, events, claims, and relations |
| IR-3 | Concept Alignment IR | Candidate canonical concepts and confidence |
| IR-4 | Sanskrit Candidate IR | Candidate Sanskrit labels, forms, and attestation status |
| IR-5 | Structural Analysis IR | Sandhi, morphology, derivation, compounds, roles, discourse, and senses |
| IR-6 | Evidence Assessment IR | Support, contradiction, reliability, and temporal validity |
| IR-7 | Scope Proposal IR | Must-change, may-change, and must-not-change predictions |
| IR-8 | Memory Transaction IR | Reversible additions, corrections, forks, exceptions, and rollback plan |

## 11.3 Information-loss prohibition

Every intermediate representation links back to the prior stage. The Sanskrit analysis must not replace the original source-language semantic representation.

The system retains:

1. original source;
2. source-faithful semantic interpretation;
3. canonical concept alignment;
4. Sanskrit structural alignment;
5. evidence and confidence state;
6. mapping among all representations.

## 11.4 Synthetic-integrity rule

Generated, translated, attested, and institution-standardized materials remain distinct.

The model must not create the following circular authority:

```text
model coins a term
→ model repeatedly translates with the term
→ model observes repeated generated usage
→ model treats repetition as independent attestation
```

## 11.5 Conflict preservation

The compiler preserves:

- competing segmentations;
- competing derivations;
- lexical and dictionary disagreement;
- school-specific analyses;
- domain-specific coexistence;
- historical and modern senses;
- contradictory evidence;
- minority and deprecated terminology.

Unresolved disagreement is represented, not erased.

---

# 12. Reconciliation Outcomes

The reconciliation engine supports more than acceptance or rejection.

| Outcome | Meaning |
|---|---|
| Confirm | Evidence supports the selected structural and concept interpretation |
| Refine | Evidence narrows, qualifies, or makes the interpretation more precise |
| Extend | A new relation, participant, domain, or sense is added |
| Override | Conventional or evidenced meaning supersedes a structural default |
| Fork | Separate senses, periods, domains, schools, or concepts are preserved |
| Merge | Duplicate records are combined after provenance-aware review |
| Supersede | A newer claim replaces an older one without deleting history |
| Expire | A time-bounded claim becomes inactive while remaining auditable |
| Deprecate | A term or analysis is retained but marked as discouraged or obsolete |
| Quarantine | Evidence or analysis remains unreliable or unresolved |
| Reject | The proposed interpretation or evidence is invalid or unsafe |
| Abstain | The system declines commitment and requests expert or domain review |

This prevents both extremes:

- forcing all reality into morphological structure;
- ignoring useful structure and treating every expression as an opaque string.

---

# 13. Scope-Controlled Knowledge Updates

## 13.1 Why update scope is the central mechanism

A useful continual-learning system must answer two questions simultaneously:

1. **Where should a new fact or meaning propagate?**
2. **Where must it stop?**

A model that remembers an update but fails to apply it to related forms has poor propagation. A model that changes every related-looking expression has poor locality.

Version 2 treats the propagation–locality balance as the architecture's strongest scientific target.

## 13.2 Layer-wise update-scope lattice

```text
Update target
│
├── Surface identity
│   ├── script variants
│   ├── transliterations
│   ├── normalization variants
│   └── valid Sandhi manifestations
│
├── Lexical paradigm
│   ├── nominal forms
│   ├── verbal forms
│   └── irregular or exceptional forms
│
├── Derivational scope
│   ├── must inherit
│   ├── may inherit
│   └── must not inherit
│
├── Compound scope
│   ├── whole-compound sense
│   ├── head-related effects
│   ├── constituent-related effects
│   └── lexicalized exception
│
├── Event and sentence scope
│   ├── role-equivalent paraphrases
│   ├── active, passive, and nominalized forms
│   ├── omitted-participant recovery
│   └── incompatible event structures
│
├── Discourse scope
│   ├── genuine coreference
│   ├── ellipsis
│   ├── quotation attribution
│   └── nearby non-coreferential entities
│
├── Cross-language scope
│   ├── equivalent concept labels
│   ├── translation variants
│   └── non-equivalent lexical lookalikes
│
└── Protected boundaries
    ├── homonym
    ├── lexicalized sense
    ├── idiom or metaphor
    ├── different domain
    ├── different register or period
    ├── school-specific interpretation
    ├── competing analysis
    └── unsupported empirical claim
```

An update may propagate through one layer and be blocked at another.

For example:

- a lexical correction should reach all case forms;
- it may reach a derived agent noun;
- it may not reach a lexicalized compound;
- it may apply only in modern computer science;
- it may remain invalid for a historical philosophical usage;
- it may be grammatically plausible but empirically unsupported.

## 13.3 Scope prediction

For a proposed update \(u\), the system predicts:

\[
\Omega(u)=g(\mathcal{S},c,e,d,t,r)
\]

where:

- \(\mathcal{S}\) is the structural analysis;
- \(c\) is the canonical concept;
- \(e\) is the evidence state;
- \(d\) is domain, register, genre, or jurisdiction;
- \(t\) is temporal scope;
- \(r\) contains inheritance, exception, precedence, and blocking relations.

The result is not merely a set of affected strings. It is a typed, explainable prediction of:

```text
must change
may change
must not change
```

## 13.4 Reversible memory transaction

Every persistent update follows a transaction flow:

```text
prepare
→ validate structural analysis
→ validate concept alignment
→ validate evidence
→ predict scope
→ detect conflicts and protected boundaries
→ stage transaction
→ run propagation, locality, and regression checks
→ commit, fork, quarantine, or reject
→ version and audit
```

Supported operations include:

- add;
- correct;
- supersede;
- fork sense;
- merge reviewed duplicates;
- create exception;
- restrict domain, register, jurisdiction, or time;
- deprecate terminology;
- expire a claim;
- rollback.

A rollback restores the previous active state while preserving the update history and dependent audit trail.

---

# 14. Confidence, Ambiguity, and Abstention

## 14.1 Internal confidence is layered

The original distinction among formation, meaning, and warrant remains valuable for users. Internally, however, the model requires finer confidence estimates:

```text
C_script
C_phonology
C_sandhi
C_lexical_identity
C_inflection
C_derivation
C_compound
C_karaka_event
C_sentence
C_discourse
C_lexical_sense
C_register_domain
C_concept_alignment
C_evidence
C_temporal_validity
C_source_reliability
C_update_scope
```

These values must be empirically calibrated. They must not be combined through an arbitrary average or product.

## 14.2 Uncertainty propagates across layers

Example:

```text
uncertain segmentation
→ several lexical analyses
→ several derivations or compound structures
→ different event structures
→ different lexical senses
→ different concept alignments
→ targeted retrieval, alternative answer, or abstention
```

The architecture avoids premature collapse. If two analyses remain plausible, both may continue into retrieval and evidence comparison.

## 14.3 User-facing summary

The model may aggregate internal confidences into three interpretable groups:

- **Formation confidence** — how the expression was structurally analyzed.
- **Meaning confidence** — which concept or sense is intended.
- **Warrant confidence** — how strongly the factual claim is supported.

### Śabda, Artha, and Warrant as an engineering abstraction

Version 1 used three broad layers—Śabda, Artha, and Warrant—to distinguish expression, meaning, and evidence. Version 2 retains that abstraction for explanation while expanding its internal structure:

```text
Śabda / formation
    script, phonology, Sandhi, lexical identity, inflection, derivation, compounds, syntax

Artha / intended concept
    event roles, sentence and discourse interpretation, lexical sense, canonical concept

Warrant / justified belief
    evidence, source reliability, contradiction, time, domain, and review state
```

These labels are used as engineering summaries, not as a claim that classical philosophical categories map directly and completely onto neural architecture.

## 14.4 Ambiguity-preserving output

The model supports:

- one preferred interpretation with alternatives;
- several live interpretations without forced selection;
- grammatical analysis without factual commitment;
- a concept answer with unresolved Sanskrit terminology;
- a domain- or register-restricted answer;
- explicit disagreement among sources or schools;
- abstention and referral for scholar or domain review.

A fluent single answer is not always the correct epistemic response.

---

# 15. Memory Types and Speeds of Learning

## 15.1 Memory types

### Parametric memory

The stable knowledge encoded in model weights:

- general language competence;
- common world knowledge;
- learned reasoning patterns;
- statistical associations;
- instruction-following behaviour.

It is powerful but difficult to inspect and risky to modify continuously.

### Sanskrit structural memory

The explicit, versioned memory covering:

- forms and surface variants;
- phonological identities;
- Sandhi candidates;
- paradigms;
- derivations;
- compounds;
- event roles;
- sentence and discourse relations;
- lexical senses;
- domain, register, and period;
- rule scope, defaults, and exceptions.

This is the principal inward-looking linguistic memory.

### Canonical semantic memory

The language-independent store of:

- concepts;
- events;
- formal relations;
- equations;
- algorithms;
- examples;
- counterexamples;
- multilingual labels;
- concept versions.

### Evidential memory

The source-grounded store of:

- atomic claims;
- supporting and contradicting evidence;
- dates;
- authority;
- source reliability;
- applicability;
- supersession;
- review state.

### Plastic working memory

Temporary or experimental state used for:

- session definitions;
- local terminology;
- unresolved hypotheses;
- staged memory transactions;
- task-specific routing;
- future temporary adapters.

Plastic working memory does not automatically modify the institutional base model.

## 15.2 Speeds of learning

### Token-time interpretation

Duration: milliseconds to seconds.

The model activates structural candidates, memory paths, and domain experts while answering. No persistent state changes.

### Session-time adaptation

Duration: one conversation, document, or research task.

The system stores local assumptions, definitions, evidence, and unresolved mappings. These expire unless deliberately promoted.

### Institutional semantic memory

Duration: days to years.

Verified concepts, terminology, structural analyses, evidence, scope rules, and exceptions enter versioned institutional memory.

### Release-time consolidation

Duration: periodic model releases.

Only stable, repeatedly useful, well-scoped knowledge is considered for distillation into model weights. Consolidation requires review, regression testing, forgetting tests, rollback preparation, and public versioning.

---

# 16. The Semantic Immune System

External retrieval and self-generated corpora create a major attack and contamination surface.

Potential threats include:

- false or fabricated facts;
- prompt injection;
- poisoned documents;
- misleading derivations;
- fabricated terminology;
- politically motivated reinterpretations;
- unreliable authority;
- synthetic translation loops;
- model repetition mistaken for attestation;
- source laundering through paraphrase;
- outdated claims presented as current;
- one school's analysis represented as universal;
- evidence from one domain applied to another.

## 16.1 Quarantine before assimilation

New material first enters a quarantined state.

The system asks:

- Is the source authentic and licensed?
- Is it authoritative for this domain?
- Is it current?
- Is the claim independently corroborated?
- Does it contradict established evidence?
- Is the Sanskrit analysis grammatically and lexically plausible?
- Does the source attempt to control the model rather than provide evidence?
- Does accepting the claim damage unrelated knowledge?
- Is the claim limited by time, domain, register, jurisdiction, or school?
- Is the purported attestation actually model-generated or translated material?

Only then may information progress through:

```text
external material
→ quarantined episodic record
→ reviewed evidence claim
→ verified semantic memory
→ optional later consolidation
```

## 16.2 Source-faithfulness protection

The original source and source-language semantic representation remain available after Sanskrit alignment. This allows auditors to detect:

- translation loss;
- over-interpretation;
- concept drift;
- terminology capture;
- institutional bias;
- unsupported semantic enrichment.

## 16.3 Counter-evidence search

The retrieval process deliberately seeks:

- contradictory evidence;
- alternative senses;
- negative examples;
- exceptions;
- competing definitions;
- domain and period restrictions.

The model must not use its initial interpretation to retrieve only confirming material.

---

# 17. Rehearsal and Validation Before Consolidation

New knowledge should be exercised before it becomes durable.

For each proposed concept or update, the system can generate:

- inflectional variants;
- Sandhi manifestations;
- related derivations;
- nested compounds;
- event-role paraphrases;
- active, passive, and nominalized forms;
- discourse references;
- cross-language equivalents;
- counterexamples;
- confusable concepts;
- lexicalized exceptions;
- alternate domain and historical senses;
- cases where literal derivation fails;
- equations or code where relevant;
- adversarially similar but unrelated expressions.

These examples are checked against:

- structural analyzers;
- canonical concept records;
- external evidence;
- formal validators;
- code execution where applicable;
- domain experts;
- scholar review;
- propagation and locality tests.

The rehearsal cycle is:

```text
new evidence or concept
→ structured memory proposal
→ generated variants and counterexamples
→ propagation and locality tests
→ evidence and domain validation
→ correction or quarantine
→ governed institutional commit
```

This is how the model integrates a concept rather than merely memorizing a sentence.

---

# 18. Controlled Plasticity and Dynamic Reconfiguration

## 18.1 Reconfiguration before rewriting

The governing principle remains:

> **Rewire at the edge; consolidate at the centre.**

But Version 2 changes the order of implementation.

```text
Stage 1: structural analysis
Stage 2: multi-index retrieval
Stage 3: writable semantic and evidential memory
Stage 4: structure-conditioned routing
Stage 5: temporary adapters or fast weights
Stage 6: reviewed base-weight consolidation
```

The first experimental pilot ends before Stage 5.

## 18.2 Forms of reconfiguration

| Form | What changes | Lifetime | Initial status |
|---|---|---:|---|
| Activation routing | Which paths, indexes, or experts are active | One inference | Included |
| Graph and memory update | Relations, concepts, senses, evidence, and scope | Persistent but reversible | Included after validation |
| Temporary adapter | Small task- or evidence-conditioned parameter delta | Session or task | Deferred |
| Base-weight update | Main model parameters | Release cycle | Deferred and governed |

## 18.3 Future effective-weight model

A later architecture may use:

\[
W_{effective}=W_0+\alpha\Delta W_{structure}+\beta\Delta W_{evidence}+\gamma\Delta W_{task}
\]

However, this equation is only a research placeholder until the programme defines:

- how each delta is generated;
- which layers it can modify;
- how structural scope constrains the change;
- how conflicts are isolated;
- how updates expire or promote;
- how rollback works;
- how unrelated capabilities are protected;
- how causality is tested.

No retrieved suggestion is allowed to rewrite base weights directly.

## 18.4 Structural learning objectives

When joint training is permitted, the model may optimize a weighted objective such as:

\[
\mathcal{L}_{total}=
\mathcal{L}_{LM}
+\lambda_1\mathcal{L}_{segmentation}
+\lambda_2\mathcal{L}_{inflection}
+\lambda_3\mathcal{L}_{derivation}
+\lambda_4\mathcal{L}_{compound}
+\lambda_5\mathcal{L}_{event}
+\lambda_6\mathcal{L}_{sentence}+\lambda_{6b}\mathcal{L}_{discourse}
+\lambda_7\mathcal{L}_{sense}
+\lambda_8\mathcal{L}_{concept}
+\lambda_9\mathcal{L}_{evidence}
+\lambda_{10}\mathcal{L}_{calibration}
+\lambda_{11}\mathcal{L}_{scope}
+\lambda_{12}\mathcal{L}_{cross-layer}
\]

The objectives respectively test language modelling, segmentation, paradigm analysis, derivation, compound structure, event roles, sentence and discourse interpretation, lexical sense, concept alignment, evidential grounding, confidence calibration, update scope, and agreement among layers.

No objective is included merely because an annotation exists. Each must have a measurable downstream role and an ablation demonstrating whether it contributes.

## 18.5 Causal integration requirement

The structural stack must affect at least one causal pathway:

- retrieval addresses;
- graph-token fusion;
- attention or gating;
- candidate ranking;
- response selection;
- confidence;
- update-scope prediction;
- routing;
- future adapter generation.

A parser whose output is displayed but ignored by the model does not satisfy the architecture.

---

# Part III — Ecosystem and Institutional Architecture

# 19. Existing Sanskrit Projects as Foundations, Not Competitors

The institution should not rebuild decades of Sanskrit computational work. Existing projects can serve as reusable components, teachers, baselines, standards partners, and sources of expert correction.

The exact use of every project remains subject to technical, licence, maintenance, and governance review.

## 19.1 Four collaboration roles

| Role | Use |
|---|---|
| Reusable component | Integrate code, services, or data formats where technically and legally appropriate |
| Teacher | Generate candidate annotations, derivations, or synthetic supervision |
| Baseline | Establish what existing symbolic or neural systems already achieve |
| Standards partner | Develop shared schemas, benchmarks, and governance |

## 19.2 Illustrative project alignment

| Project or resource | Potential role in Version 2 |
|---|---|
| Saṃsādhanī / Sanskrit Computational Linguistics platform | Morphological, Sandhi, compound, kāraka, generation, and parser candidates; deterministic expert and standards partner |
| Vidyut | High-speed derivation, reverse analysis, Sandhi, generation traces, synthetic examples, and verification |
| Sanskrit Heritage Platform | Alternative segmentations, lexical candidates, morphology, and uncertainty-lattice generation |
| ByT5-Sanskrit | Neural segmentation, morphology, OCR normalization, and strong neural-only baseline |
| SanskritShala and annotation tools | Neural candidate generation, interactive scholar correction, active learning, and benchmark construction |
| SHR++-style workflows | Human-in-the-loop annotation and correction infrastructure |
| SansGPT | Sanskrit generative pretraining and tokenizer baseline |
| DheeYantra and Sanskrit assistants | Instruction-following and conversational Sanskrit baselines |
| BharatGen and Indian foundation-model programmes | General knowledge backbones, compute, multilingual transfer, and national-scale teacher models |
| IndicTrans2 and AI4Bharat resources | Translation candidates, back-translation, multilingual alignment, and cross-language benchmarks |
| Sāmayik | Contemporary Sanskrit seed corpus and translation baseline |
| Sanskrit WordNet and lexical resources | Sense, synonym, concept, and cross-language lexical alignment |
| Universal Semantic Representation | Language-independent concepts, semantic roles, discourse, and generation interfaces |
| Sanskrit Voyager and corpus-search systems | Attestation, morphology-aware retrieval, and evidence grounding |
| Panini Tokenizer and tokenizer experiments | Compression, segmentation, and morphology-versus-token-count baselines |
| ParamTatva | Phonological and Sanskrit-structured representation baseline |
| PINGALA-like systems | Verifier-guided generation and lessons on soft versus hard constraints |
| Pāṇinian Foundation for Indic Processing | Shared representation standards and cross-Indic evaluation collaboration |

The proposed institution contributes the missing integration layer:

```text
existing linguistic expertise
+
open structural interchange standard
+
canonical concept and evidence alignment
+
cross-layer reconciliation
+
update-scope prediction
+
controlled causal evaluation
```

## 19.3 Upstream contribution

Where existing projects are used, the programme should:

- contribute bug fixes and coverage improvements upstream;
- publish adapters rather than private forks where possible;
- fund maintenance and documentation;
- preserve project attribution;
- expose disagreements among tools;
- avoid treating one tool as ground truth;
- create shared evaluation resources.

---

# 20. Institutional Governance

The governance structure is part of the model architecture because it determines which terminology, analyses, evidence, and updates become authoritative.

## 20.1 Required working groups

The programme should establish coordinated groups for:

- representation standards;
- Pāṇinian grammar and derivation;
- phonology, script, and Vedic/historical extensions;
- lexicography and sense inventories;
- sentence semantics and verbal cognition;
- discourse and śāstric organization;
- modern technical terminology;
- domain evidence and validation;
- computational modelling and infrastructure;
- evaluation and statistics;
- security and synthetic integrity;
- provenance, licensing, and open release.

No single category of “Sanskrit expert” is sufficient for the complete stack.

## 20.2 Analysis versus institutional standardization

The system must distinguish:

- historically attested usage;
- dictionary-recorded usage;
- one scholarly interpretation;
- unresolved competing analyses;
- institution-approved modern terminology;
- deprecated terminology;
- model-generated suggestions.

Institutional approval does not erase alternative history or scholarship.

## 20.3 Adjudication

The programme requires:

- annotation manuals;
- inter-annotator agreement measures;
- disagreement taxonomies;
- source and school attribution;
- adjudication procedures;
- published correction history;
- appeal and revision mechanisms;
- independent evaluation.

## 20.4 Versioning and rollback

Every public system state identifies:

- base-model version;
- structural schema version;
- institutional memory version;
- active terminology version;
- evidence snapshot;
- active adapter set, if any;
- retrieval sources;
- session-specific state.

This preserves reproducibility despite evolving memory.

---

# 21. Open-Weight and Open-Research Release Model

Open weights alone are insufficient for an institutionally significant research programme.

The programme should release, subject to rights and safety constraints:

- model weights and checkpoints;
- tokenizers;
- training and inference code;
- structural interchange schemas;
- tool adapters;
- canonical concept and evidence models;
- annotation guidelines;
- benchmark data and hidden-test governance procedures;
- evaluation harnesses;
- causal-intervention tools;
- model cards;
- corpus documentation;
- provenance records;
- known limitations;
- negative results;
- rollback and version policies.

The programme must state clearly whether a release is:

- open weight;
- open code;
- open data;
- open training recipe;
- open evaluation;
- or fully reproducible open research.

---

# 22. Institutional Deliverables

## 22.1 Sanskrit Structural Interchange Format

An open format capable of representing:

- candidate analyses;
- typed nodes and relations;
- derivation traces;
- hyperedges;
- rule scope;
- confidence;
- provenance;
- tool and version;
- human corrections;
- unresolved alternatives;
- licence and review state.

## 22.2 Multi-Index Sanskrit Structural Memory

A reference implementation supporting structural, conceptual, evidential, and discourse retrieval with logged paths.

## 22.3 Canonical Concept and Evidence Commons

A governed knowledge resource containing:

- concept IDs;
- definitions;
- formal relations;
- terminology;
- Sanskrit structural alignments;
- equations and code;
- source evidence;
- disagreement;
- version history.

## 22.4 Structural Assimilation Compiler

A reproducible pipeline from source material to reversible memory proposals.

## 22.5 Rule-Scope and Update-Scope Engine

A system for predicting inheritance, exceptions, protected boundaries, and rollback dependencies.

## 22.6 Propagation–Locality Benchmark

A benchmark measuring where new knowledge should and should not propagate across:

- forms;
- paradigms;
- derivations;
- compounds;
- event paraphrases;
- discourse;
- domains;
- registers;
- languages.

## 22.7 Open Model Family

The programme should maintain three related tracks:

### Track A — Research-native model

A relatively small Sanskrit-primary model trained from scratch or continued from a controlled initialization. Its purpose is causal research, matched ablations, and reproducibility.

### Track B — Capability model

A strong open multilingual or Indian foundation-model backbone connected to structural retrieval, concept/evidence memory, and verification. Its purpose is practical translation, education, technical assistance, and institutional deployment.

### Track C — Sanskrit Structural Adapter SDK

A reusable open layer that can attach the structural stack to multiple backbones. If the adapter improves unrelated model families, the institution demonstrates an architectural contribution rather than one successful checkpoint.

Specialist Vedic, prosodic, manuscript, or multimodal models remain separately gated extensions.

## 22.8 Sanskrit Technical Knowledge Commons

The institution should maintain a provenance-rich modern knowledge resource rather than an undifferentiated translated corpus. Each concept record can contain:

```text
concept ID
source-language terms
approved and alternative Sanskrit labels
structural analyses
definition
domain and register
equations and formal relations
algorithms and code
examples and counterexamples
confusable concepts
source evidence
reviewers and disagreements
attested / translated / generated / standardized status
version history
```

A governed corpus-expansion loop may operate as:

```text
concept and terminology design
→ source-aligned translation candidates
→ Sanskrit and domain review
→ concept/evidence records
→ model training and evaluation
→ improved translation assistance
→ further reviewed corpus expansion
```

The loop is not allowed to treat model-generated frequency as independent attestation.

---

# Part IV — Scientific Identity, Risks, and Roadmap

# 23. Scientific Novelty

## 23.1 Relationship to existing paradigms

| Existing paradigm | Existing strength | Distinct question introduced here |
|---|---|---|
| Ordinary LLM | Broad parametric pattern learning | Can explicit Sanskrit structure constrain interpretation and update scope? |
| RAG | Retrieves external passages | Can internal structural gaps generate better retrieval and durable assimilation? |
| Knowledge graph | Stores concepts and relations | Can linguistic transformations, paradigms, discourse, and rule scope improve addressing and inheritance? |
| Universal linguistic representation | Encodes language-neutral structure | Does the Sanskrit organization add value beyond equivalent universal features? |
| Generic executable grammar | Provides transformations, defaults, and exceptions | Do Sanskrit-derived rule organizations produce a better propagation–locality trade-off? |
| Model editing or continual learning | Changes knowledge or behaviour | Can multilayer structural scope improve propagation, locality, reversibility, and auditability? |
| Sanskrit parser | Produces linguistic analyses | Can those analyses causally control retrieval, concept alignment, and memory transactions? |
| Sanskrit LLM | Generates or understands Sanskrit | Does the complete structural stack improve learning and updates beyond Sanskrit fluency? |

## 23.2 What is not claimed as new

The project does not claim to be the first:

- Sanskrit language model;
- Sanskrit generative model;
- morphology-aware tokenizer;
- Sandhi splitter;
- Sanskrit parser;
- Pāṇinian computational system;
- compound analyzer;
- Sanskrit semantic representation;
- knowledge graph;
- retrieval-augmented model;
- model-editing method;
- dynamic router;
- persistent-memory system;
- or open Indian-language model.

These areas have substantial prior work.

## 23.3 The causal principle under test

The proposed contribution is narrower and stronger:

> **Can an executable multilayer Sanskrit structural representation causally improve how a foundation model acquires, retrieves, propagates, restricts, revises, and explains knowledge when compared with information-equivalent universal linguistic, semantic, procedural, learned-neural, vector-memory, and text-only alternatives?**

The relevant Sanskrit-specific features include:

- transformations between surface and canonical forms;
- paradigmatic identity;
- derivational history;
- nested compound organization;
- predicate-centred event roles;
- sentence and discourse constraints;
- lexicalized and domain-bounded senses;
- explicit inheritance, default, exception, precedence, and optionality;
- cross-layer constraint intersection.

## 23.4 The strongest novelty endpoint

The strongest possible evidence is not fluent Sanskrit generation. It is a measurable shift in the **propagation–locality frontier**.

At a fixed level of non-target preservation, the Sanskrit structural system should propagate a valid update more accurately to:

- surface and script variants;
- Sandhi manifestations;
- inflectional forms;
- inheriting derivatives;
- relevant compounds;
- event-equivalent paraphrases;
- discourse references;
- cross-language equivalents.

At the same time, it should better protect:

- homonyms;
- unrelated paradigms;
- non-inheriting derivatives;
- lexicalized compounds;
- idioms;
- unrelated event roles;
- different domains;
- different registers and periods;
- competing scholarly analyses;
- unsupported claims.

## 23.5 Defensible Version 2 uniqueness statement

> **This programme tests whether an executable multilayer Sanskrit structural representation—spanning phonological transformation, Sandhi, inflection, derivation, compound hierarchy, predicate-centred event roles, sentence and discourse constraints, lexicalized meaning, register, and explicit rule scope—can causally improve knowledge acquisition, multi-index retrieval, propagation, exception handling, and update locality over information-equivalent universal linguistic, semantic-graph, generic procedural, learned-neural, vector-memory, and text-only baselines.**

The project earns this claim only through controlled evidence. The architecture's completeness is not itself proof of novelty.

---

# 24. Principal Risks and Failure Modes

## 24.1 Etymological fallacy

The current meaning of a word may not equal its derivational history or literal composition.

**Protection:** separate derivation, lexical sense, canonical concept, and evidence; allow lexicalization to block inheritance.

## 24.2 Circular self-confirmation

The model may form an internal hypothesis, retrieve only similar material, and treat that similarity as confirmation.

**Protection:** require counter-evidence retrieval, competing interpretations, source diversity, and evidence-level provenance.

## 24.3 Forcing reality into Sanskrit structure

Some concepts may not map cleanly to inherited categories or elegant compounds.

**Protection:** preserve atomic canonical concepts, optional labels, and explicit derivation-insufficient status.

## 24.4 Terminology engineering artifact

A descriptive technical term may help simply because experts deliberately encoded its definition, not because the broader Sanskrit architecture is superior.

**Protection:** compare with equally descriptive controlled terminology in English and other languages, and with information-equivalent universal representations.

## 24.5 Natural-language ambiguity

A system that performs well on engineered terminology may fail on attested compounds, polysemy, idioms, discourse, and historical usage.

**Protection:** evaluate clean-room fictional, engineered technical, and attested natural Sanskrit separately.

## 24.6 Parser cascade

One wrong early analysis may corrupt every later layer.

**Protection:** preserve lattices, delay commitment, track dependencies, run cross-layer consistency checks, and roll back downstream records.

## 24.7 Graph explosion

The multilayer lattice can grow combinatorially.

**Protection:** sparse representations, candidate beams, pruning, caching, memoization, approximate indexes, hot and archival memory, retrieval-depth limits, and explicit latency budgets.

## 24.8 Weak tooling

Scholar-validated structure may help while automatically predicted structure is too noisy for practical use.

**Protection:** distinguish oracle, rule-generated, neural-predicted, ensemble, and noisy conditions. Treat oracle success with predicted failure as a tooling gap, not proof of deployment readiness.

## 24.9 Structural traces without causal use

The model may display a plausible analysis while answering from unrelated neural memory.

**Protection:** remove, corrupt, substitute, or patch structural states and measure changes in retrieval, confidence, answer, routing, and update scope.

## 24.10 Over-propagation

Formal inheritance may spread updates into lexicalized, domain-specific, or historical senses that should remain protected.

**Protection:** explicit sense IDs, blocking exceptions, domain and register boundaries, propagation–locality evaluation.

## 24.11 Under-propagation

The model may store a correction without applying it to valid variants and consequences.

**Protection:** gold update-scope lattices, multi-hop propagation tests, event and discourse paraphrases, and sequential update evaluation.

## 24.12 Synthetic-data circularity

Generated Sanskrit may become the model's own evidence.

**Protection:** strict status labels, source-language preservation, untouched tests, independent attestation, and expert-reviewed concept IDs.

## 24.13 Institutional capture

One institution may turn a preferred terminology or interpretation into an apparently universal truth.

**Protection:** preserve source and school attribution, minority analyses, attested versus standardized status, public revision history, and independent boards.

## 24.14 Security and poisoning

Retrieved material may contain malicious instructions, fabricated evidence, or targeted memory poisoning.

**Protection:** source quarantine, instruction/content separation, trust policies, corroboration, scope restrictions, staged transactions, and no direct weight rewrite.

## 24.15 Catastrophic drift

Persistent memory and future adapters may gradually alter unrelated behaviour.

**Protection:** versioned memory, expiry, rollback, locality tests, regression suites, and delayed weight consolidation.

## 24.16 Loss of reproducibility

Two deployed instances may diverge because of different memory states.

**Protection:** publish base-model, schema, memory, evidence, adapter, and session-state versions for every reproducible run.

## 24.17 Attribution overreach

The project may label heterogeneous Sanskrit traditions as purely Pāṇinian.

**Protection:** maintain the layered attribution model and use “Sanskrit Structural” for the complete architecture.

## 24.18 Excessive system complexity

The architecture may become too large to attribute gains or failures.

**Protection:** structural ladder, leave-one-layer-out ablations, frozen-model phases, and stage-gated implementation.

---

# 25. Scientific Evaluation in Brief

The companion controlled protocol provides the complete experimental design. This paper records the conceptual requirements.

## 25.1 Core comparison

All systems must receive the same:

- facts and definitions;
- concept records;
- evidence;
- model backbone;
- tokenizer where possible;
- graph capacity;
- retrieval budget;
- context budget;
- training and inference compute.

Only the representation and mechanism under test should change.

## 25.2 Required baseline families

The Sanskrit stack must be compared with:

- text-only context;
- flat vector memory;
- strong generic semantic graph;
- information-equivalent universal linguistic stack;
- generic executable grammar with scope, inheritance, defaults, exceptions, and precedence;
- learned neural latent structure;
- controlled descriptive English;
- another morphologically rich language where feasible.

Beating a weak graph or text-only baseline is insufficient for a Sanskrit-specific architectural claim.

## 25.3 Structural ladder

```text
S0 text only
S1 script + phonology + Sandhi
S2 inflection
S3 derivation
S4 compounds
S5 kāraka and event roles
S6 sentence constraints
S7 discourse and coreference
S8 rule scope, defaults, and exceptions
S9 lexical sense, register, and evidence
S-Full complete stack
```

The programme also runs full-minus-one-layer ablations.

## 25.4 Evaluation worlds

1. **Clean-room fictional knowledge** — prevents pretraining leakage and allows exact update scope.
2. **Engineered modern technical knowledge** — tests terminology, equations, code, and practical reasoning.
3. **Attested natural Sanskrit** — tests real ambiguity, lexicalization, discourse, genre, and historical usage.

## 25.5 Main capabilities tested

- concept acquisition from few examples;
- multi-index retrieval;
- propagation;
- update locality;
- ambiguity and calibration;
- causal use;
- external-query generation;
- end-to-end efficiency.

## 25.6 Oracle versus predicted structure

The programme distinguishes:

- scholar-validated oracle structure;
- rule-engine-generated structure;
- neural-predicted structure;
- ensemble structure;
- deliberately noisy structure.

Possible interpretations:

- **Oracle succeeds, predicted fails:** the representation may be valuable, but tooling is inadequate.
- **Oracle fails:** the structural hypothesis itself is weakened.

---

# 26. Research and Scaling Roadmap

## Stage 0 — Specification

Deliver:

- bounded coverage contract;
- attribution model;
- canonical concept and evidence schemas;
- structural interchange format;
- annotation manual;
- expert governance;
- baseline and equivalence rules;
- pre-registered stopping criteria.

## Stage 1 — Representation and graph-only falsification

Build:

- oracle structural records;
- tool adapters;
- generic and universal controls;
- clean-room benchmark;
- graph-only retrieval and scope prediction.

Question:

> Does the Sanskrit topology and rule organization provide any signal before an LLM is involved?

## Stage 2 — Frozen-model structural retrieval

Use one frozen base model. Train only structural encoders, retrieval components, and response interfaces.

Question:

> Does the explicit stack improve acquisition, retrieval, propagation, locality, and calibration without modifying base weights?

## Stage 3 — Joint structural learning

Add:

- graph-token fusion;
- auxiliary structural objectives;
- cross-layer consistency learning;
- causal interventions;
- multiple backbone validation.

Question:

> Does joint learning add value beyond external structural retrieval?

## Stage 4 — Writable institutional memory

Introduce:

- persistent concept and evidence updates;
- sequential corrections;
- versioning;
- rollback;
- propagation and locality under long update sequences.

Question:

> Can the system assimilate knowledge safely without rewriting base weights?

## Stage 5 — Structure-conditioned routing

Allow dynamic selection among:

- structural indexes;
- domain experts;
- retrieval strategies;
- verification modules.

Question:

> Does structure improve routing and reduce unnecessary computation or retrieval?

## Stage 6 — Temporary adapters and controlled plasticity

Only after earlier stages succeed, test:

- scope-conditioned adapters;
- fast weights;
- task memory;
- rehearsal;
- controlled consolidation.

This stage requires a separate protocol.

## Stage 7 — Larger open-weight capability model

Scale only if:

- the propagation–locality frontier improves beyond strong controls;
- predicted structure retains meaningful oracle benefits;
- causal use is demonstrated;
- cost remains proportionate;
- results reproduce independently.

## Stage 8 — Specialist Sanskrit expansion

Add separately validated modules for:

- Vedic accent and morphology;
- recensional and oral variation;
- Chandas;
- kāvya and alaṅkāra;
- extended śāstric discourse;
- manuscript restoration;
- recitation and multimodal inputs.

---

# 27. Decision and Falsification Rules

The programme must narrow or stop its strongest claim if:

- the full stack does not beat an information-equivalent universal linguistic stack;
- a generic executable grammar matches propagation and locality;
- gains disappear under family, sense, discourse, domain, or register holdouts;
- results occur only for engineered descriptive terminology;
- attested natural Sanskrit does not reproduce controlled gains;
- predicted analyses erase oracle gains without a credible tooling path;
- causal interventions show the model ignores the structural inputs;
- structural cost outweighs meaningful accuracy, data-efficiency, or memory gains;
- propagation improves only by damaging locality;
- independent replication fails.

Possible programme outcomes are:

| Result | Appropriate conclusion |
|---|---|
| Beats only text or vector memory | Explicit structure helps; Sanskrit-specific novelty is unproven |
| Matches universal linguistic stack | Narrow the claim to explicit linguistic structure generally |
| Matches generic executable grammar | Procedural scope explains the gain; Sanskrit is a strong instance |
| Only lexical and morphological tasks improve | Continue as Sanskrit morphology and terminology research |
| Event and discourse tasks improve | Broaden to structured concept and document assimilation |
| Propagation rises but locality falls | Inheritance mechanism is unsafe |
| Oracle succeeds but predicted structure fails | Invest in tools before model scale |
| Full stack shifts propagation–locality across all worlds | Strong support for the central architectural claim |
| Costs exceed meaningful benefits | Preserve resources but do not claim an efficiency architecture |

Negative findings remain valuable if the datasets, schemas, tools, and benchmarks are released.

---

# 28. Where the Model Could Be Competitive

The first objective is not universal superiority over the largest commercial models.

The architecture is designed to compete on specific capabilities.

## 28.1 Novel-expression understanding

Interpret well-formed but unseen inflections, derivations, and compounds while preserving uncertainty.

## 28.2 Low-shot concept acquisition

Use structural priors and canonical grounding to learn new concepts from fewer examples.

## 28.3 Precise knowledge updates

Propagate corrections to valid forms, event paraphrases, and discourse references while protecting unrelated senses and domains.

## 28.4 Technical Sanskrit

Produce consistent terminology linked to definitions, equations, algorithms, code, evidence, and review history.

## 28.5 Morphology-aware and concept-aware retrieval

Retrieve through scripts, Sandhi variants, paradigms, derivations, compounds, roles, senses, concepts, and evidence.

## 28.6 Cross-language transfer

Align Sanskrit structures with language-independent concepts and apply knowledge through English and other Indian-language interfaces.

## 28.7 Auditable outputs

Expose:

- structural trace;
- concept trace;
- evidence trace;
- confidence and alternatives;
- update-scope trace;
- provenance and version.

## 28.8 Smaller-model competence

Test whether explicit structure allows a smaller model to approach a larger purely neural model on targeted tasks.

## 28.9 Institutional knowledge management

Support governed terminology, versioned evidence, reproducible updates, rollback, and long-term public stewardship.

---

# 29. Broader Perspectives

## 29.1 Linguistic perspective

Sanskrit becomes more than a language of output. Its structural traditions become a set of explicit hypotheses about how forms, meanings, relations, defaults, and exceptions can be represented computationally.

## 29.2 Cognitive perspective

The system resembles a reasoner that interprets new information through prior structures but remains capable of revising those structures when evidence demands it.

The architecture does not claim human-like cognition or literal internal Sanskrit thought. Its contribution is explicit, inspectable constraint and memory structure.

## 29.3 Epistemological perspective

The model distinguishes:

- what is structurally possible;
- what is likely intended;
- what concept is represented;
- what evidence supports the claim;
- how certain each layer remains;
- which changes are justified.

## 29.4 Software-engineering perspective

The model resembles a stable kernel surrounded by:

- typed structural modules;
- versioned graphs;
- transducers;
- writable memory;
- reversible transactions;
- validators;
- routing;
- future adapters;
- audit logs.

## 29.5 Institutional perspective

An institution is particularly suited to the architecture because durable semantic memory requires:

- terminology governance;
- evidence standards;
- expert adjudication;
- versioning;
- public accountability;
- long-term maintenance;
- open releases;
- rollback and correction.

## 29.6 Efficiency perspective

Potential efficiency benefits include:

- native tokenization;
- retrieval through canonical forms;
- reduced redundant search;
- smaller retrieved contexts;
- structural caching;
- dynamic routing;
- lower exposure requirements for new concepts.

Every benefit must be measured end to end, including parser, graph, storage, and reconciliation costs.

---

# 30. Final Vision: A Governed Knowledge Metabolism

The Version 2 model is not best described as an LLM that looks inward instead of outward.

It is:

> **A foundation model whose multilayer Sanskrit structural system generates and constrains candidate interpretations; whose canonical concept layer prevents language from defining reality; whose external evidence grounds or corrects claims; and whose reversible institutional memory controls how validated knowledge propagates, where it stops, and when it may later be consolidated.**

Its knowledge metabolism is:

```text
preserve the source
        ↓
construct structural alternatives
        ↓
align canonical concepts
        ↓
identify missing roles, facts, and evidence
        ↓
retrieve or request what is absent
        ↓
compare structure, usage, discourse, and evidence
        ↓
retain ambiguity or select a reconciled interpretation
        ↓
predict propagation and protected boundaries
        ↓
rehearse variants, consequences, and counterexamples
        ↓
commit a reversible, versioned memory transaction
        ↓
consolidate into weights only after sustained validation
```

The architecture's scientific value depends on a demanding result:

> **The Sanskrit structural stack must outperform information-equivalent universal and procedural alternatives, not merely unstructured text.**

A positive result would support a broader foundation-model principle:

> **A formally organized natural language can provide an executable system not only for representing expressions, but for constraining interpretation, generating alternatives, defining inheritance, protecting exceptions, retrieving evidence, and controlling where knowledge updates should and should not propagate.**

A negative result would still produce valuable open corpora, standards, analyzers, benchmarks, terminology, and evidence infrastructure. It would, however, require the institution to narrow the architectural claim rather than scale on belief alone.

---

# Appendix A — End-to-End Illustrative Example

Suppose a technical domain introduces or revises a concept represented by canonical concept `C-042`.

## A.1 External source

```text
Claim:
In domain D, process P operates on vectors rather than scalars.

Evidence:
Two reviewed domain sources.

Temporal scope:
Current.
```

## A.2 Source preservation

The compiler stores:

- original source spans;
- authors and institutions;
- publication and retrieval dates;
- licence;
- source-language semantic parse;
- extracted atomic claim;
- evidence confidence.

## A.3 Structural alignment

The system identifies:

- candidate Sanskrit term and alternative labels;
- surface and Sandhi manifestations;
- lexical identity;
- inflectional paradigm;
- derivational relations;
- compound occurrences;
- event structure;
- domain-specific lexical sense;
- competing historical or general senses.

## A.4 Scope prediction

```text
Must change:
- domain-D definition of C-042
- approved Sanskrit domain sense
- inflectional forms referring to that sense
- inheriting derivatives whose argument type is inherited
- compounds whose whole meaning depends on that sense
- event-role paraphrases
- genuine discourse references

May change:
- rate or instrument terms whose definitions depend on input type
- cross-language explanatory examples

Must not change:
- historical scalar usage
- unrelated domain D2
- lexicalized compound L-19
- homonymous stem H-4
- metaphorical use M-7
- unsupported claim that all related processes use vectors
```

## A.5 Reconciliation

The engine may choose:

- **Refine** if the domain sense already exists;
- **Fork** if general and domain-specific senses must coexist;
- **Supersede** if the prior domain claim is outdated;
- **Quarantine** if evidence conflicts.

## A.6 Rehearsal

The model tests:

- inflectional variants;
- related compounds;
- active and nominalized event forms;
- cross-language questions;
- lexicalized exceptions;
- unrelated homonyms;
- rollback.

## A.7 Commit

The transaction stores:

- new concept version;
- updated sense alignment;
- evidence links;
- affected records;
- protected records;
- confidence;
- reviewer approval;
- rollback dependency;
- public version.

---

# Appendix B — Version 1 to Version 2 Section Alignment

The following table records how every major section of `Paninian_Self_Assimilating_Model.md` was preserved, expanded, relocated, or constrained.

| Version 1 section | Version 2 alignment | Main change |
|---|---|---|
| Executive Idea | Executive Idea; Sections 1 and 30 | Preserved knowledge assimilation, but replaced derivation-centred framing with the complete structural stack |
| §1 Central Insight: Inward Structure, Outward Evidence | Sections 1, 10, and 11 | Preserved the inward/outward loop and made retrieval depend on cross-layer uncertainty and explicit compiler stages |
| §2 Dhātus as Internal Addresses | Sections 2, 6.4–6.5, and 9 | Retained dhātus as one useful address; replaced root primacy with multi-index memory |
| §3 Looking Within Itself Must Be Explicit | Sections 8–10 | Retained explicit memory beside weights and defined structural, concept, evidence, and retrieval paths |
| §4 Reconfiguration Before Rewriting | Section 18 | Preserved “rewire at the edge; consolidate at the centre” and made plasticity stage-gated |
| §5 Proposed Architecture | Sections 5–13 | Reconstructed the architecture around typed layers, concept independence, reconciliation, and update scope |
| §6 Four Types of Memory | Section 15 | Expanded derivational memory into Sanskrit structural memory and separated canonical semantic memory |
| §7 Assimilation Compiler | Section 11 | Replaced a claim-centred compiler with eight provenance-preserving intermediate representations |
| §8 Realignment Must Be Two-Way | Sections 8 and 12 | Preserved external correction and expanded reconciliation outcomes to fork, supersede, expire, merge, reject, and abstain |
| §9 Śabda, Artha, and Warrant | Sections 7 and 14 | Preserved as a user-facing engineering abstraction while adding fine-grained internal confidence |
| §10 Dynamic Rewiring Through Effective Weights | Section 18 | Retained as a future hypothesis; removed from the first pilot and added scope and causal requirements |
| §11 Semantic Inheritance With Override | Sections 6.10–6.11 and 13 | Replaced informal inheritance with sense IDs, rule scope, protected exceptions, and a layer-wise update lattice |
| §12 Four Speeds of Learning | Section 15.2 | Preserved token-, session-, institutional-, and release-time learning |
| §13 Model Decides When Not to Retrieve | Section 10.1 | Expanded to internal, external, reconciliation, and abstention/review modes |
| §14 Internal Structure as Retrieval-Query Generator | Section 10.2 | Preserved and generalized from derivational gaps to missing roles and cross-layer constraints |
| §15 Semantic Immune System | Section 16 | Expanded to source faithfulness, translation loops, synthetic attestation, disagreement, and counter-evidence search |
| §16 Rehearsal and Dreaming | Section 17 | Expanded rehearsal across paradigms, compounds, event paraphrases, discourse, exceptions, registers, equations, and code |
| §17 Comparison With Existing Paradigms | Sections 19 and 23.1 | Separated ecosystem collaboration from scientific comparison with universal and procedural baselines |
| §18 Potentially Unique Institutional Deliverables | Section 22 | Replaced root-centred deliverables with interchange standards, multi-index memory, concept/evidence commons, and scope benchmarks |
| §19 Principal Risks | Section 24 | Preserved the original risks and added parser cascades, graph growth, tooling, causal traces, institutional capture, and baseline artifacts |
| §20 Research Programme | Sections 25–27 | Replaced Models A–E as the primary design with structural ladders, strong controls, stages, and stop conditions |
| §21 Training Objectives | Section 18.4 and Section 25 | Expanded objectives across all structural layers and required downstream ablation evidence |
| §22 Broader Perspectives | Section 29 | Preserved linguistic, cognitive, epistemological, engineering, institutional, and efficiency perspectives |
| §23 Defensible Uniqueness Statement | Section 23 | Narrowed novelty to a causal comparison of the complete structural principle against matched alternatives |
| §24 Final Insight: Knowledge Metabolism | Section 30 | Preserved the metaphor and aligned it to concept independence, scope-controlled memory, and governed consolidation |
| Selected References | Appendix F | Retained the source evidence base and expanded Sanskrit-project references |

A concise formulation of the largest conceptual replacements is:

| Version 1 formulation | Version 2 formulation |
|---|---|
| Dhātu-addressed internal memory | Multi-index Sanskrit structural memory |
| Derivational memory | Partitioned Sanskrit structural memory plus canonical semantic memory |
| Pāṇinian self-retrieval | Cross-layer constraint intersection and structural retrieval |
| Semantic inheritance with override | Typed update-scope lattice with protected boundaries |
| Tri-axial confidence only | Layer-level uncertainty with formation, meaning, and warrant summaries |
| Dynamic effective weights as near-term architecture | Deferred plasticity after frozen-model and writable-memory validation |
| D > B and E > D as primary comparisons | Propagation–locality frontier against strong matched baselines |

---

# Appendix C — Alignment with the Controlled Experimental Protocol

This conceptual paper is aligned to the companion protocol in the following ways:

| Protocol decision | Concept-paper implementation |
|---|---|
| Internal representation is not dhātu-centred | Sections 6 and 9 define the complete stack and multi-index memory |
| Canonical concepts remain language-independent | Section 7 separates concepts and evidence from Sanskrit structure |
| First pilot excludes fast-weight rewriting | Section 18 defers adapters and base-weight updates |
| Propagation–locality is the strongest endpoint | Sections 13 and 23 make update scope central |
| Full stack faces strong controls | Section 25 summarizes universal, semantic, procedural, neural, vector, and text baselines |
| Alternative analyses remain live | Sections 6, 8, and 14 preserve lattices and ambiguity |
| Every update is reversible and versioned | Section 13 defines the transaction manager |
| Synthetic status remains explicit | Sections 11 and 16 prohibit circular attestation |
| Causal use must be tested | Sections 4, 9, 24, and 25 require intervention-based evidence |
| Scaling is stage-gated | Sections 26 and 27 define progression and stop rules |

---

# Appendix D — Traceability to the Refactored Gap Analysis

| Gap family | Version 2 resolution |
|---|---|
| FG-01 Scope, attribution, and bounded coverage | Sections 3 and 20 define layered attribution, coverage boundaries, and governance |
| FG-02 Script, phonology, Sandhi, and surface identity | Sections 6.1–6.3 define provenance, canonical identity, and probabilistic segmentation |
| FG-03 Inflection, derivation, compounds, and lexical sense | Sections 6.4–6.6 and 6.10 separate paradigms, processes, hypergraphs, and senses |
| FG-04 Event structure, sentence interpretation, discourse, and register | Sections 6.7–6.10 define event, sentence, discourse, and boundary layers |
| FG-05 Executable rules and structural representation | Sections 5–9 define typed layers, rule scope, concept independence, and multi-index retrieval |
| FG-06 Assimilation, memory, inheritance, and update scope | Sections 11–13 and 15 define compiler stages, memory partitions, scope lattice, and transactions |
| FG-07 Confidence, ambiguity, and response policy | Section 14 defines layer-level confidence, alternatives, and abstention |
| FG-08 Data, annotation, expert review, and synthetic integrity | Sections 16, 19–22 define synthetic safeguards, partner roles, governance, and open infrastructure |
| FG-09 Experimental controls and novelty measurement | Sections 23, 25, and 27 define strong baselines, structural ladders, and falsification |
| FG-10 Plasticity and dynamic rewiring | Section 18 defers adapters and weight consolidation until structural gates pass |
| FG-11 Error containment, scale, interoperability, and causal observability | Sections 6.3, 9.3, 16, 21–22, and 24 define containment, logging, standards, and causal tests |
| FG-12 Governance, uniqueness, and falsification | Sections 20, 23, 26–27 define governance, narrow claims, stage gates, and stopping rules |

---

# Appendix E — Source Basis and Supersession

This Version 2 conceptual paper synthesizes and aligns:

1. `Sanskrit_Native_LLM_Proposal(1).md`
2. `Paninian_Grounded_Foundation_Model_Strategy.md`
3. `Paninian_Self_Assimilating_Model.md`
4. `Paninian_Self_Assimilating_Model_Gap_Analysis_Refactored_v2.md`
5. `Sanskrit_Structural_Self_Assimilating_Model_V2_Research_Architecture_and_Protocol.md`

The earlier documents remain part of the project's intellectual and design history.

This document supersedes `Paninian_Self_Assimilating_Model.md` as the authoritative conceptual architecture. It does not supersede the companion controlled experimental protocol for benchmark, statistical, implementation, or stage-gate details.

---

# Appendix F — Selected References

The following references are retained from the source documents as the immediate evidence base for the architectural motivation. The architecture itself remains a research hypothesis.

- Amrith Krishna et al., **Word Segmentation in Sanskrit Using Path Constrained Random Walks** — <https://aclanthology.org/C16-1048/>
- Jivnesh Sandhan et al., **DepNeCTI: Dependency-based Nested Compound Type Identification for Sanskrit** — <https://aclanthology.org/2023.findings-emnlp.914/>
- Amba Kulkarni et al., **Dependency Relations for Sanskrit Parsing and Treebank** — <https://aclanthology.org/2020.tlt-1.12/>
- Harshad Ayachit et al., **Computational Modelling of the Apatyādhikāra in Aṣṭādhyāyī** — <https://aclanthology.org/2026.iscls-1.16/>
- Tapas Khanra et al., **TantraTagger** — <https://aclanthology.org/2026.iscls-1.4/>
- Sriram Krishnan et al., **Challenges in Processing Vedic Sanskrit** — <https://aclanthology.org/2025.wsc-csdh.9/>
- Anagha Pradeep et al., **Towards Building a Computational Sense Inventory from the Monier-Williams Dictionary** — <https://aclanthology.org/2026.iscls-1.3/>
- Lewis et al., **Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks** — <https://arxiv.org/abs/2005.11401>
- Mitchell et al., **Memory-Based Model Editing at Scale** — <https://proceedings.mlr.press/v162/mitchell22a.html>
- Asai et al., **Self-RAG** — <https://openreview.net/forum?id=hSyW5go0v8>
- SansGPT — <https://aclanthology.org/2024.icon-1.50/>
- ByT5-Sanskrit — <https://aclanthology.org/2024.findings-emnlp.805/>
- Saṃsādhanī / Sanskrit Computational Linguistics platform — <https://sanskrit.uohyd.ac.in/scl/>
- Vidyut — <https://github.com/ambuda-org/vidyut>
- Sanskrit Heritage Platform — <https://sanskrit.inria.fr/>
