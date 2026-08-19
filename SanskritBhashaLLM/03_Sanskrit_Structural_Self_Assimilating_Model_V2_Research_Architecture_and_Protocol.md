# Sanskrit Structural Self-Assimilating Foundation Model
## Version 2 Research Architecture and Controlled Experimental Protocol

**Working designation:** Sanskrit Structural Self-Assimilating Foundation Model, with a Pāṇinian grammatical core  
**Document version:** 2.0  
**Status:** Controlled research architecture and pre-registration framework  
**Date:** August 2026  
**Intended setting:** Institution-led, publicly funded, open-weight and open-research programme

---

# Document Purpose

This document converts the earlier proposal, strategy paper, self-assimilating-model brainstorming paper, and refactored gap analysis into an implementable research architecture and a controlled experimental protocol.

It is designed to answer one primary scientific question:

> **When information, data, model size, representation capacity, retrieval budget, and compute are controlled, does an executable multilayer Sanskrit structural representation improve knowledge acquisition, retrieval, propagation, exception handling, and update locality over information-equivalent universal linguistic, semantic-graph, generic procedural, learned-neural, vector-memory, and text-only baselines?**

The document is not yet a production-system specification. It defines:

- the bounded Version 1 Sanskrit structural stack;
- the target architecture and its invariants;
- the canonical concept, evidence, structural, confidence, and update representations;
- the controlled experimental conditions;
- the benchmark worlds, tasks, holdouts, metrics, and statistical plan;
- the stage gates that determine whether self-assimilation, dynamic routing, adapters, or larger-scale training should proceed;
- the institutional governance and open-release requirements.

The programme must be willing to falsify or narrow its central claim. It should not scale merely because the architecture is culturally significant or conceptually elegant.

---

# Executive Decision

The Version 2 programme adopts five decisions.

1. **The internal representation is not dhātu-centred.** Dhātus remain one important index, but the model uses a multilayer structural stack covering surface identity, phonology, Sandhi, inflection, derivation, compounds, event roles, sentence and discourse constraints, lexical senses, register, domain, rule scope, concepts, and evidence.

2. **Reality is not defined by Sanskrit morphology.** A language-independent canonical concept graph and evidence graph remain outside the Sanskrit structural stack. Sanskrit expressions align to concepts; they do not make concepts true.

3. **The first pilot excludes fast-weight and base-weight rewriting.** It tests structural analysis, multi-index retrieval, writable semantic memory, propagation, locality, ambiguity handling, and causal use with a frozen base model.

4. **The strongest novelty endpoint is propagation–locality.** The programme must demonstrate that the Sanskrit stack propagates a valid update farther across forms and meanings that should inherit it, while better protecting homonyms, lexicalized exceptions, unrelated roles, domains, registers, and unsupported claims.

5. **The full stack must face strong, information-equivalent controls.** Beating text-only or vector retrieval is insufficient. A strong novelty claim requires outperforming a universal linguistic stack and a generic executable grammar under matched conditions.

---

# Part I — Scientific Proposition

# 1. Research Thesis

The programme tests whether Sanskrit's explicit, multilayer organization can function as an executable inductive bias for foundation models.

The proposed structural stack provides more than labels. It contains:

- transformations between surface and canonical forms;
- paradigmatic relationships among inflections;
- procedural derivational histories;
- hierarchical compound structure;
- predicate-centred participant relations;
- sentence-level constraints and missing-role expectations;
- discourse and coreference links;
- lexicalized, domain-specific, historical, and idiomatic senses;
- scoped defaults, inheritance, exceptions, precedence, and optionality;
- alignment to language-independent concepts and externally warranted evidence.

The central hypothesis is not that every Sanskrit expression is semantically transparent. It is that explicit cross-layer constraints may reduce the search space for interpretation, create more reliable retrieval paths, and define more precise boundaries for knowledge inheritance and revision.

## 1.1 Core causal proposition

For an input expression or passage \(x\), the system constructs a set of candidate structural analyses:

\[
\mathcal{S}(x)=\{s_1,s_2,\ldots,s_n\}
\]

Each candidate may include surface, phonological, Sandhi, morphological, derivational, compound, event, discourse, sense, domain, and rule-scope information.

The system aligns these candidates with canonical concepts \(c\) and evidence \(e\):

\[
P(c,e\mid x,\mathcal{S}(x),d,t)
\]

where \(d\) is domain/register context and \(t\) is temporal context.

For a proposed knowledge update \(u\), the system predicts an update scope:

\[
\Omega(u)=g(\mathcal{S},c,e,d,t,r)
\]

where \(r\) includes inheritance, exception, precedence, and blocking relations.

The primary scientific claim is supported only if this Sanskrit-structured scope function produces a better propagation–locality trade-off than matched universal and procedural alternatives.

---

# 2. Primary, Secondary, and Exploratory Hypotheses

## 2.1 Primary hypothesis: propagation–locality

**H-P:** At a fixed non-target preservation level, the full Sanskrit structural stack achieves higher recall of required update consequences than the strongest information-equivalent baseline.

A practical primary endpoint is:

> **Propagation recall at or above 98% non-target preservation.**

The 98% threshold is provisional and must be confirmed during pilot pre-registration.

The primary null hypothesis is:

> The Sanskrit structural stack does not shift the propagation–locality Pareto frontier beyond the strongest universal linguistic or generic procedural baseline.

## 2.2 Secondary hypothesis: knowledge acquisition

**H-A:** Given identical evidence and exposure counts, the Sanskrit stack reaches a target level of concept understanding with fewer examples or a higher area under the learning curve.

The system must demonstrate more than definition recall. It must discriminate nearby concepts, solve a novel application, handle a related unseen form, and reject a morphologically plausible but unsupported interpretation.

## 2.3 Secondary hypothesis: multi-index retrieval

**H-R:** At a fixed retrieval, latency, token, and graph-operation budget, the Sanskrit stack retrieves the correct concept or evidence more reliably across surface, Sandhi, inflectional, derivational, compound, event-role, discourse, and cross-language variants.

## 2.4 Secondary hypothesis: ambiguity and calibration

**H-C:** The lattice-based Sanskrit representation improves calibrated uncertainty and selective accuracy when several segmentations, derivations, compound relations, senses, or discourse interpretations remain plausible.

## 2.5 Secondary hypothesis: causal use

**H-U:** Intervening on the structural representation produces predictable changes in retrieval, confidence, answer accuracy, and update scope, demonstrating that the model uses the structure causally rather than displaying it post hoc.

## 2.6 Exploratory hypothesis: external-query formation

**H-Q:** Cross-layer unsatisfied constraints and missing event roles generate more focused external retrieval queries than surface-query or generic semantic-decomposition baselines.

## 2.7 Exploratory hypothesis: efficiency

**H-E:** At matched answer quality, the structural stack reduces one or more of:

- retrieved context tokens;
- repeated external searches;
- KV-cache use;
- total inference FLOPs;
- latency;
- examples required for concept acquisition.

Efficiency is not assumed. Parser, graph, reconciliation, and storage costs must be counted end to end.

---

# 3. Scope, Attribution, and Version 1 Coverage Contract

## 3.1 Layered attribution

The project must not attribute every Sanskrit-related component directly to the Aṣṭādhyāyī. The architecture distinguishes:

| Layer | Primary intellectual or technical source |
|---|---|
| Pāṇinian grammatical core | Morphology, derivation, compounds, kāraka, rule organization |
| Śikṣā/Prātiśākhya-informed layer | Phonology, sound classes, accent and recitational features |
| Nirukta/lexicographic layer | Word senses, etymological proposals, conventional and attested meanings |
| Śābdabodha/verbal-cognition layer | Sentence expectancy, compatibility, connectedness, intended purport |
| Tantrayukti/discourse layer | Structured exposition, objection, response, example, conclusion and related discourse functions |
| Chandas/prosodic layer | Meter and prosodic constraints |
| Modern concept/evidence layer | Scientific definitions, equations, code, empirical evidence, time and provenance |

The working project name therefore uses **Sanskrit Structural** for the complete architecture and **Pāṇinian grammatical core** for its central grammatical component.

## 3.2 Included in Version 1

Version 1 covers Classical and contemporary prose with:

- Unicode and transliteration normalization;
- canonical phonological representation;
- selected varṇa and sound-class features;
- bidirectional Sandhi and segmentation candidates;
- subanta and tiṅanta features sufficient for the benchmark;
- kṛt, taddhita, selected sanādi and other pilot-relevant derivations;
- nested samāsa structure, vigraha candidates, and lexicalization flags;
- vibhakti-to-kāraka/event-role mapping;
- selected sentence constraints, including argument expectancy and compatibility;
- coreference and limited discourse links;
- lexical sense IDs, domain, register, period, and attestation status;
- defaults, exceptions, precedence, inherited scope, and optionality needed for the pilot;
- canonical concept and evidence records;
- multi-index retrieval and reversible memory transactions.

## 3.3 Explicitly deferred

The first pilot does not claim full support for:

- complete Vedic accent and morphology;
- recensional and oral-text variation;
- full Chandas coverage;
- kāvya and alaṅkāra modelling;
- complete śāstric discourse across traditions;
- manuscript restoration;
- multimodal recitation;
- unrestricted self-modifying weights;
- national-scale corpus or model training.

The architecture reserves extension points for these modules, but they require separate datasets, specialists, and validation.

## 3.4 Non-goals of the controlled pilot

The pilot does not attempt to prove that:

- Sanskrit is universally superior for every type of knowledge;
- the model literally thinks in Sanskrit;
- morphology alone provides scientific truth;
- a Sanskrit stack replaces external sources;
- the architecture eliminates hallucination;
- token or inference cost is automatically reduced by a fixed percentage;
- a single model should replace existing Sanskrit tools and projects.

---

# Part II — Version 2 Research Architecture

# 4. Architectural Invariants

The following requirements are non-negotiable.

1. **Concept independence:** canonical concepts exist independently of Sanskrit labels or derivations.
2. **Evidence separation:** structurally plausible meaning and empirically warranted truth remain separate.
3. **Alternative preservation:** ambiguous analyses remain live until evidence or context justifies commitment.
4. **Typed provenance:** every structural analysis, concept alignment, evidence claim, and update records its source, tool, version, confidence, and reviewer history.
5. **Reversible updates:** every persistent change is a transaction with explicit scope, dependencies, version, and rollback.
6. **Exception protection:** lexicalized, domain-specific, historical, idiomatic, and competing senses can block inheritance.
7. **Causal observability:** structural traces are not accepted as explanations until interventions show causal effect.
8. **External override:** evidence may reject or override an elegant structural interpretation.
9. **Controlled plasticity:** writable memory and routing are validated before temporary adapters; permanent weight consolidation is last.
10. **Open reproducibility:** schemas, code, model configurations, evaluation harnesses, and non-sensitive data are released under explicit licences.

---

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
             ANSWER + STRUCTURAL/CONCEPT/EVIDENCE TRACE
```

The layers are connected through typed edges and hyperedges. They are not forced into a single tree. Sandhi and derivational operations may be represented through transducers or state transitions, compounds through hypergraphs, events through multi-participant relations, and evidence through claim-level provenance links.

---

# 6. Module Specifications

## 6.1 Input and source-provenance module

### Responsibilities

- preserve original source bytes or text;
- record language, script, author, publication, date, location, licence, and retrieval method;
- separate user assertions, model-generated text, translated text, attested text, and institution-standardized text;
- attach cryptographic or content hashes where feasible;
- reject or quarantine unsupported executable instructions embedded in retrieved content.

### Required outputs

```text
SourceRecord
├── source_id
├── original_content
├── source_language
├── source_script
├── source_type
├── author/institution
├── publication_time
├── retrieval_time
├── licence
├── content_hash
├── generated/translated/attested/standardized status
└── trust and review state
```

## 6.2 Script, normalization, and phonology module

### Responsibilities

- Unicode normalization;
- transliteration conversion with provenance;
- canonical phonological representation;
- optional varṇa, place, manner, and pratyāhāra-class features;
- OCR and speech-noise hypotheses;
- cross-script identity mapping.

### Design rule

Script identity must not be confused with lexical identity. Several surface forms may resolve to one canonical lexical candidate, while visually or phonetically similar strings may remain separate.

## 6.3 Sandhi and segmentation lattice

### Responsibilities

- generate candidate word boundaries and unsandhied forms;
- preserve multiple valid candidates;
- score candidates using phonological validity, morphology, sentence compatibility, discourse, and context;
- prevent uncertain analyses from creating permanent knowledge updates;
- support backward dependency repair when a segmentation changes.

### Candidate object

```text
SegmentationCandidate
├── candidate_id
├── surface_span
├── boundary_sequence
├── canonical_forms
├── generating_rules/tools
├── local_score
├── cross-layer score
├── status: live / selected / rejected / unresolved
└── downstream_dependencies
```

## 6.4 Lexical identity and inflectional paradigm module

### Responsibilities

- distinguish lexeme, stem, lemma, and surface form;
- represent subanta and tiṅanta features;
- retain syncretic alternatives;
- link paradigm members;
- represent irregular or exceptional forms;
- define which lexical updates propagate through a paradigm.

### Pilot feature contract

At minimum, records must support:

- nominal stem, gender, case, and number;
- verbal root/stem, person, number, tense/mood category, voice, and pada where relevant;
- paradigm ID;
- ambiguity and confidence;
- source/tool/version.

## 6.5 Derivational process graph

### Responsibilities

- represent candidate derivational histories rather than only final decomposition;
- include upasarga, kṛt, taddhita, selected sanādi and pilot-relevant transformations;
- record rule applications, inherited context, exceptions, order, and intermediate states;
- distinguish derivational relation from current lexical meaning;
- permit multiple derivations to one surface form.

### Core distinction

```text
Derivationally suggested meaning
≠
Attested lexical sense
≠
Canonical concept
≠
Empirical truth
```

## 6.6 Compound hypergraph

### Responsibilities

- identify nested constituents;
- represent heads, modifiers, exocentric relations, and vigraha candidates;
- retain competing samāsa analyses;
- align compound candidates to lexical senses and concepts;
- mark lexicalized, technical, historical, and disputed compounds;
- define constituent-level and whole-compound update permissions.

### Required relation types

The exact ontology is to be developed with scholars, but the representation must support:

- constituent-of;
- semantic-head-of;
- modifier-of;
- candidate-vigraha;
- candidate-compound-type;
- lexicalized-as;
- expresses-concept;
- domain-restricted-as;
- inheritance-blocked-by.

## 6.7 Kāraka and event-role graph

### Responsibilities

- separate vibhakti realization from underlying participant relation;
- represent predicates, states, agents, affected entities, instruments, recipients, sources, locations, and other pilot-relevant roles;
- connect active, passive, nominalized, reordered, and partially omitted expressions describing the same event;
- generate missing-role and expectancy signals;
- map to a language-independent event representation.

## 6.8 Sentence-constraint module

### Responsibilities

- model unsatisfied argument expectancy;
- test semantic compatibility among candidate participants and predicates;
- retain multiple plausible dependency or interpretation structures;
- use connectedness and intended-purport signals where operationally defined;
- determine when a candidate interpretation is grammatically possible but semantically anomalous;
- generate targeted questions for missing relations.

This module must not pretend that philosophical concepts such as tātparya have already been completely formalized. Only explicitly defined computational approximations may enter the pilot.

## 6.9 Discourse and coreference module

### Responsibilities

- track entities and concepts across sentences;
- represent pronouns, ellipsis, quotation, attribution, cause, contrast, objection, answer, example, and conclusion for selected data;
- maintain topic continuity;
- prevent updates from propagating to nearby but non-coreferential entities;
- preserve unresolved discourse alternatives.

## 6.10 Lexical-sense, register, domain, and period module

### Responsibilities

- assign stable sense IDs;
- distinguish literal, conventional, domain, historical, metaphorical, idiomatic, and disputed senses;
- record corpus attestations and dictionary provenance;
- distinguish institution-approved terminology from historically attested usage;
- mark inheritance permissions and blocking conditions;
- bound updates by register, period, genre, domain, and jurisdiction where applicable.

## 6.11 Rule-scope engine

The rule-scope engine is a research hypothesis inspired by explicit grammatical organization, not a literal transplantation of the Aṣṭādhyāyī into neural learning.

### Required functions

- governing scope;
- inherited context;
- default and exception;
- precedence among applicable rules;
- optional alternatives;
- isolation of temporary or intermediate states;
- internal control metadata not emitted as surface text;
- explicit dependency and rollback links.

### Candidate mappings

| Grammatical mechanism | Candidate engineering role |
|---|---|
| Adhikāra | Scope governing a family of updates |
| Anuvṛtti | Inherited context shared across descendants |
| Utsarga–apavāda | Default with protected exception |
| Rule precedence | Conflict resolution among candidate updates |
| Optionality | Retention of multiple admissible analyses |
| It-marker | Internal control metadata |
| Asiddha-like isolation | Protection from premature cross-stage contamination |

These mappings must be evaluated against a generic executable rule engine with equivalent capabilities.

## 6.12 Canonical concept graph

The canonical concept graph is language-independent.

### Required content

```text
ConceptRecord
├── concept_id
├── type: entity / process / property / relation / event / proposition
├── definitions
├── formal relations
├── inputs and outputs
├── participant roles
├── equations or formal specifications
├── algorithms or code where applicable
├── examples and counterexamples
├── neighbouring and confusable concepts
├── multilingual labels
├── Sanskrit candidate labels and sense alignments
├── evidence links
├── domain / jurisdiction / temporal scope
└── version and review history
```

A concept may exist without an analyzable Sanskrit term. The record must support:

```text
atomic concept
+ external definition
+ optional Sanskrit label
+ derivation-insufficient status
```

## 6.13 Evidence and provenance graph

### Required content

- atomic claim;
- original source span;
- source identity and date;
- support, contradiction, and dependency relations;
- domain authority;
- temporal validity;
- source reliability and review state;
- generated, translated, attested, or standardized status;
- claim confidence;
- applicability boundaries;
- supersession history.

The evidence graph never treats model repetition as independent corroboration.

## 6.14 Cross-layer reconciliation module

### Responsibilities

- rank structural interpretations;
- align them to concepts;
- compare structural priors with attested usage and evidence;
- preserve disagreements;
- choose among confirm, refine, extend, override, fork, and quarantine outcomes;
- calculate proposed update scope;
- decide whether external retrieval or expert review is required.

### Reconciliation outcomes

| Outcome | Meaning |
|---|---|
| Confirm | Evidence supports the selected interpretation |
| Refine | Evidence narrows or specifies it |
| Extend | A new relation, domain, or sense is added |
| Override | Conventional or evidenced meaning supersedes a structural default |
| Fork | Separate senses, domains, periods, or schools are retained |
| Quarantine | Evidence or interpretation remains unreliable or unresolved |

## 6.15 Multi-index structural memory

The memory must be addressable through:

- surface and script variants;
- canonical phonological forms;
- Sandhi analyses;
- lexical identity;
- paradigm membership;
- derivational paths;
- compound constituents and hierarchy;
- event roles;
- sentence constraints;
- discourse referents;
- lexical senses;
- register/domain/period;
- canonical concepts;
- evidence claims.

The retrieval path must be logged. The system should distinguish a result found through surface similarity from one reached through a valid structural or semantic path.

## 6.16 Retrieval and response router

The router selects among:

1. **Internal structural mode** — analysis or retrieval from known structural and concept memory.
2. **External evidence mode** — current, empirical, high-stakes, or unsupported claims.
3. **Reconciliation mode** — morphology, usage, context, or sources conflict.
4. **Abstention/review mode** — uncertainty or disagreement exceeds policy thresholds.

The first pilot uses routing and memory selection but does not generate fast-weight adapters.

## 6.17 Reversible update transaction manager

Every persistent update follows:

```text
prepare
→ validate structure
→ validate concept alignment
→ validate evidence
→ predict scope
→ detect conflicts and protected boundaries
→ stage transaction
→ run regression and locality tests
→ commit or quarantine
→ version and audit
```

A transaction supports:

- add;
- correct;
- supersede;
- fork sense;
- create exception;
- restrict domain/register/time;
- retire terminology;
- rollback.

---

# 7. Typed Multilayer Representation

## 7.1 Representation form

The implementation may use a graph-plus-transducer architecture rather than one storage technology.

- phonological and Sandhi transformations may use finite-state or neural transducers;
- inflection and derivation may use typed process graphs;
- compounds may use hypergraphs;
- events may use predicate-centred multi-participant graphs;
- discourse may use relation graphs;
- rules may use scoped procedural objects;
- concepts and evidence may use versioned property graphs or equivalent stores.

The public interchange model must abstract over the underlying database.

## 7.2 Common node requirements

Every node must carry, where applicable:

```text
id
node_type
canonical_value
surface_value(s)
source
source_tool
source_tool_version
human_reviewer
confidence
status
register/domain/time
licence
created_version
superseded_by
```

## 7.3 Common relation requirements

Every relation must carry:

```text
relation_id
relation_type
source_node(s)
target_node(s)
applicability conditions
confidence
provenance
rule or evidence basis
inheritance permission
blocking exception
scope
version
```

## 7.4 Candidate-analysis bundle

```text
AnalysisBundle
├── input_span
├── script/phonological candidates
├── segmentation candidates
├── lexical and inflection candidates
├── derivational candidates
├── compound candidates
├── event/sentence candidates
├── discourse candidates
├── lexical-sense candidates
├── concept alignments
├── evidence links
├── layer confidence vector
├── unresolved conflicts
└── dependency graph
```

---

# 8. Confidence, Ambiguity, and Abstention

## 8.1 Internal confidence vector

The internal model maintains at least:

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

These values must be calibrated empirically. They must not be combined through an arbitrary average or product.

## 8.2 User-facing summary

For presentation, the system may aggregate to:

- **Formation confidence** — how the expression was structurally analyzed;
- **Meaning confidence** — which concept or interpretation is intended;
- **Warrant confidence** — how strongly evidence supports the factual claim.

## 8.3 Ambiguity-preserving outputs

The system supports:

- one selected analysis with alternatives;
- several live analyses without forced collapse;
- grammatical analysis without factual commitment;
- a concept answer with unresolved terminology;
- a domain- or register-restricted answer;
- explicit abstention and review request.

## 8.4 Retrieval and abstention triggers

External retrieval or review is triggered by combinations such as:

- low or divergent segmentation confidence;
- incompatible event structures;
- unresolved lexicalized versus literal meanings;
- evidence conflicts;
- temporally unstable facts;
- high-stakes domains;
- update scope crossing protected boundaries.

---

# 9. Assimilation Compiler and Intermediate Representations

The Assimilation Compiler converts external material into a reversible, structured memory proposal.

| Stage | Intermediate representation | Required output |
|---|---|---|
| IR-0 | SourceRecord | Original content, provenance, licence and status |
| IR-1 | NormalizedSource | Script/language normalization with reversible mapping |
| IR-2 | SourceSemanticIR | Source-faithful entities, events, relations and claims |
| IR-3 | ConceptAlignmentIR | Candidate canonical concepts and confidence |
| IR-4 | SanskritCandidateIR | Candidate Sanskrit labels, forms and attestation status |
| IR-5 | StructuralAnalysisIR | Sandhi, morphology, derivation, compounds, roles, discourse and senses |
| IR-6 | EvidenceAssessmentIR | Support, contradiction, reliability and temporal validity |
| IR-7 | ScopeProposalIR | Must-change, may-change and must-not-change predictions |
| IR-8 | MemoryTransactionIR | Reversible additions, modifications, forks, exceptions and rollback plan |

## 9.1 Information-loss requirement

Each stage must retain links to the prior stage. The Sanskrit representation must not replace or discard the source-language semantic representation.

## 9.2 Synthetic integrity requirement

Generated, translated, attested, and institution-standardized materials remain distinct. Generated usage cannot become independent evidence merely through repetition.

## 9.3 Conflict requirement

The compiler must preserve:

- competing segmentations;
- competing derivations;
- dictionary or school disagreement;
- domain-specific coexistence;
- historical versus modern meanings;
- evidence contradictions.

---

# 10. Layer-Wise Update-Scope Lattice

The update-scope lattice is the central object for continual-learning evaluation.

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
│   ├── active/passive/nominalized forms
│   ├── omitted-participant recovery
│   └── incompatible event structure
│
├── Discourse scope
│   ├── coreference
│   ├── ellipsis
│   ├── quotation attribution
│   └── nearby non-coreferential entity
│
├── Cross-language scope
│   ├── equivalent concept labels
│   ├── translation variants
│   └── non-equivalent lexical lookalikes
│
└── Protected boundaries
    ├── homonym
    ├── lexicalized or idiomatic sense
    ├── different domain
    ├── different register or period
    ├── competing school or terminology
    ├── historical usage
    ├── unsupported empirical claim
    └── quarantined evidence
```

Each scope edge records:

- affected property;
- typed relation;
- inheritance class;
- confidence;
- domain/register/time;
- evidence basis;
- blocking exception;
- rollback dependency.

---

# Part III — Controlled Experimental Protocol

# 11. Experimental Principle

The experiment must isolate the value of the representation rather than reward the Sanskrit condition for receiving more information, better annotations, more parameters, or more compute.

The shortest defensible comparison is:

```text
Same canonical concepts and evidence
Same Sanskrit input text
Same tokenizer
Same base model and frozen weights
Same graph-encoder parameter budget
Same memory capacity
Same retrieval budget
Same context-token budget
Same training examples
Same optimisation budget
Same update mechanism
Same evaluation items

Change only the structural representation and its permitted operations.
```

The first pilot therefore separates:

1. structural representation;
2. retrieval;
3. writable memory;
4. routing;
5. plastic adaptation.

Plastic adaptation is excluded until the first four demonstrate value.

---

# 12. Canonical World Model

All experimental conditions are compiled from one representation-neutral canonical world.

```text
CanonicalKnowledgeRecord
├── concept or claim ID
├── definition
├── type
├── participant and relation structure
├── formal properties
├── examples and counterexamples
├── evidence
├── update dependencies
├── must-change / may-change / must-not-change gold labels
└── domain, time and version
```

From each record, the project generates:

- the Sanskrit structural stack;
- the universal linguistic stack;
- the generic semantic graph;
- the generic executable grammar;
- the learned-neural structural condition;
- vector-memory records;
- text-only passages.

No condition receives facts or relations absent from the canonical record.

---

# 13. Evaluation Worlds

## 13.1 World W1 — Clean-room fictional knowledge

Purpose:

- prevent pretraining leakage;
- create exact gold propagation and locality scope;
- test acquisition from one or a few examples;
- include valid, invalid, ambiguous, and lexicalized-like constructions under controlled rules.

Content may include fictional:

- processes;
- instruments;
- substances;
- entities;
- event roles;
- causal relations;
- domain conventions;
- terminology updates.

The Sanskrit terms are independently constructed and reviewed, but all conditions receive the same canonical concept information.

## 13.2 World W2 — Engineered modern technical knowledge

Purpose:

- test practical scientific and technical relevance;
- connect terms to equations, algorithms, code, and formal definitions;
- assess terminology consistency and low-shot concept acquisition.

Initial domains should be selected for objective validation, for example:

- elementary algorithms and data structures;
- linear algebra;
- mechanics;
- elementary electronics or networking;
- formal logic.

The pilot should begin with two or three domains rather than broad STEM coverage.

## 13.3 World W3 — Attested natural Sanskrit

Purpose:

- test real ambiguity, syncretism, lexicalization, historical usage, register, and discourse;
- determine whether controlled gains survive natural material;
- expose tooling and annotation limitations.

The attested set must remain separate from Sanskritization data used to create engineered terminology.

## 13.4 Cross-cutting adversarial set

All worlds include:

- morphologically plausible but fictional claims;
- misleading Sandhi splits;
- homonyms;
- lexicalized compounds;
- domain conflicts;
- historical versus modern senses;
- contradictory sources;
- poisoned or prompt-injection-bearing retrieval content;
- unsupported but fluent explanations.

---

# 14. Pilot Dataset Targets

Exact sizes must be finalized after annotation-cost and statistical-power pilots. A reasonable first target is:

| Resource | Pilot target |
|---|---:|
| Clean-room canonical concepts | 120–180 |
| Modern technical concepts | 80–120 |
| Attested passages or examples | 600–1,000 |
| Inflectional paradigm probes | 500–800 |
| Derivational-family probes | 500–800 |
| Compound structures | 300–500 |
| Event-role and sentence paraphrases | 500–800 |
| Lexicalized/domain/register exceptions | 200–350 |
| Discourse/coreference probes | 200–350 |
| Controlled update events | 150–250 |
| Total evaluation probes | 5,000–10,000 |

The pilot is designed to estimate effect sizes and annotation reliability, not to establish final national-scale benchmarks.

---

# 15. Holdout Regimes

Random train/test splits are prohibited as the sole evaluation.

## 15.1 Surface and Sandhi holdouts

- unseen script or transliteration manifestation;
- unseen Sandhi environment;
- unseen boundary ambiguity;
- noisy OCR or speech-like variation.

## 15.2 Inflectional holdouts

- unseen paradigm cell;
- unseen irregular form;
- syncretic form requiring context;
- same ending on an unrelated lexeme.

## 15.3 Derivational holdouts

- unseen base-plus-operation combination;
- complete derivational-family holdout;
- unseen nominal-base derivation;
- competing derivational histories;
- root or stem introduced with minimal evidence at test time.

## 15.4 Compound holdouts

- unseen component combination;
- unseen nesting pattern;
- unseen compound relation;
- lexicalized exception;
- exocentric interpretation;
- context-dependent analysis.

## 15.5 Event and sentence holdouts

- unseen word order;
- active/passive transformation;
- nominalization;
- omitted argument;
- new role-equivalent paraphrase;
- same words with changed participant roles.

## 15.6 Discourse holdouts

- unseen coreference pattern;
- ellipsis;
- quotation and attribution;
- objection–response structure;
- nearby non-coreferential distractor.

## 15.7 Sense, register, and domain holdouts

- new domain-specific sense;
- historical versus modern meaning;
- philosophical versus scientific usage;
- idiom or metaphor;
- institution-standardized term versus historical attestation.

## 15.8 Evidence and update holdouts

- newly introduced fact;
- corrected fact;
- contradictory evidence;
- time-limited fact;
- unsupported but structurally plausible claim;
- update requiring a new exception or sense fork.

---

# 16. Experimental Conditions

# 16.1 Structural ladder

The Sanskrit structural conditions are cumulative:

```text
S0  Text only
S1  Script normalization + phonology + Sandhi lattice
S2  S1 + lexical identity + inflection
S3  S2 + derivational process graph
S4  S3 + compound hypergraph
S5  S4 + kāraka/event roles
S6  S5 + sentence constraints
S7  S6 + discourse/coreference
S8  S7 + rule scope/defaults/exceptions
S9  S8 + lexical senses/register/domain/evidence boundaries
SF  Complete Version 1 stack
```

The study also runs full-minus-one-layer ablations.

## 16.2 Strong baseline families

| Code | Baseline | Purpose |
|---|---|---|
| T | Text-only context | Tests whether explicit memory is needed |
| V | Flat vector memory | Tests whether similarity retrieval is sufficient |
| G | Generic semantic graph | Tests explicit conceptual relations |
| U | Universal linguistic stack | Tests explicit linguistic structure independent of Sanskrit organization |
| X | Generic executable grammar | Tests scoped rules, inheritance, defaults, exceptions, and precedence independent of Pāṇinian organization |
| N | Learned neural latent structure | Tests whether the model can learn equivalent organization without explicit symbolic input |
| CE | Controlled descriptive English | Tests whether transparent terminology alone creates the gain |
| ML | Another morphologically rich language or synthetic morphology | Tests general morphology versus Sanskrit-specific organization |

The exact CE and ML conditions may be introduced after the first pilot if resources are limited, but they are required before claiming Sanskrit-specific generality.

## 16.3 Sanskrit-specific negative controls

- **SF-Anonymized:** keep topology; replace relation labels with arbitrary IDs.
- **SF-Shuffled:** preserve graph size and degree distribution; rewire valid relations.
- **SF-Tree:** force one highest-scoring analysis.
- **SF-Lattice:** preserve alternatives and confidence.
- **SF-NoSandhi, NoInflection, NoDerivation, NoCompound, NoKāraka, NoSentence, NoDiscourse, NoRule, NoSense:** leave-one-layer-out variants.
- **Oracle-SF:** scholar-validated structure.
- **Predicted-SF:** automatically predicted structure.
- **Ensemble-SF:** combined tool/model candidates.
- **Noisy-SF:** calibrated corruption at multiple rates.

---

# 17. Capacity and Compute Equivalence

Each comparison must match or explicitly normalize:

- facts, definitions, examples, equations, code, and evidence;
- node, edge, hyperedge, and relation-vocabulary budgets;
- graph-encoder parameter count;
- adapter parameter count;
- retrieved-node and path budgets;
- context tokens passed to the language model;
- base-model architecture and parameter count;
- tokenizer and vocabulary;
- training examples and optimizer steps;
- training and inference FLOPs;
- parser and graph-construction cost;
- storage, memory, latency, and caching;
- number of external retrieval calls.

## 17.1 Information-equivalent compilation audit

An independent team reviews randomly sampled canonical records and all compiled representations to determine whether one condition contains extra information.

## 17.2 Capacity curves

Where strict equality is unnatural, report performance as a function of:

- graph capacity;
- retrieved nodes;
- context tokens;
- compute;
- latency.

This prevents one condition from winning only because it uses a larger representation.

---

# 18. Model and Training Phases

## Phase E0 — Representation and annotation pilot

No language-model integration.

Deliverables:

- canonical schema;
- structural interchange format;
- annotation manual;
- oracle structural records;
- generic and universal compilers;
- agreement and adjudication results.

## Phase E1 — Graph-only falsification

Use:

- symbolic traversal;
- graph retrieval;
- graph neural network or graph transformer with matched capacity.

Tasks:

- concept retrieval;
- affected-set prediction;
- exception blocking;
- scope classification;
- ambiguity ranking.

Purpose:

> Determine whether the topology and procedural organization contain useful signal before involving a foundation model.

## Phase E2 — Frozen language model with structural retrieval

Use one identical frozen base model for all conditions.

Train only:

- graph encoders;
- cross-attention or fusion adapters;
- retrieval/ranking layers;
- confidence heads.

No fast weights or base-model updates.

Purpose:

- isolate representation value;
- reduce confounding from full fine-tuning;
- test acquisition, retrieval, propagation, locality, and causal use.

## Phase E3 — Joint structural training

Proceed only if E1 or E2 shows reproducible signal.

Allow:

- joint token–structure alignment;
- auxiliary tasks for segmentation, inflection, derivation, compounds, roles, discourse, senses, and scope;
- cross-layer consistency objectives;
- concept and evidence alignment.

Purpose:

- determine whether joint training produces additional value beyond external structural retrieval.

## Phase E4 — Writable institutional semantic memory

Proceed only if SF improves the primary endpoint.

Add:

- reversible memory transactions;
- versioned concept/evidence updates;
- scope and exception application;
- rollback and replay;
- long sequences of updates.

The base model remains frozen.

## Phase E5 — Controlled plasticity

Proceed only after E4 demonstrates stable propagation, locality, rollback, and reproducibility.

Potential additions:

- scope-conditioned routing;
- temporary adapters;
- fast weights;
- rehearsal;
- reviewed model consolidation.

E5 requires a separate protocol. It is not part of the first pilot's success criteria.

---

# 19. Training Objectives

For joint-training phases, a candidate objective is:

\[
\mathcal{L}_{total}=
\mathcal{L}_{LM}
+\lambda_1\mathcal{L}_{normalization}
+\lambda_2\mathcal{L}_{segmentation}
+\lambda_3\mathcal{L}_{inflection}
+\lambda_4\mathcal{L}_{derivation}
+\lambda_5\mathcal{L}_{compound}
+\lambda_6\mathcal{L}_{event}
+\lambda_7\mathcal{L}_{sentence}
+\lambda_8\mathcal{L}_{discourse}
+\lambda_9\mathcal{L}_{sense}
+\lambda_{10}\mathcal{L}_{concept}
+\lambda_{11}\mathcal{L}_{evidence}
+\lambda_{12}\mathcal{L}_{scope}
+\lambda_{13}\mathcal{L}_{calibration}
+\lambda_{14}\mathcal{L}_{consistency}
\]

The first pilot should not optimize all terms simultaneously. The structural ladder determines which losses are enabled at each stage.

## 19.1 Cross-layer consistency examples

- selected Sandhi split must support selected lexical candidates;
- inflection must agree with sentence-role hypotheses;
- compound interpretation must align with the selected lexical sense;
- event structure must agree with canonical concept relations;
- evidence must not be treated as support outside its domain or temporal scope;
- an exception must block inherited updates where annotated.

---

# 20. Task Families and Metrics

# 20.1 Knowledge acquisition

Expose each new concept at:

\[
n\in\{1,2,4,8,16\}
\]

examples or evidence units.

Test:

- direct recall;
- paraphrase recognition;
- discrimination from confusable concepts;
- application to a new problem;
- recognition under unseen structural forms;
- transfer to related expressions;
- rejection of unsupported structural interpretations;
- cross-language application where included.

### Metrics

- accuracy and macro-F1;
- area under the learning curve;
- \(N_{80}\): examples required to reach 80% performance;
- calibration at each exposure level;
- performance per training example and per compute unit.

# 20.2 Multi-index retrieval

Queries include:

- exact and normalized surface form;
- transliteration;
- Sandhi manifestation;
- unseen inflection;
- unseen derivative;
- compound component or nested structure;
- event-role description;
- sentence paraphrase;
- discourse reference;
- domain description;
- English or other-language label;
- evidence request.

### Metrics

- Recall@1, @5, @10;
- Mean Reciprocal Rank;
- nDCG;
- path recall;
- downstream answer accuracy;
- retrieved tokens;
- graph operations;
- latency;
- cost per correct retrieval.

# 20.3 Propagation

For every update, annotate each related item:

```text
must change
may change
must not change
```

Evaluate propagation across:

- script and Sandhi variants;
- paradigms;
- derivatives;
- compounds;
- event-role paraphrases;
- discourse references;
- cross-language equivalents;
- downstream multi-hop consequences.

### Metrics

\[
\text{Propagation Precision}
=\frac{\text{correctly changed affected items}}{\text{all items changed}}
\]

\[
\text{Propagation Recall}
=\frac{\text{correctly changed affected items}}{\text{all items that should change}}
\]

Also report:

- propagation F1;
- performance by structural layer;
- performance by graph distance;
- multi-hop consequence accuracy;
- update latency and cost.

# 20.4 Locality

Hard negatives include:

- phonologically similar but unrelated forms;
- homonyms;
- unrelated stems sharing endings;
- non-inheriting derivatives;
- lexicalized compounds;
- idioms and metaphors;
- changed participant roles;
- nearby non-coreferential entities;
- different domains, registers, periods, schools, or jurisdictions;
- unsupported empirical claims.

### Metrics

- non-target preservation accuracy;
- false-positive update rate;
- output-distribution change on controls;
- unrelated benchmark retention;
- degradation after 10, 50, 100, and 250 sequential updates;
- rollback fidelity.

# 20.5 Primary propagation–locality endpoint

Plot the Pareto frontier:

```text
x-axis: false-positive update rate or 1 - locality

y-axis: propagation recall
```

A Sanskrit advantage requires:

- higher propagation at matched locality; or
- higher locality at matched propagation;
- replication across clean-room and at least one natural or technical world;
- survival against the universal linguistic and generic executable baselines.

# 20.6 Ambiguity and calibration

Tasks include:

- candidate segmentation coverage;
- compound and derivation ranking;
- sense selection;
- domain and register disambiguation;
- abstention when no candidate is sufficiently supported.

### Metrics

- top-k candidate coverage;
- Brier score;
- Expected Calibration Error;
- selective accuracy versus coverage;
- risk at fixed abstention rate;
- unresolved-alternative preservation;
- error propagation from early to later layers.

# 20.7 Causal use

Interventions include:

- remove one structural layer;
- corrupt a relation;
- replace one valid analysis with another;
- patch a graph state from another example;
- remove concept or evidence links;
- alter an exception or scope edge;
- preserve displayed explanation while changing internal routing, where technically feasible.

### Metrics

- change in answer accuracy;
- change in retrieval path;
- change in confidence;
- change in update scope;
- causal sensitivity and specificity;
- agreement between displayed trace and actual retrieval/routing logs.

# 20.8 Efficiency

Measure end to end:

- input and output tokens;
- retrieved context tokens;
- graph-construction time;
- graph-retrieval operations;
- parser/transducer compute;
- base-model FLOPs;
- latency;
- peak memory;
- persistent storage;
- examples required per learned concept;
- cost per correct answer or correct update.

No efficiency claim may ignore the cost of producing and maintaining the structural representation.

---

# 21. Oracle, Predicted, Ensemble, and Noisy Structure

The protocol separates linguistic theory from tooling quality.

| Condition | Meaning |
|---|---|
| Oracle | Scholar-validated structural analysis |
| Rule-generated | Output from deterministic or procedural tools |
| Neural-predicted | Output from learned analyzers |
| Ensemble | Multiple tools and models with confidence and provenance |
| Noisy | Controlled corruption of nodes, edges, labels, or confidence |

## 21.1 Interpretation rules

- **Oracle succeeds, predicted fails:** the structural thesis may be sound; tooling is the bottleneck.
- **Oracle fails:** the central representational claim is weakened.
- **Lattice succeeds, tree fails:** uncertainty preservation is necessary.
- **Shuffled matches full:** genuine structural organization is not responsible for the gain.
- **Anonymized matches labelled:** topology, rather than traditional labels, may drive performance.
- **Performance collapses under modest noise:** deployment feasibility is weak even if the oracle result is positive.

---

# 22. Statistical Analysis Plan

## 22.1 Pre-registration

Before final training, publish:

- primary and secondary hypotheses;
- primary endpoint;
- conditions and ablations;
- exclusion criteria;
- seed count;
- sample-size and power assumptions;
- stopping rules;
- correction for multiple comparisons;
- handling of missing or disputed annotations.

## 22.2 Random seeds

Use at least five independent seeds per pilot condition. Increase the number if seed variance is large.

## 22.3 Paired evaluation

All conditions are evaluated on the same examples and update events.

## 22.4 Confidence intervals

Report:

- 95% bootstrap confidence intervals;
- seed-level variance;
- concept-family-level variance;
- domain and register variance;
- oracle/predicted variance.

## 22.5 Mixed-effects analysis

Where appropriate, model:

- representation condition as a fixed effect;
- concept family, structural family, domain, register, and seed as random effects.

This tests whether gains generalize rather than being driven by a few roots, compounds, or terminology families.

## 22.6 Multiple comparisons

Pre-designate:

- one primary comparison: SF versus the strongest matched U/X baseline on the propagation–locality endpoint;
- a limited set of secondary comparisons;
- an explicit correction method for exploratory ablations.

## 22.7 Hidden test set

An independent evaluation team holds the final natural and technical test sets. The development team sees only the schema and task specification.

## 22.8 External replication

Before a national-scale claim, at least one external institution should reproduce the main result from released code and a sealed or subsequently released benchmark.

---

# 23. Provisional Go/No-Go Criteria

Thresholds are provisional and must be finalized after the pilot power study.

## Gate G0 — Representation readiness

Proceed to E1 only if:

- the Version 1 schema is complete;
- experts reach acceptable agreement or documented disagreement on the pilot layers;
- generic and universal compilers pass information-equivalence audit;
- every record has provenance and licensing status;
- synthetic and attested data remain separable.

## Gate G1 — Structural signal

Proceed to frozen-LM integration if one or more graph-only tasks show a reproducible advantage over text/vector and the result is not reproduced by shuffled topology.

## Gate G2 — Controlled model value

Proceed to joint training only if SF or a substantial subset:

- improves propagation recall by at least five absolute points at the pre-registered locality threshold; or
- reduces concept exposures by approximately 20% at matched target performance; or
- improves Recall@5 by at least five absolute points at matched retrieval budget;
- and does not materially worsen calibration or cost per correct result.

At least one effect must reproduce in W2 or W3, not only W1.

## Gate G3 — Sanskrit-specific structural value

A strong Sanskrit/Pāṇinian novelty claim requires:

- SF to outperform the information-equivalent universal linguistic stack;
- SF to outperform or shift the Pareto frontier beyond the generic executable grammar;
- gains to survive controlled English or another structured-language comparison when introduced;
- full-minus-layer and negative controls to identify responsible mechanisms.

If SF only beats text/vector, narrow the claim to explicit structure generally.

## Gate G4 — Tooling feasibility

Proceed to writable institutional memory only if predicted or ensemble structure preserves a substantial proportion of oracle benefit. A provisional target is at least 70% of the oracle improvement, subject to task and cost analysis.

## Gate G5 — Controlled self-assimilation

Proceed to dynamic routing or adapters only if:

- 100 or more sequential memory updates retain the pre-registered locality threshold;
- rollback restores the prior state within tolerance;
- update conflicts and exceptions remain auditable;
- reproducibility is maintained across instances;
- cost remains within the agreed deployment envelope.

## Gate G6 — Scale

Consider larger models or corpus expansion only if:

- the central result reproduces across two backbones;
- the gain survives natural Sanskrit;
- information and compute audits confirm fairness;
- the benefit is not explained solely by curated descriptive terminology;
- an external group reproduces the main endpoint;
- an independent board recommends scale-up.

---

# 24. Mandatory Stop or Narrowing Conditions

The programme must narrow or stop the architectural claim if:

- the universal linguistic stack matches SF on the primary endpoint;
- a generic executable grammar matches propagation and locality;
- shuffled or random topology matches the authentic structure;
- gains vanish under family, sense, discourse, domain, or register holdouts;
- gains appear only for engineered terms;
- attested natural Sanskrit fails to reproduce controlled gains;
- predicted analyses erase oracle gains without a credible tool-improvement path;
- structure improves propagation only by damaging locality;
- graph and parser costs outweigh meaningful gains;
- displayed traces are not causally related to model behaviour;
- synthetic Sanskritization becomes the primary source of its own validation.

A negative result should still produce reusable datasets, schemas, tools, and benchmarks.

---

# 25. Result-Interpretation Matrix

| Result | Interpretation | Programme action |
|---|---|---|
| SF beats text/vector only | Explicit structure helps; Sanskrit-specific novelty is unproven | Preserve structural tools; narrow claim |
| SF matches U | Linguistic structure generally explains the gain | Reframe as universal structured-language research |
| SF matches X | Procedural scope/default/exception machinery explains the gain | Treat Sanskrit as a rich implementation, not unique mechanism |
| Oracle wins; predicted fails | Theory may be valid; tools are inadequate | Invest selectively in analyzers and annotation |
| Engineered terms win; natural data fails | Terminology design or curation drives performance | Narrow to technical-terminology programme |
| Acquisition improves; propagation/locality does not | Useful low-shot lexical/concept learning | Do not claim continual-learning breakthrough |
| Retrieval improves; update scope does not | Useful retrieval architecture | Defer self-assimilation and rewriting |
| Propagation improves; locality falls | Inheritance is too aggressive | Improve exceptions and scope; do not scale |
| SF-Lattice beats SF-Tree | Preserving ambiguity is necessary | Make lattice architecture mandatory |
| Full stack wins across W1–W3 | Strong support for the structural thesis | Proceed to writable memory and replication |
| Full stack shifts propagation–locality beyond U and X | Strong support for new foundation-model principle | Prepare larger open research programme |
| Costs dominate gains | Scientific signal may remain, but efficiency claim fails | Retain research outputs; avoid deployment claim |

---

# Part IV — Data, Governance, Engineering, and Open Research

# 26. Annotation and Interoperability Schema

A shared annotation record must contain:

```text
record_id
source and source-language content
script and normalization provenance
phonological form
Sandhi and segmentation candidates
canonical lexical forms
inflectional features and paradigm IDs
derivational candidates and rule traces
compound hierarchy and vigraha candidates
kāraka/event graph
sentence and discourse structures
lexical sense IDs
register/domain/period/genre
canonical concept IDs
evidence and contradiction links
update-scope labels
layer confidence vector
source tool and version
reviewer and adjudication history
licence and release status
```

## 26.1 Tool adapters

Existing tools remain authoritative in their domains where appropriate. Each adapter converts tool-specific output into the common schema and records:

- source tool;
- version;
- confidence or ranking;
- original output;
- conversion rule;
- unresolved fields;
- human corrections.

## 26.2 No silent normalization

All conversions must be reversible or preserve the original representation.

---

# 27. Expert Governance

No single category called “Sanskrit expert” is sufficient.

## 27.1 Required working groups

1. Representation standards and interoperability.
2. Pāṇinian grammar and derivation.
3. Phonology, script, and Vedic/historical extensions.
4. Lexicography, senses, and dictionaries.
5. Sentence semantics, kāraka, and verbal cognition.
6. Discourse and śāstric organization.
7. Modern terminology and domain science.
8. Evidence, provenance, and source quality.
9. Computational architecture and infrastructure.
10. Evaluation, statistics, and independent replication.
11. Safety, poisoning, privacy, licensing, and public release.

## 27.2 Adjudication

The project must publish:

- annotation manuals;
- inter-annotator agreement;
- disagreement taxonomies;
- adjudication policies;
- minority or alternative analyses;
- institution-approved versus historically attested distinctions;
- correction and version history.

## 27.3 Independence

The benchmark team and final evaluation team should be institutionally separate from the main model-development team where practical.

---

# 28. Error Containment and Scaling

## 28.1 Cascade containment

An early error may propagate:

```text
wrong normalization
→ wrong segmentation
→ wrong lexeme
→ wrong derivation or compound
→ wrong event role
→ wrong concept
→ wrong update
```

Controls include:

- alternative-path preservation;
- delayed commitment;
- layer confidence thresholds;
- cross-layer consistency checks;
- evidence checks;
- dependency-tracked rollback;
- quarantine for low-confidence persistent updates.

## 28.2 Growth controls

Use:

- bounded candidate beams;
- sparse hypergraphs;
- retrieval-depth limits;
- caching and memoization;
- hot versus archival memory;
- approximate indexes;
- graph versioning;
- offline analysis for expensive operations;
- explicit latency and storage budgets.

## 28.3 Reproducibility record

Every output in research mode records:

- base-model version;
- structural-memory version;
- concept/evidence-memory version;
- active condition and ablations;
- retrieved nodes and paths;
- source evidence;
- session state;
- random seed where relevant.

---

# 29. Security and Synthetic-Integrity Controls

The system must defend against:

- prompt injection in retrieved material;
- fabricated citations;
- false grammatical authority;
- politically or institutionally motivated sense collapse;
- model-generated terminology treated as independent attestation;
- poisoned examples;
- silent domain or temporal leakage;
- repeated updates causing drift.

## 29.1 Evidence quarantine

```text
external claim
→ quarantine
→ provenance and source validation
→ contradiction search
→ domain review
→ scope review
→ provisional memory
→ validated institutional memory
```

## 29.2 Synthetic status

Every usage is labelled as one of:

- attested;
- translated;
- model-generated;
- expert-proposed;
- institution-standardized;
- disputed;
- deprecated.

Frequency of generated usage cannot be treated as evidence of established meaning.

---

# 30. Open-Research Release Policy

The programme should release, subject to rights and safety constraints:

- representation and interchange schemas;
- annotation guidelines;
- structural compilers and tool adapters;
- canonical concept and evidence schemas;
- graph and retrieval code;
- benchmark generation code;
- training and evaluation harnesses;
- open model weights and checkpoints for completed stages;
- model and data cards;
- compute and cost reports;
- ablation and negative results;
- governance and adjudication procedures;
- final benchmark after the sealed evaluation period.

“Open weight” alone is not sufficient. Reproducible research requires the architecture, data lineage, protocol, and evaluation system.

---

# Part V — Work Packages and Decision Gates

# 31. Indicative Work Plan

The schedule is illustrative and should be revised after staffing and resource assessment.

| Work package | Indicative period | Principal deliverables | Gate |
|---|---:|---|---|
| WP0 — Scope, attribution, governance | Months 0–3 | Coverage contract, boards, licences, pre-registration outline | G0 |
| WP1 — Canonical and interchange schemas | Months 1–6 | Concept, evidence, structural, confidence and transaction schemas | G0 |
| WP2 — Annotation pilot and compilers | Months 3–10 | Oracle records, tool adapters, U/G/X baselines, agreement report | G0 |
| WP3 — Benchmark worlds | Months 5–14 | W1, W2, W3 datasets, holdouts, hidden test protocol | G1 |
| WP4 — Graph-only experiments | Months 9–16 | E1 results, topology controls, scope prediction | G1 |
| WP5 — Frozen-model experiments | Months 13–22 | E2 structural ladder, acquisition/retrieval/propagation/locality | G2/G3 |
| WP6 — Joint structural training | Months 20–30 | E3 results, causal interventions, two-backbone validation | G3/G4 |
| WP7 — Writable institutional memory | Months 26–36 | E4 sequential updates, rollback, audit and replication | G5 |
| WP8 — Controlled plasticity research | After G5 | Separate protocol for adapters and consolidation | G6 |
| WP9 — Specialist Sanskrit expansion | Parallel after core validation | Vedic, Chandas, kāvya, discourse and manuscript modules | Separate gates |

---

# 32. Required Deliverables

## 32.1 Scientific deliverables

- pre-registered controlled experiment;
- propagation–locality benchmark;
- acquisition and multi-index retrieval benchmarks;
- oracle/predicted/noisy structural evaluation;
- strong universal and procedural baselines;
- causal-intervention results;
- statistical and cost analysis;
- negative-result report where applicable.

## 32.2 Infrastructure deliverables

- open Sanskrit Structural Interchange Format;
- canonical concept/evidence model;
- multi-index structural memory reference implementation;
- rule-scope and update-scope representations;
- reversible memory transaction system;
- tool adapters;
- annotation and adjudication platform.

## 32.3 Institutional deliverables

- open governance charter;
- expert-consortium agreements;
- terminology and evidence review workflow;
- version and rollback policy;
- licensing and public-release policy;
- external replication agreement.

---

# 33. Requirements Traceability to the Refactored Gap Analysis

| Gap family | Version 2 response |
|---|---|
| FG-01 Scope and attribution | Sections 3 and 27 define layered attribution, bounded coverage, and governance |
| FG-02 Script, phonology and Sandhi | Sections 6.1–6.3 and 15.1 define canonical identity, lattices, and holdouts |
| FG-03 Inflection, derivation, compounds and senses | Sections 6.4–6.6, 6.10 and 15.2–15.4 define separate structures and tests |
| FG-04 Event, sentence, discourse and register | Sections 6.7–6.10 and 15.5–15.7 define event/discourse scope and boundaries |
| FG-05 Executable rules and representation | Sections 6.11–7 define typed graph/transducer architecture and rule scope |
| FG-06 Assimilation, memory and update scope | Sections 6.14–6.17, 9 and 10 define compiler IRs, memory, and transactions |
| FG-07 Confidence and ambiguity | Section 8 and task 20.6 define layer-level calibration and abstention |
| FG-08 Data, annotation and synthetic integrity | Sections 26, 27 and 29 define schema, adjudication and safeguards |
| FG-09 Experimental controls | Sections 11–25 define worlds, baselines, equivalence, metrics and stopping rules |
| FG-10 Plasticity | Sections 18 and 23 defer adapters until structural and memory gates pass |
| FG-11 Error, scale, interoperability and causality | Sections 7, 20.7, 26 and 28 define containment, standards and interventions |
| FG-12 Governance, uniqueness and falsification | Sections 22–25, 27 and 31 define governance, claims and stop conditions |

---

# 34. Defensible Version 2 Uniqueness Statement

> **This programme tests whether an executable multilayer Sanskrit structural representation—spanning phonological transformation, Sandhi, inflection, derivation, compound hierarchy, predicate-centred event roles, sentence and discourse constraints, lexicalized meaning, register, and explicit rule scope—can causally improve knowledge acquisition, multi-index retrieval, propagation, exception handling, and update locality over information-equivalent universal linguistic, semantic-graph, generic procedural, learned-neural, vector-memory, and text-only baselines.**

The project does not claim that each component is individually new. Its proposed contribution is the controlled demonstration—or falsification—of the complete structural principle.

---

# 35. Final Decision Rule

The programme earns the right to proceed toward a self-assimilating open-weight foundation model only if:

1. the Sanskrit stack shifts the propagation–locality frontier beyond strong matched baselines;
2. the result survives clean-room, technical, and attested evaluations;
3. predicted or ensemble structure retains enough oracle benefit to be feasible;
4. causal interventions confirm that the model uses the structure;
5. cost and latency remain proportionate to the gain;
6. an independent team reproduces the principal result.

A positive result would support a broader foundation-model principle:

> **A formally organized natural language can provide an executable system not only for representing expressions, but for constraining interpretation, generating alternatives, defining inheritance, preserving exceptions, retrieving evidence, and controlling where knowledge updates should and should not propagate.**

A negative result would still yield valuable open resources, but the institution should not scale the architecture or present Sanskrit structure as a superior continual-learning substrate.

---

# Appendix A — Minimum Pilot Readiness Checklist

- [ ] Version 1 coverage contract approved.
- [ ] Layered attribution approved.
- [ ] Canonical concept and evidence schemas frozen for the pilot.
- [ ] Structural interchange schema versioned.
- [ ] Annotation manual published.
- [ ] Expert groups and adjudication workflow operating.
- [ ] Synthetic, translated, attested, and standardized data separated.
- [ ] W1, W2, and W3 pilot sets built.
- [ ] Hidden test governance established.
- [ ] Universal linguistic and generic executable baselines implemented.
- [ ] Information-equivalence audit completed.
- [ ] Compute and capacity budgets pre-registered.
- [ ] Structural ladder and negative controls implemented.
- [ ] Oracle, predicted, ensemble, and noisy structures available.
- [ ] Propagation–locality endpoint and thresholds pre-registered.
- [ ] Causal interventions implemented.
- [ ] Rollback and audit logs tested for E4.
- [ ] Open-release and licensing review completed.
- [ ] Independent replication partner identified.

---

# Appendix B — Example Update Event

```text
Update ID: U-017
Canonical concept: C-042
Update type: domain-specific correction
Claim: In domain D, process P operates on vectors rather than scalars.
Evidence: E-220, E-221
Temporal scope: current
Domain: D

Must change:
- canonical definition of C-042 in D
- approved Sanskrit domain sense S-042-D
- inflectional forms referring to S-042-D
- inheriting derivatives whose argument type is inherited
- compound occurrences whose whole meaning depends on S-042-D
- role-equivalent event paraphrases
- genuine discourse references

May change:
- rate and instrument terms whose definitions depend on input type
- cross-language explanatory examples

Must not change:
- historical scalar usage
- unrelated domain D2
- lexicalized compound L-19
- homonymous stem H-4
- metaphorical use M-7
- unsupported claim that all related processes use vectors

Rollback dependency:
- restore prior concept version
- restore affected examples
- invalidate derived cache entries
- preserve the retracted evidence and audit trail
```

---

# Appendix C — Example Layer Confidence Record

```text
C_script             = 1.00
C_phonology          = 0.98
C_sandhi             = 0.72
C_lexical_identity   = 0.81
C_inflection         = 0.94
C_derivation         = 0.67
C_compound           = 0.61
C_karaka_event       = 0.88
C_sentence           = 0.84
C_discourse          = 0.79
C_lexical_sense      = 0.58
C_register_domain    = 0.91
C_concept_alignment  = 0.76
C_evidence           = 0.97
C_temporal_validity  = 0.95
C_source_reliability = 0.93
C_update_scope       = 0.69

Decision:
- preserve two compound/sense analyses;
- retrieve targeted domain evidence;
- answer with preferred interpretation and alternative;
- prohibit persistent update until scope confidence exceeds threshold.
```

---

# Appendix D — Source Basis

This Version 2 document synthesizes and operationalizes:

1. `Sanskrit_Native_LLM_Proposal(1).md`
2. `Paninian_Grounded_Foundation_Model_Strategy.md`
3. `Paninian_Self_Assimilating_Model.md`
4. `Paninian_Self_Assimilating_Model_Gap_Analysis_Refactored_v2.md`

The earlier documents remain vision, strategy, brainstorming, and gap-analysis sources. This document supersedes them only for the research architecture and controlled experimental protocol.

---

# Appendix E — Selected Evidence Base from the Source Documents

- Amrith Krishna et al., **Word Segmentation in Sanskrit Using Path Constrained Random Walks** — https://aclanthology.org/C16-1048/
- Jivnesh Sandhan et al., **DepNeCTI: Dependency-based Nested Compound Type Identification for Sanskrit** — https://aclanthology.org/2023.findings-emnlp.914/
- Amba Kulkarni et al., **Dependency Relations for Sanskrit Parsing and Treebank** — https://aclanthology.org/2020.tlt-1.12/
- Harshad Ayachit et al., **Computational Modelling of the Apatyādhikāra in Aṣṭādhyāyī** — https://aclanthology.org/2026.iscls-1.16/
- Tapas Khanra et al., **TantraTagger** — https://aclanthology.org/2026.iscls-1.4/
- Sriram Krishnan et al., **Challenges in Processing Vedic Sanskrit** — https://aclanthology.org/2025.wsc-csdh.9/
- Anagha Pradeep et al., **Towards Building a Computational Sense Inventory from the Monier-Williams Dictionary** — https://aclanthology.org/2026.iscls-1.3/
- Lewis et al., **Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks** — https://arxiv.org/abs/2005.11401
- Mitchell et al., **Memory-Based Model Editing at Scale** — https://proceedings.mlr.press/v162/mitchell22a.html
- Asai et al., **Self-RAG** — https://openreview.net/forum?id=hSyW5go0v8

