# Refactored Gap Analysis of the Pāṇinian Self-Assimilating Foundation Model

## From a Dhātu-Centred Design to a Full Sanskrit Structural Stack

**Document reviewed:** `Paninian_Self_Assimilating_Model.md`  
**Source gap analysis:** `Paninian_Self_Assimilating_Model_Gap_Analysis.md`  
**Purpose:** Remove repetition while preserving every substantive gap and making the analysis directly usable for a Version 2 architecture and research protocol.  
**Status:** Refactored research gap analysis; not yet an architecture specification.  
**Date:** August 2026

---

# Executive Assessment

The self-assimilating-model concept retains a strong core:

- internal structure generates hypotheses;
- external evidence grounds, refines, or corrects them;
- adaptation is reversible and governed;
- linguistic plausibility, intended meaning, and empirical support remain distinct;
- provenance, contradiction, rollback, and institutional consolidation are architectural requirements.

The central correction is that the internal structure cannot remain principally **dhātu-addressed**. It must become a typed, uncertainty-aware Sanskrit structural stack:

```text
script and phonology
→ Sandhi and segmentation
→ lexical form and inflection
→ derivation
→ compound hierarchy
→ kāraka and event structure
→ sentence and discourse constraints
→ lexical sense, register, and domain
→ rule scope, inheritance, and exception
→ canonical concept and evidence
```

The scientific thesis therefore changes from **dhātu-addressed self-assimilation** to:

> **Cross-layer constraint intersection and update control over an executable Sanskrit structural stack, aligned to a language-independent concept and evidence layer.**

This expanded thesis is stronger, but harder to prove. A full Sanskrit stack cannot be compared only with a generic semantic graph; it must face information-equivalent universal linguistic, semantic, procedural, learned-neural, vector-memory, and text-only controls.

## Refactoring outcome

The original 47-gap register repeated the same issues in its summary table, detailed analysis, section-impact table, and remediation plan. This version consolidates all 47 gaps into **12 gap families**, each treated once. The legacy IDs remain in a crosswalk for traceability.

---

# 1. Principles to Preserve

| Principle | Decision |
|---|---|
| Intensional prior versus referential grounding | Retain. Structure may suggest meaning; external evidence establishes real-world claims. |
| Explicit memory beside model weights | Retain. Parametric knowledge is not a clean structural database. |
| Reconfiguration before permanent rewriting | Retain. Retrieval and writable memory precede adapters and weight consolidation. |
| Two-way correction | Retain. Evidence may override literal derivation or introduce atomic concepts. |
| Provenance and contradiction | Retain. Every assimilated claim needs source, time, reliability, and review state. |
| Multi-speed learning | Retain. Token-, session-, institutional-, and release-time learning remain useful. |
| Explicit failure modes | Retain and expand. Etymological fallacy, self-confirmation, poisoning, drift, and reproducibility remain central. |

---

# 2. Consolidated Gap Map

**Severity:** **Critical** affects the validity of the central claim or experiment; **High** threatens natural-language robustness or implementation; **Later-specialist** is deliberately deferred from the first pilot.

| ID | Gap family | Legacy gaps | Severity | Core correction |
|---|---|---|---:|---|
| **FG-01** | Scope, attribution, and bounded coverage | G-01–G-03 | Critical | Define module origins, replace the root-only address, and bound Version 1. |
| **FG-02** | Script, phonology, Sandhi, and surface identity | G-04–G-05 | Critical | Add canonical forms and a probabilistic Sandhi/segmentation lattice. |
| **FG-03** | Inflection, derivation, compounds, and lexical sense | G-06–G-08, G-11 | Critical | Separate paradigms, derivational processes, compound structure, and conventional senses. |
| **FG-04** | Event structure, sentence interpretation, discourse, and register | G-09–G-15 | Critical / Later-specialist | Add kāraka–vibhakti mapping, sentence/discourse constraints, register boundaries, and staged specialist modules. |
| **FG-05** | Executable rules and structural representation | G-16–G-19 | Critical | Use a typed multilayer representation, rule graph, canonical concept layer, and multi-index retrieval. |
| **FG-06** | Assimilation, memory, inheritance, and update scope | G-20–G-24 | Critical | Compile external evidence across layers and express updates as reversible scope transactions. |
| **FG-07** | Confidence, ambiguity, and response policy | G-25–G-27 | High | Calibrate uncertainty by layer and preserve unresolved alternatives. |
| **FG-08** | Data, annotation, expert review, and synthetic integrity | G-28–G-30 | Critical | Publish a common schema, adjudication model, and safeguards against self-generated evidence loops. |
| **FG-09** | Experimental controls and novelty measurement | G-31–G-38 | Critical | Separate structure from retrieval, memory, plasticity, information, and compute. |
| **FG-10** | Plasticity and dynamic rewiring | G-39–G-40 | High | Defer fast weights and specify scope-controlled adaptation before implementation. |
| **FG-11** | Error containment, scale, interoperability, and causal observability | G-41–G-44 | Critical | Contain cascades, bound graph growth, standardize tool outputs, and test causal use. |
| **FG-12** | Governance, uniqueness, and falsification | G-45–G-47 | Critical | Align expert governance with the stack and pre-register a narrow novelty claim and stopping rules. |

---

# 3. Consolidated Gap Analysis

## FG-01 — Scope, Attribution, and Bounded Coverage

**Legacy gaps:** G-01–G-03

### Gap

“Pāṇinian” currently covers a wider set of ideas than the Aṣṭādhyāyī alone, while “dhātu-addressed memory” covers too little of Sanskrit. The architecture also lacks a bounded meaning of “all elements of Sanskrit.”

Relevant sources should be distinguished:

```text
Pāṇinian grammatical core
Śikṣā/Prātiśākhya phonology and accent
Nirukta and lexicographic sense analysis
Śābdabodha and verbal-cognition constraints
Tantrayukti and discourse organization
Chandas and prosodic structure
modern concept and evidence governance
```

Many valid addresses do not begin with a dhātu: nominal stems, indeclinables, inflections, compounds, event roles, lexicalized senses, discourse references, atomic concepts, and conventional terminology.

### Required Remediation

- Define a layered attribution model.
- Consider **Sanskrit Structural Self-Assimilating Foundation Model**, with a Pāṇinian grammatical core, as the broader name.
- Replace one primary root address with a **multi-index structural address system**.
- Publish a Version 1 coverage contract:
  - Classical and contemporary prose first;
  - phonology, Sandhi, morphology, compounds, kāraka, lexical sense, selected sentence/discourse relations, domain, and register included;
  - Vedic accent, Chandas, kāvya, alaṅkāra, and expanded śāstric discourse treated as specialist modules.

---

## FG-02 — Script, Phonology, Sandhi, and Surface Identity

**Legacy gaps:** G-04–G-05

### Gap

The architecture does not define identity across scripts, transliteration, Unicode variation, OCR or speech noise, phonological alternation, and Sandhi. Sandhi is mentioned but not represented as a bidirectional probabilistic lattice.

### Consequences

- one lexeme can fragment into several memory entries;
- cross-script retrieval becomes unreliable;
- a premature split can corrupt all downstream analyses;
- plausible and intended segmentations are not distinguished.

### Required Remediation

```text
surface text and source script
→ Unicode/transliteration normalization
→ canonical phonological form
→ candidate Sandhi boundaries
→ candidate lexical forms
→ morphological and sentence compatibility
→ contextual ranking
```

Store varṇa/sound-class features where useful, script provenance, alternative paths, confidence, and links from surface variants to canonical lexical and concept records. Uncertain splits must not create permanent updates.

---

## FG-03 — Inflection, Derivation, Compounds, and Lexical Sense

**Legacy gaps:** G-06–G-08, G-11

### Gap

Four different mechanisms are currently compressed into a general derivational memory:

1. **Inflection:** subanta and tiṅanta paradigms, syncretism, irregularity, and ambiguity.
2. **Derivation:** kṛt, taddhita, sanādi, causative, desiderative, intensive, feminine, and nominal-base formations, including alternative derivations.
3. **Samāsa:** nested constituents, head structure, vigraha, competing relations, exocentricity, and context.
4. **Lexical sense:** literal, conventional, domain, historical, metaphorical, idiomatic, and disputed meanings.

### Consequences

The model cannot determine whether an update should move across an inflectional paradigm, a semantically inheriting derivative, a compound constituent, or a lexicalized form that must block inheritance.

### Required Remediation

Represent these layers separately:

```text
lexeme
├── inflectional paradigm
├── candidate derivational histories
├── compound participation and hierarchy
└── lexical-sense inventory
```

Each sense needs an ID, provenance, domain/register/time, attestation status, and inheritance permissions. Institution-approved terminology must remain distinct from historical attestation. Samāsa should be a probabilistic compound hypergraph rather than a flat component list.

---

## FG-04 — Event Structure, Sentence Interpretation, Discourse, and Register

**Legacy gaps:** G-09, G-10, G-12–G-15

### Gap

The architecture does not adequately separate:

- vibhakti as surface realization from kāraka as participant relation;
- voice, tense/aspect/mood, nominalization, and omitted arguments;
- sentence-level expectancy, compatibility, connectedness, and intended purport;
- coreference, ellipsis, quotation, cause, contrast, objection, answer, and conclusion;
- register, historical period, genre, and domain;
- Vedic accent, recensional variation, Chandas, and oral structure.

### Consequences

The system cannot reliably recognize event-equivalent paraphrases or protect a modern update from contaminating another discourse referent, historical stage, philosophical sense, poetic use, or specialist register.

### Required Remediation

```text
vibhakti and morphosyntax
→ kāraka and event roles
→ sentence constraints
→ discourse and coreference
→ register, period, genre, and domain
```

Version 1 should include event roles, selected sentence constraints, coreference, domain, and register. Vedic and prosodic coverage should be explicitly deferred and separately validated.

---

## FG-05 — Executable Rules and Structural Representation

**Legacy gaps:** G-16–G-19

### Gap

A flat root-centred graph cannot express scope, inherited context, defaults, exceptions, precedence, optionality, isolated intermediate states, multi-part relations, language-independent concepts, or retrieval through several indexes.

### Required Remediation

Adopt a typed multilayer hypergraph or graph-plus-transducer system:

```text
phonological graph/transducers
surface and lexical graph
inflectional paradigm graph
derivational process graph
compound hypergraph
event/kāraka graph
sentence and discourse graphs
lexical-sense graph
rule/meta-rule graph
canonical concept graph
evidence/provenance graph
```

Candidate engineering roles include:

| Grammatical mechanism | Possible machine role |
|---|---|
| Adhikāra | Update scope |
| Anuvṛtti | Inherited context |
| Utsarga–apavāda | Default with protected exception |
| Rule precedence | Conflict resolution |
| Optionality | Multiple admissible analyses |
| It-marker | Internal control metadata |
| Asiddha-like isolation | Temporary-state isolation |

These are hypotheses, not literal equivalences.

The **canonical concept graph must remain language-independent** and contain definitions, formal relations, equations, code, and evidence. Sanskrit structures align to concepts but do not define reality by themselves.

Retrieval must support form, phonology, paradigm, derivation, compound, event role, sense, discourse referent, concept, and evidence indexes, while recording the path used.

---

## FG-06 — Assimilation, Memory, Inheritance, and Update Scope

**Legacy gaps:** G-20–G-24

### Gap

The present compiler is claim-centred, the memory taxonomy is too coarse, and “semantic inheritance with override” is not executable. Legitimate competing analyses also lack a representation.

### Required Remediation

#### Staged Assimilation Compiler

```text
preserve source
→ normalize language/script
→ source-faithful semantic parse
→ extract entities/events
→ align canonical concepts
→ propose Sanskrit lexical candidates
→ analyze phonology, Sandhi, morphology, compounds, sentence, and discourse
→ assign register/domain/time
→ evaluate evidence and contradiction
→ propose inheritance and update scope
→ validate
→ commit a reversible memory transaction
```

#### Operational memory partitions

- form and variant memory;
- paradigm memory;
- derivation and compound memory;
- event, sentence, and discourse memory;
- lexical-sense and register memory;
- rule/meta-rule memory;
- canonical concept and evidence memory;
- temporary plastic memory.

#### Layer-wise update-scope lattice

```text
Update target
├── surface/script/Sandhi variants
├── inflectional forms
├── inheriting and non-inheriting derivatives
├── compound occurrences
├── event paraphrases
├── discourse references
├── cross-language equivalents
└── protected boundaries
    ├── homonym
    ├── lexicalized sense
    ├── different domain/register/time
    ├── competing analysis
    └── unsupported claim
```

For every propagation, record the inherited property, typed relation, domain, register, time, confidence, blocking exception, and affected memory type. Preserve unresolved analyses with their school, source, dictionary, or domain attribution.

The update-scope lattice should become the central object for propagation, locality, and rollback evaluation.

---

## FG-07 — Confidence, Ambiguity, and Response Policy

**Legacy gaps:** G-25–G-27

### Gap

Three top-level confidence scores are useful for presentation but too coarse internally. Confidence propagation and ambiguity-preserving responses are unspecified.

### Required Remediation

Maintain layer-level confidence for script, phonology, Sandhi, inflection, derivation, compound, kāraka, sentence, discourse, lexical sense, concept alignment, evidence, temporal validity, and source reliability.

Uncertainty must propagate without premature collapse. For example:

```text
uncertain segmentation
→ several morphological analyses
→ several compound/sentence interpretations
→ divergent concept alignments
→ targeted retrieval or abstention
```

The model must support multiple live analyses, a preferred interpretation with alternatives, grammatical analysis without factual commitment, unresolved terminology, and scholar/domain-review abstention.

---

## FG-08 — Data, Annotation, Expert Review, and Synthetic Integrity

**Legacy gaps:** G-28–G-30

### Gap

There is no common record for the expanded stack, no full adjudication model, and insufficient protection against model-generated Sanskrit becoming its own evidence.

### Required Remediation

A shared record should contain:

```text
source and source language
script/normalization provenance
Sandhi candidates and canonical forms
morphology and derivation
compound hierarchy
kāraka/sentence/discourse structure
lexical sense, register, domain, and time
canonical concept IDs
evidence and contradiction
update-scope labels
tool, version, reviewer, and adjudication history
```

Governance needs distinct specialists in phonology/Vedic studies, Pāṇinian grammar, lexicography, sentence semantics, discourse/śāstra, computational linguistics, modern domains, evaluation, and data governance. Publish annotation manuals, agreement measures, disagreement taxonomies, and correction history.

Synthetic safeguards must keep **generated**, **translated**, **attested**, and **institution-standardized** usage separate; preserve source-language evidence; use untouched tests; and prevent repeated model output from becoming semantic authority.

---

## FG-09 — Experimental Controls and Novelty Measurement

**Legacy gaps:** G-31–G-38

### Gap

The current Models A–E progression changes structure, retrieval, memory, provenance, contradiction handling, parameters, and plasticity simultaneously. A generic semantic graph is also too weak a comparator for a full executable Sanskrit stack.

### Required Remediation

#### Structural ladder before assimilation

```text
S0 text only
S1 script + phonology + Sandhi
S2 inflection
S3 derivation
S4 compounds
S5 kāraka/event roles
S6 sentence constraints
S7 discourse/coreference
S8 rule scope/defaults/exceptions
S9 lexical senses/register/evidence
S-Full complete stack
```

Run full-minus-one-layer ablations. Add retrieval, writable memory, routing, adapters, and consolidation only after structural value is demonstrated.

#### Strong controls

- information-equivalent generic semantic graph;
- universal linguistic stack;
- generic executable grammar;
- learned neural latent structure;
- controlled descriptive English or another morphologically rich language;
- vector memory;
- text-only control.

#### Equivalence requirements

Match facts, definitions, concept relations, node/edge/relation budgets, encoder parameters, retrieval budget, context tokens, training/inference FLOPs, parser cost, latency, storage, and memory.

#### Theory-versus-tool separation

Compare scholar-validated oracle, rule-generated, neural-predicted, ensemble, and noisy structures. Oracle success with predicted failure indicates a tooling problem; oracle failure weakens the representation thesis.

#### Holdouts and evaluation worlds

Use unseen Sandhi, paradigm cells, derivations/families, nested compounds, event paraphrases, domain senses, lexical exceptions, discourse relations, register boundaries, and conflicting updates across:

1. clean-room fictional concepts;
2. engineered modern technical Sanskrit;
3. attested natural Sanskrit.

#### Primary novelty endpoint

Measure whether the Sanskrit stack shifts the **propagation–locality Pareto frontier** across forms, inflections, derivations, compounds, events, discourse, and languages while preserving homonyms, lexicalized exceptions, unrelated roles, domains, registers, and unsupported claims.

---

## FG-10 — Plasticity and Dynamic Rewiring

**Legacy gaps:** G-39–G-40

### Gap

Fast weights and effective-weight equations appear before the structural representation has been validated, and the equations do not define update generation, scope, conflict, expiry, or rollback.

### Required Remediation

Use this order:

```text
structural analysis
→ structured retrieval
→ writable semantic memory
→ routing
→ temporary adapters
→ reviewed weight consolidation
```

Before adapters are introduced, specify which layers may change, how structural scope constrains updates, how deltas interact, how they expire or promote, how rollback works, and how unrelated capabilities are regression-tested.

Exclude fast-weight and base-weight rewriting from the first pilot.

---

## FG-11 — Error Containment, Scale, Interoperability, and Causal Observability

**Legacy gaps:** G-41–G-44

### Gap

The architecture lacks containment for cascading linguistic errors, a scale plan for large lattices, a common tool interchange format, and proof that displayed structural traces causally affect answers.

### Required Remediation

- Preserve alternative paths and delay commitment.
- Use layer-specific thresholds and cross-layer consistency checks.
- Roll back downstream records when an upstream analysis changes.
- Bound candidate beams, retrieval depth, latency, storage, and compute.
- Use sparse hypergraphs, caching, memoization, versioning, approximate indexes, and hot/archive memory.
- Publish a format carrying candidates, typed relations, derivation traces, confidence, tool/version, corrections, unresolved alternatives, provenance, and licence.
- Run causal interventions: remove, corrupt, substitute, or patch structural states and compare output, confidence, retrieval, routing, and update logs.

---

## FG-12 — Governance, Uniqueness, and Falsification

**Legacy gaps:** G-45–G-47

### Gap

Governance does not mirror the expanded stack, the uniqueness statement is broader than the algorithmic core, and no stop rule is attached to the thesis.

### Required Remediation

Create coordinated groups for representation standards, grammar, lexical resources, sentence/discourse analysis, Vedic/historical material, modern terminology, domain evidence, evaluation, safety, provenance, licensing, and release.

The novelty claim should test the **causal value of the stack's organization, transformations, inheritance, exceptions, and scope**, not claim that every integrated component is new.

Narrow or stop the architectural claim if:

- an information-equivalent universal linguistic stack matches it;
- a generic executable grammar matches propagation and locality;
- gains vanish under family, sense, discourse, or register holdouts;
- predicted analyses erase oracle gains without a credible tooling path;
- graph costs outweigh meaningful accuracy or data-efficiency gains;
- benefits come only from curated terminology;
- attested natural Sanskrit does not reproduce controlled gains.

---

# 4. Target Architecture After Gap Resolution

```text
INPUT + SOURCE PROVENANCE
        │
        ▼
SCRIPT / PHONOLOGY / SANDHI LATTICE
        │
        ▼
LEXICAL + INFLECTIONAL LATTICE
        │
        ▼
DERIVATION GRAPH + COMPOUND HYPERGRAPH
        │
        ▼
KĀRAKA / EVENT / SENTENCE / DISCOURSE GRAPHS
        │
        ▼
LEXICAL SENSE + REGISTER + DOMAIN
        │
        ├──────────────┐
        ▼              ▼
RULE-SCOPE ENGINE   CANONICAL CONCEPT GRAPH
        │              │
        └────────── EVIDENCE / PROVENANCE
                       │
                       ▼
             CROSS-LAYER RECONCILIATION
                       │
                       ▼
             MULTI-INDEX STRUCTURAL MEMORY
                       │
                       ▼
              RETRIEVAL / ROUTING / RESPONSE
                       │
                       ▼
             REVERSIBLE UPDATE TRANSACTION
```

## Architectural invariants

1. Canonical concepts remain language-independent.
2. Alternatives remain live until evidence justifies commitment.
3. Every update has scope, provenance, confidence, and rollback.
4. External evidence may override structural plausibility.
5. Explanatory traces must be causally tested.
6. Plasticity follows structural-memory validation.

---

# 5. Prioritized Remediation Roadmap

## Priority 0 — Specification

- Define naming and attribution boundaries.
- Publish the Version 1 coverage contract.
- Define canonical concept/evidence schemas.
- Define typed structural, rule, and interchange formats.
- Define multi-index retrieval and the update-scope lattice.
- Publish annotation and adjudication rules.
- Pre-register baselines, equivalence constraints, and stopping criteria.

## Priority 1 — First structural pilot

Implement script/phonology, Sandhi, inflection, derivation, nested compounds, kāraka/event roles, lexical senses, domain/register, and external concept/evidence memory.

Use a frozen base model, oracle and predicted structures, no fast-weight rewriting, and clean-room, technical, and attested evaluations.

Primary question:

> Does the multilayer Sanskrit representation improve acquisition, retrieval, propagation, and locality over information-equivalent universal, semantic, procedural, neural, vector, and text-only controls?

## Priority 2 — Scope and exception research

Add rule scope, defaults/exceptions, precedence, sentence compatibility, discourse/coreference, scope prediction, fine-grained calibration, and causal intervention tests.

## Priority 3 — Controlled self-assimilation

Only after structural gains are demonstrated, add writable institutional memory, scope-conditioned routing, temporary adapters, rehearsal, and governed weight consolidation.

## Priority 4 — Specialist expansion

Add independently validated Vedic, recensional, oral, Chandas, kāvya/alaṅkāra, extended śāstric discourse, manuscript, and recitation modules.

---

# 6. Revised Uniqueness and Result Interpretation

## Defensible uniqueness statement

> **We seek to determine whether an executable multilayer Sanskrit structural representation—spanning phonological transformation, inflection, derivation, compound hierarchy, predicate-centred semantic roles, sentence and discourse constraints, lexicalized meaning, register, and explicit rule scope—can serve as a causal substrate for knowledge acquisition, retrieval, propagation, exception handling, and update locality, outperforming information-equivalent universal linguistic, semantic-graph, generic procedural, learned neural, vector-memory, and text-only baselines.**

## Result interpretation

| Result | Programme implication |
|---|---|
| Beats text/vector only | Explicit structure helps; Sanskrit-specific novelty is unproven. |
| Matches universal linguistic stack | Narrow the claim to explicit linguistic structure generally. |
| Matches generic executable grammar | Procedural scope explains the gain; Sanskrit is a strong instance, not a unique mechanism. |
| Oracle succeeds, predicted fails | Representation may be valid; tooling is the bottleneck. |
| Only engineered terms succeed | Curation or descriptive naming may drive the result. |
| Controlled gains fail on attested Sanskrit | Natural ambiguity limits generalization. |
| Propagation rises but locality falls | Inheritance is too aggressive. |
| Propagation–locality improves across all worlds | Strong support for the central novelty claim. |
| Costs outweigh meaningful gains | Preserve resources, but do not scale as an efficiency architecture. |

---

# 7. Legacy Gap Crosswalk

| Refactored family | Legacy gaps retained |
|---|---|
| FG-01 | G-01–G-03 |
| FG-02 | G-04–G-05 |
| FG-03 | G-06–G-08, G-11 |
| FG-04 | G-09–G-10, G-12–G-15 |
| FG-05 | G-16–G-19 |
| FG-06 | G-20–G-24 |
| FG-07 | G-25–G-27 |
| FG-08 | G-28–G-30 |
| FG-09 | G-31–G-38 |
| FG-10 | G-39–G-40 |
| FG-11 | G-41–G-44 |
| FG-12 | G-45–G-47 |

---

# 8. Final Assessment

The expanded understanding of Sanskrit does not invalidate the self-assimilating concept. It shows that its current internal structure is incomplete.

The durable cycle remains:

```text
internal structure proposes
external evidence grounds or corrects
controlled memory reconciles
institutional governance consolidates
```

But “internal structure” must mean a typed, uncertainty-aware Sanskrit structural stack rather than mainly a dhātu graph.

The resulting research proposition is:

> **A formally organized natural language may provide not only labels for concepts, but an executable system for constraining interpretation, generating alternatives, defining inheritance, representing exceptions, and controlling where knowledge updates should and should not propagate.**

The next artifact should be a **Version 2 Research Architecture and Controlled Experimental Protocol**, not an immediate expansion of the brainstorming model.

---

# 9. Selected Evidence Base

These works support the need for the missing layers; the proposed architecture remains a research hypothesis.

1. Amrith Krishna et al., **Word Segmentation in Sanskrit Using Path Constrained Random Walks** — https://aclanthology.org/C16-1048/
2. Jivnesh Sandhan et al., **DepNeCTI: Dependency-based Nested Compound Type Identification for Sanskrit** — https://aclanthology.org/2023.findings-emnlp.914/
3. Amba Kulkarni et al., **Dependency Relations for Sanskrit Parsing and Treebank** — https://aclanthology.org/2020.tlt-1.12/
4. Harshad Ayachit et al., **Computational Modelling of the Apatyādhikāra in Aṣṭādhyāyī** — https://aclanthology.org/2026.iscls-1.16/
5. Tapas Khanra et al., **TantraTagger** — https://aclanthology.org/2026.iscls-1.4/
6. Sriram Krishnan et al., **Challenges in Processing Vedic Sanskrit** — https://aclanthology.org/2025.wsc-csdh.9/
7. Anagha Pradeep et al., **Towards Building a Computational Sense Inventory from the Monier-Williams Dictionary** — https://aclanthology.org/2026.iscls-1.3/

---

# 10. Proposed Next Artifact

The Version 2 architecture and protocol should specify:

- bounded stack coverage and attribution;
- canonical concept/evidence models;
- typed structural and rule representations;
- multi-index retrieval;
- the Assimilation Compiler's intermediate forms;
- the update-scope lattice;
- confidence and ambiguity handling;
- annotation and interoperability schemas;
- structural ladder, baselines, ablations, and holdouts;
- propagation–locality benchmarks;
- oracle-versus-predicted evaluation;
- go/no-go criteria for plasticity and scale.
