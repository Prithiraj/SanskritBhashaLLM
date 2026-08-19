# Pāṇinian-Grounded Foundation Model Strategy

## Using Existing Sanskrit Projects to Build a Distinct Open-Weight Institutional LLM

The opportunity is not to build another LLM that happens to speak Sanskrit. It is to use Sanskrit’s unusually explicit grammatical and derivational system as a machine-readable learning substrate—while treating existing Sanskrit projects as expert components, teachers, datasets, and baselines.

A generic Sanskrit LLM competes with SansGPT, ByT5-Sanskrit, BharatGen, DheeYantra, ParamTatva, and future institutional models.

A **Pāṇinian-grounded foundation model that learns jointly from surface language, derivational structures, semantic representations, and modern scientific grounding** would use those projects rather than duplicate them.

---

# 1. What Actually Makes Sanskrit Stand Out?

Sanskrit is not special merely because it has inflection, compounds, or relatively flexible word order. Other languages have these properties.

What stands out computationally is their **combination with an unusually detailed, procedural grammatical tradition**.

Pāṇini’s system does not merely list acceptable sentences or describe broad tendencies. It represents language through ordered operations, derivational rules, technical markers, rule interaction, and meta-rules. Modern computational work regularly treats the Aṣṭādhyāyī as a formal or generative system rather than an ordinary descriptive grammar.

The useful distinction is:

> English supplies abundant linguistic data.  
> Sanskrit supplies linguistic data **plus an externalized theory of how many of its forms are generated and related**.

This does not mean the complete semantics of every Sanskrit expression can be calculated mechanically. It means the model can be given much more structured supervision than raw next-token prediction alone.

## 1.1 Derivational Morphology

A Sanskrit expression can carry relationships involving:

- dhātu;
- upasarga;
- kṛt and taddhita suffixes;
- nominal and verbal inflection;
- case, number, person, tense and mood;
- derivational history.

The important benefit is not just that a word can be divided into parts. It is that the model can potentially receive a **derivational trace**:

```text
underlying root
    ↓
prefix application
    ↓
derivational suffix
    ↓
phonological transformations
    ↓
inflection
    ↓
surface form
```

That trace creates supervision at several levels.

A conventional model sees:

```text
surface tokens → predict continuation
```

A Pāṇinian-grounded model could see:

```text
surface tokens
+ root
+ affixes
+ grammatical features
+ derivation path
+ candidate semantic contribution
```

The additional information may help the model connect rare or previously unseen forms to known families.

This is the deepest computational opportunity in Sanskrit.

## 1.2 Samāsa: Semantic Compression with Ambiguity

Sanskrit compound formation can encode relationships that another language might express through a longer phrase. Computational research describes compounding as pervasive in Sanskrit and as an important source of lexical and structural economy. But compound interpretation is also context-sensitive: the surface components do not always uniquely specify the intended semantic relation.

That gives the project both an advantage and a research problem.

The advantage is:

```text
several related concepts
→ compact structured expression
```

The problem is:

```text
one compact expression
→ several plausible compound analyses
```

Therefore the model should not receive one supposedly infallible samāsa analysis. It should receive a **ranked lattice of candidates**:

```text
Candidate A: Tatpuruṣa interpretation       0.55
Candidate B: Karmadhāraya interpretation    0.27
Candidate C: lexicalized/domain meaning     0.18
```

Context, domain knowledge, definitions, equations, and actual usage should determine which candidate wins.

That is better than both extremes:

- purely statistical guessing;
- rigid symbolic parsing.

## 1.3 Sandhi: Systematic Transformation, Not Merely a Nuisance

Sandhi can remove visible word boundaries and alter sounds at boundaries, making Sanskrit segmentation difficult. Existing Sanskrit NLP research consequently treats segmentation as a central problem rather than a trivial preprocessing step.

But Sandhi is also highly structured.

For an LLM, this means the same underlying expression may exist at several representational levels:

```text
surface phonological form
↕
possible word boundaries
↕
canonical lexical forms
↕
derivational structure
```

Most general-purpose tokenizers operate principally at the surface-string level. A Sanskrit-native model could explicitly connect all four.

This can improve:

- segmentation;
- robustness to spelling and script variation;
- lexical retrieval;
- morphological reuse;
- token efficiency;
- error detection.

## 1.4 Kāraka: Predicate-Centred Semantic Relations

Pāṇinian analysis can represent participants through their relationships to an action or predicate rather than depending entirely on fixed word order. Kāraka-oriented systems have also been applied computationally beyond Sanskrit, including question-answering and analysis in modern Indian languages.

This is valuable because it offers a representation such as:

```text
action: giving
agent: teacher
recipient: student
object: knowledge
instrument: speech
location: classroom
```

The surface word order may vary, but the underlying relational structure can remain stable.

For a multilingual model, that could become a bridge between:

- Sanskrit;
- Hindi;
- Marathi;
- Bengali;
- other languages whose surface syntax differs;
- English output;
- formal semantic graphs.

This is stronger than claiming Sanskrit is genealogically the parent of every Indian language. The defensible claim is that **Pāṇinian categories may provide a useful shared computational representation** across languages.

## 1.5 The Grammar Can Generate, Analyze, and Verify

Most linguistic datasets contain examples:

```text
input → label
```

A rule system such as Pāṇinian grammar can potentially do more:

- generate valid forms;
- produce derivation histories;
- reject invalid combinations;
- enumerate competing analyses;
- expose intermediate transformations;
- validate generated outputs.

This means it can function as:

- a data generator;
- a weak supervisor;
- an adversarial-example generator;
- an auxiliary-task provider;
- an inference-time verifier;
- an interpretability interface.

That makes Sanskrit valuable not merely as training text but as an **experimental environment for neuro-symbolic language modelling**.

## 1.6 What Sanskrit Grammar Cannot Provide by Itself

This boundary is critical.

A morphological analysis can suggest that a new expression means something like:

```text
backward + flow
```

It cannot by itself tell the model:

- what a gradient is;
- what a loss function is;
- how the chain rule works;
- how parameters are updated;
- what code implements the operation.

The grammar supplies an **intensional prior**: an initial structural indication of meaning.

Modern documents, equations, experiments, code, definitions, and usage supply **referential grounding**.

The Kimi discussion reached exactly this synthesis: Pāṇinian analysis generates candidate meanings; a Sanskritized modern corpus supplies distributional and referential grounding; contextual neural processing resolves ambiguity, lexicalization, and idiomatic drift.

That—not “Sanskrit words automatically contain complete knowledge”—is the strongest intellectual foundation for the project.

---

# 2. What the Proposal Is Really Proposing

After rereading it, the proposal can be understood as three layers.

## Layer A: Formal Linguistic Structure

The proposal introduces a Pāṇinian Agent responsible for:

- Sandhi splitting;
- samāsa classification;
- dhātu–pratyaya decomposition;
- semantic-role analysis.

Individually, these functions are not new. Existing Sanskrit systems already perform substantial parts of them.

But the proposal does not stop at using them as standalone NLP utilities. It places them inside a general generative architecture.

That is where the first element of potential novelty begins.

## Layer B: Manufactured Modern Knowledge Grounding

The Sanskritization flywheel proposes:

```text
lexicon design
→ translation
→ expert review
→ model training
→ improved translation
→ corpus expansion
```

This addresses the most serious limitation of a Sanskrit-only classical corpus: morphology can help organize concepts, but it cannot create missing modern scientific knowledge.

The project therefore attempts to combine:

- classical grammatical structure;
- modern scientific content;
- controlled terminology;
- iterative synthetic-data creation.

That combination is more important than simply collecting more Sanskrit books.

## Layer C: Sanskrit-Anchored Representation with Multilingual Interfaces

The proposal keeps English where required for code and interoperability, while using Sanskrit as the central representational language.

The strongest version of this should not be stated as:

> “We know that the model literally thinks in Sanskrit.”

That is difficult to verify.

It should be operationalized as:

> **The model uses an explicitly Sanskrit-anchored Pāṇinian intermediate representation during training and inference, and causal experiments demonstrate that this representation contributes to its answers.**

That is measurable.

---

# 3. The Actual Uniqueness

The uniqueness is **not any single component**.

It is not:

- the first Sanskrit generative model;
- the first Pāṇinian parser;
- the first Sanskrit tokenizer;
- the first Sanskrit morphology system;
- the first Sanskrit semantic representation;
- the first structured Sanskrit transformer;
- the first Indic multilingual model.

Each of those claims has meaningful prior art.

The defensible novelty is the following complete system:

> **A jointly trained, open-weight foundation model that fuses compact Sanskrit surface representations with probabilistic Pāṇinian derivation graphs, a language-independent semantic representation, and grounded modern technical knowledge—and demonstrates causal improvements in low-shot acquisition and systematic use of genuinely unseen concepts.**

There are five required elements.

## 3.1 Probabilistic Derivation, Not One Deterministic Parse

The model receives:

- alternative Sandhi splits;
- alternative lemmas;
- alternative samāsa analyses;
- possible derivations;
- confidence scores;
- tool provenance.

It learns which symbolic analyzer to trust under which conditions.

## 3.2 Joint Learning, Not Preprocessing

A parser simply placed before an ordinary LLM is not enough.

The derivation graph must affect:

- embeddings;
- attention;
- intermediate representations;
- auxiliary losses;
- decoding;
- confidence;
- generated answers.

Then causal ablations must show that the model actually uses it.

## 3.3 Modern Concept Grounding

Every important technical term should link to:

- a concept identifier;
- definition;
- Sanskrit term and alternatives;
- derivational analysis;
- English and Indic-language equivalents;
- equations;
- code;
- diagrams where relevant;
- authoritative source passages;
- expert review;
- version history.

## 3.4 Strict Compositional Evaluation

The benchmark must withhold entire term families and combinations from training.

The model should not be rewarded for memorizing a near-duplicate.

It should demonstrate:

- understanding of an unseen derivation;
- provisional semantic inference;
- grounding from one or a few examples;
- application to a new problem;
- transfer to another language;
- correct handling of ambiguity and idiom.

## 3.5 A Reusable Architecture, Not One Checkpoint

The Pāṇinian structural layer should be capable of attaching to more than one foundation-model backbone.

If it improves:

- a Sanskrit model trained from scratch;
- an Indian multilingual model;
- another open multilingual model;

then the institution has demonstrated an architectural contribution rather than merely releasing another fine-tune.

---

# 4. A Unique Architecture Built from the Existing Ecosystem

The following architecture has not been identified as a publicly documented system implemented end to end.

## The Pāṇinian Grounded Foundation Model

```text
                    USER INPUT
          Sanskrit / English / Indic language
                         │
                         ▼
        ┌───────────────────────────────────┐
        │ Script and phonological adapter   │
        │ canonical forms + byte fallback  │
        └─────────────────┬─────────────────┘
                          │
           ┌──────────────┴──────────────┐
           │                             │
           ▼                             ▼
┌──────────────────────┐      ┌─────────────────────────┐
│ Compact token stream │      │ Pāṇinian derivation     │
│                      │      │ lattice                 │
│ native tokenizer     │      │                         │
│ efficient sequence   │      │ Sandhi candidates       │
│ ordinary context     │      │ dhātu/upasarga/pratyaya │
└──────────┬───────────┘      │ kṛt/taddhita            │
           │                  │ samāsa alternatives     │
           │                  │ kāraka relations        │
           │                  │ confidence/provenance   │
           │                  └────────────┬────────────┘
           │                               │
           └──────────────┬────────────────┘
                          ▼
              ┌────────────────────────┐
              │ Token–graph fusion     │
              │ transformer            │
              │                        │
              │ cross-attention        │
              │ confidence gating      │
              │ structural adapters    │
              └────────────┬───────────┘
                           │
                           ▼
              ┌────────────────────────┐
              │ Grounded concept graph │
              │                        │
              │ USR / semantic roles   │
              │ terminology registry   │
              │ definitions            │
              │ equations              │
              │ code                   │
              │ source evidence        │
              └────────────┬───────────┘
                           │
                           ▼
              ┌────────────────────────┐
              │ Multilingual decoder   │
              │ + verifier-guided      │
              │ generation             │
              └────────────────────────┘
```

## Why Two Parallel Streams Matter

A tokenizer optimized entirely for compression might represent a long compound as one token. That reduces sequence length but can conceal its internal structure.

A tokenizer optimized entirely for morphology might produce:

```text
prefix + root + derivational suffix + inflection
```

That exposes structure but may consume more sequential tokens.

The proposed architecture avoids that trade-off:

```text
compact sequential token
+
off-sequence morphological features
```

The token stream provides efficiency.

The derivation graph provides compositional transparency.

This is a particularly strong extension of the token-efficiency part of the proposal. The current document proposes a Pāṇinian-aware tokenizer, but treats morphological segmentation mainly as tokenization. The stronger design represents morphology as an additional structured channel, so the model does not need to choose between token compression and linguistic decomposition.

---

# 5. How Existing Projects Become Collaborators and Components

The institution should classify every external project into one of four roles:

| Role | Meaning |
|---|---|
| **Reusable component** | Integrate code or APIs after technical and licence review |
| **Teacher** | Generate annotations or outputs used to train the new model |
| **Baseline** | Compare against it to establish that the new architecture adds value |
| **Standards partner** | Collaborate on representations, data formats, benchmarks, or governance |

Not every project should be copied into the final runtime. Some are more useful as teachers or evaluation baselines.

## 5.1 Saṃsādhanī: Deterministic Grammatical Expert

The University of Hyderabad’s Saṃsādhanī ecosystem already provides:

- morphological analysis and generation;
- Sandhi tools;
- compound processing;
- derivational generators;
- parsing;
- transliteration;
- an Aṣṭādhyāyī simulator.

Use it for:

- candidate morphological analyses;
- kāraka and dependency structures;
- rule-derived synthetic data;
- validation of generated forms;
- derivation supervision;
- expert-tool comparison.

Do not rebuild all of Saṃsādhanī.

Instead, develop a standard adapter that converts its output into the institution’s probabilistic intermediate representation.

Its role would be:

```text
Saṃsādhanī output
→ normalized derivation candidates
→ confidence/provenance layer
→ foundation-model training
```

## 5.2 Vidyut: High-Speed Derivation and Generation Engine

Vidyut exposes Sanskrit derivation, reverse lookup, Sandhi, segmentation, transliteration, and related linguistic functions through reusable Rust and Python infrastructure. Its prakriyā functionality is especially relevant because it can expose derivational processes rather than merely final labels.

Use it for:

- large-scale generation of valid derived forms;
- derivation traces;
- reverse analysis;
- adversarial invalid forms;
- unit tests for grammatical generation;
- inference-time verification;
- efficient preprocessing.

The institution could fund missing coverage and contribute improvements upstream rather than creating an incompatible new derivation engine.

## 5.3 Sanskrit Heritage: Exhaustive Candidate Lattice

The Sanskrit Heritage Platform provides lexicons, morphology, segmentation, tagging, and parsing. Its reader is particularly useful because it can enumerate alternative phonologically and lexically valid segmentations rather than prematurely forcing one interpretation.

That makes it suitable for constructing the **uncertainty lattice**.

Instead of storing:

```text
correct split = A
```

store:

```text
A: candidate from Heritage
B: candidate from Vidyut
C: candidate from Saṃsādhanī
D: neural candidate from ByT5
human decision: B
contextual evidence: …
```

Disagreement between tools is valuable training data. It teaches the model when grammar is ambiguous and when context is required.

## 5.4 ByT5-Sanskrit: Neural Morphology Teacher and Hard Baseline

ByT5-Sanskrit uses byte-level modelling and has been applied to:

- Sanskrit segmentation;
- lemmatization;
- morphosyntactic analysis;
- parsing-related tasks;
- OCR correction.

It demonstrates how much Sanskrit structure a sufficiently trained neural model can learn without an explicit symbolic engine.

Use it as:

- a neural segmentation teacher;
- a morphology and lemma annotator;
- an OCR/noisy-input normalizer;
- a fallback when deterministic tools fail;
- the strongest neural-only baseline.

This baseline is essential.

The proposed project must demonstrate that:

```text
neural model + explicit Pāṇinian structure
```

outperforms:

```text
strong neural model alone
```

on the unique tasks.

Otherwise, the explicit architecture is not justified.

## 5.5 SanskritShala: Expert Ensemble and Human Correction

SanskritShala integrates neural modules for:

- segmentation;
- morphological tagging;
- dependency parsing;
- compound-type identification;
- interactive correction.

Use it for:

- additional neural-analysis candidates;
- scholar-facing correction interfaces;
- error collection;
- active-learning workflows;
- disagreement analysis;
- benchmark creation.

Its human-correction pattern is particularly valuable for the institutional corpus-building programme.

## 5.6 SHR++ and Annotation Tools: Data-Production Infrastructure

The SHR++ work demonstrates that combining automatic analyses with human review can reduce annotation effort while preserving expert correction.

The institution should build on this pattern rather than asking scholars to annotate every field manually.

The workflow should be:

```text
several tools produce candidates
→ model ranks candidates
→ expert confirms or corrects
→ correction enters training set
→ model improves
```

This is the practical form of the Sanskritization flywheel.

## 5.7 SansGPT: Generative Baseline and Pretraining Knowledge

SansGPT establishes Sanskrit generative pretraining and a custom tokenizer designed with Sanskrit compounds in mind. Its project includes model checkpoints and training/tokenization resources.

Use it as:

- a Sanskrit decoder-only baseline;
- a source of tokenizer experiments;
- a pretraining-data comparison;
- a small generative teacher;
- an ablation reference.

The new project should not claim to be the first Sanskrit GPT.

It should ask:

> Does adding the derivation and grounding streams produce abilities that SansGPT does not exhibit?

## 5.8 DheeYantra and Other Sanskrit Assistants: Instruction Baseline

The DheeYantra Sanskrit model is based on an existing Qwen-family foundation model and targets Sanskrit conversation and assistant-like behaviour.

Use it for:

- instruction-following comparison;
- conversational Sanskrit evaluation;
- synthetic instruction generation, where licensing permits;
- dialogue-style benchmark creation.

It competes at the product surface but not necessarily at the architectural-research level.

## 5.9 BharatGen and Indian Foundation Models: Backbone and National-Scale Teacher

Government-supported Indian foundation-model initiatives can supply:

- broad world knowledge;
- Indic-language competence;
- training infrastructure;
- multilingual evaluation;
- larger-model teachers;
- practical deployment backbones.

The institution should not try to outspend these programmes on a second generic multilingual model.

Instead, it should offer a **Pāṇinian adapter layer** that can be attached to BharatGen-type backbones.

That turns the relationship from competition into complementarity:

```text
BharatGen:
general knowledge + multilingual capacity

Proposed institution:
Pāṇinian representation + Sanskrit grounding
+ compositional benchmark + expert verification
```

## 5.10 IndicTrans2 and AI4Bharat: Translation and Multilingual Bridge

IndicTrans2 provides open translation infrastructure covering India’s scheduled languages and is part of a broader open Indic-language research ecosystem.

Use it for:

- first-pass Sanskritization candidates;
- source-target alignment;
- back-translation;
- multilingual terminology projection;
- cross-lingual benchmark construction;
- adapters for Hindi and other Indic languages.

It should not be trusted alone for authoritative technical Sanskrit. Its translations should feed an expert-governed pipeline.

## 5.11 Sāmayik: Seed Corpus for Contemporary Sanskrit

Sāmayik provides a contemporary English–Sanskrit parallel corpus covering modern prose domains and has been used to improve contemporary Sanskrit translation beyond classical-text domains.

Use it as:

- a seed modern-language corpus;
- a translation baseline;
- a style and terminology study;
- a source of contemporary syntactic patterns;
- an evaluation set after careful leakage controls.

It will not be sufficient for the proposed technical knowledge commons, but it reduces the need to start from zero.

## 5.12 Sanskrit WordNet: Lexical Concept Graph

Sanskrit WordNet provides synsets and lexical-semantic relationships and can support concept alignment rather than mere string translation.

Use it to connect:

```text
surface term
→ lemma
→ synset/concept
→ synonyms
→ broader/narrower concepts
→ equivalent terms in other languages
```

This is especially useful for disambiguation and retrieval.

## 5.13 Universal Semantic Representation: Do Not Reinvent the Semantic Layer

USR Bank work has already developed a Pāṇinian/Indian-grammar-inspired representation covering:

- concepts;
- morphosyntactic relations;
- semantic roles;
- discourse;
- tense;
- aspect;
- modality;
- causation;
- speaker intention.

It is explicitly designed to support language-independent representation and multilingual generation.

This is an important correction to the novelty landscape.

The project cannot claim:

> “We are the first to invent a Pāṇinian semantic representation.”

Instead, it should collaborate with or extend USR.

A strong combined representation might contain:

```text
Pāṇinian derivation layer
    dhātu / affixes / samāsa / Sandhi

USR semantic layer
    concepts / roles / discourse / intention

Modern grounding layer
    definitions / equations / code / evidence
```

That complete vertical integration remains much more distinctive.

## 5.14 Sanskrit Voyager: Retrieval and Evidence Grounding

Sanskrit Voyager supports morphology-aware searching and reading across Sanskrit corpora, accounting for:

- inflection;
- Sandhi;
- compounds;
- transliteration.

Use it for:

- corpus retrieval;
- attestation of generated terms;
- evidence-backed answers;
- finding historical usage;
- retrieval-augmented generation;
- source citation.

The foundation model should not be expected to memorize the entire Sanskrit textual tradition. Retrieval is more reliable and easier to update.

## 5.15 Panini Tokenizer: Compression Baseline

The ArthaLabs Panini Tokenizer uses recursive splitting, dictionary lookup, Sandhi reversal, and a Sanskrit-oriented vocabulary. Its published compression claims should be independently tested, but it provides a useful open tokenizer baseline.

Use it for:

- tokenizer ablations;
- comparison with ordinary BPE and Unigram tokenizers;
- testing morphological transparency versus sequence compression;
- identifying failure cases.

Do not simply adopt its self-reported compression numbers as institutional evidence.

## 5.16 ParamTatva: Phonological Representation Experiment

ParamTatva’s public code includes:

- Sanskrit-specific phonological features;
- Maheshvara-sūtra-related embeddings;
- pratyāhāra-oriented attention biases.

That means the new project should not claim:

> “First transformer to incorporate Sanskrit formal structure.”

Instead, use ParamTatva as:

- a phonological-embedding baseline;
- an architectural ablation;
- a source of ideas for the input layer;
- a reproducibility target.

Its publicly visible emphasis is closer to phonological and pratyāhāra structure than to the full derivational-semantic grounding proposed here.

## 5.17 PINGALA: Verifier-Guided Decoding Pattern

PINGALA combines neural Sanskrit generation with symbolic metrical control. It demonstrates the broader pattern:

```text
neural generation
+
formal Sanskrit verifier
→ controlled output
```

It also illustrates that overly hard formal constraints can improve formal correctness while damaging semantic quality.

Use this lesson for grammatical decoding:

- symbolic rules should guide;
- confidence should be preserved;
- semantic correctness should be measured;
- the system must permit justified exceptions.

## 5.18 Pāṇinian Foundation for Indic Processing: Shared Standards Partner

The 2026 Pāṇinian Foundation paper proposes a unifying framework and benchmark programme for Indic-language processing, while observing that morphology, parsing, and semantic roles remain fragmented across separate projects. It also notes that morpheme-level semantics remains underdeveloped as an evaluation area.

This is highly aligned with the project.

Use it as:

- a standards collaboration;
- a source of cross-Indic benchmarks;
- a basis for shared representations;
- an external evaluation framework.

The proposed model would go beyond that framework by actually training and causally testing a generative foundation model using the representation.

---

# 6. The Institution Should Become the Integrator, Not the Replacement

The institutional strategy should be:

```text
existing projects remain authoritative in their domains
                       ↓
the institution defines interoperability standards
                       ↓
tools produce compatible candidate structures
                       ↓
the model learns from their agreements and disagreements
                       ↓
improvements are contributed back upstream
```

Government funding can support the ecosystem through:

- formal consortium agreements;
- sub-grants to maintain existing tools;
- shared compute;
- fellowships;
- common data formats;
- joint benchmark development;
- upstream maintenance;
- expert review programmes.

This is more credible than claiming the institution will recreate decades of Sanskrit computational linguistics internally.

It also gives the government a compelling national-infrastructure argument:

> The programme consolidates and advances existing Indian and international Sanskrit computational research instead of displacing it.

---

# 7. A Two-Track Model Strategy

A single model cannot simultaneously prove scientific novelty and immediately compete with large general-purpose models economically.

The institution should build two related tracks, plus an adapter layer.

## Track A: Research-Native Model

Train a relatively small model from scratch using:

- Sanskrit-native tokenizer;
- Pāṇinian derivation graph;
- USR semantic representation;
- controlled corpus;
- matched neural-only baselines.

Purpose:

- prove causality;
- test token efficiency;
- test unseen composition;
- test sample efficiency;
- publish reproducible ablations.

This model is where the scientific uniqueness is established.

## Track B: Capability Model

Take a strong open multilingual or Indian foundation-model backbone and add:

- Pāṇinian graph adapters;
- Sanskrit continued pretraining;
- controlled terminology grounding;
- retrieval;
- verification;
- multilingual output adapters.

Purpose:

- practical question answering;
- translation;
- education;
- technical assistance;
- institutional deployment.

This model may not be as scientifically clean because the backbone already contains broad knowledge. But it can become useful much faster.

## Track C: Pāṇinian Adapter SDK

Release the structural layer as an independent open component that can attach to multiple models.

For example:

```text
BharatGen + Pāṇinian adapter
Open multilingual model + Pāṇinian adapter
Sanskrit-native model + Pāṇinian adapter
```

If the adapter improves several unrelated backbones, the institution has established a general architectural result.

That is more defensible and valuable than claiming one particular checkpoint is revolutionary.

---

# 8. What the Institution Must Own

Existing projects can supply many components. The institution’s durable contribution should be the layer that does not currently exist as one coherent public system.

## 8.1 Pāṇinian Grounded Representation

Create an open standard encoding:

- surface form;
- canonical form;
- Sandhi alternatives;
- lemma and dhātu;
- upasarga and pratyaya;
- kṛt/taddhita derivations;
- samāsa alternatives;
- kāraka relations;
- USR concepts and discourse;
- confidence;
- provenance;
- lexicalized or idiomatic status;
- technical concept identifiers;
- source grounding.

Call it, for example, the **Pāṇinian Grounded Representation**, although the eventual name should be decided with scholars and partner institutions.

## 8.2 Sanskrit Technical Knowledge Commons

This should be more than a translated corpus.

Each concept record should contain:

```text
Concept ID
Source-language name
Approved Sanskrit term or alternatives
Morphological derivation
Definition
Domain
Equations
Algorithms
Code
Examples
Related concepts
Confusable concepts
Source citations
Reviewers
Confidence
Version history
```

That resource can serve:

- models;
- universities;
- translators;
- textbook authors;
- terminology commissions;
- digital libraries;
- public educational platforms.

## 8.3 Compositional Generalization Benchmark

This is likely the most publishable and globally distinctive asset.

It should test:

| Test | What is withheld |
|---|---|
| Unseen surface form | Exact word |
| Unseen combination | Known components in a new combination |
| Family holdout | Entire related derivational family |
| New concept | Technical referent introduced in one or a few examples |
| Ambiguous compound | Context determines among valid parses |
| Idiomatic conflict | Literal morphology conflicts with established usage |
| Cross-lingual transfer | Learn through Sanskrit, apply in another language |
| Causal test | Remove or corrupt the supplied derivation |
| Efficiency test | Fixed accuracy, tokens, memory, latency, and FLOPs |

Without this benchmark, the project may produce impressive demonstrations but no proof that the new architecture matters.

## 8.4 Open Model Family

Release:

- tokenizer;
- research model;
- capability model;
- adapters;
- checkpoints;
- training code;
- evaluation harness;
- model cards;
- corpus documentation;
- provenance records.

Open weights alone are not enough for an institutionally significant research programme.

---

# 9. Training Objectives That Make the Architecture Genuinely Different

The current proposal already includes next-token prediction combined with dhātu identification and samāsa classification.

That should be expanded into the central objective:

\[
\mathcal{L}
=
\mathcal{L}_{LM}
+
\lambda_1\mathcal{L}_{derivation}
+
\lambda_2\mathcal{L}_{parse-ranking}
+
\lambda_3\mathcal{L}_{semantic-role}
+
\lambda_4\mathcal{L}_{concept-alignment}
+
\lambda_5\mathcal{L}_{grounding}
+
\lambda_6\mathcal{L}_{translation}
+
\lambda_7\mathcal{L}_{calibration}
\]

Where:

- \(L_{LM}\): ordinary next-token prediction;
- \(L_{derivation}\): predict roots, affixes, and derivational history;
- \(L_{parse-ranking}\): rank alternative analyses;
- \(L_{semantic-role}\): predict kāraka and USR relations;
- \(L_{concept-alignment}\): connect multilingual terms to the same concept;
- \(L_{grounding}\): connect terms to definitions, equations, code, or evidence;
- \(L_{translation}\): preserve concepts across languages;
- \(L_{calibration}\): admit uncertainty when several analyses remain plausible.

This joint objective is much harder to dismiss as “a parser attached to a chatbot.”

---

# 10. A Concrete End-to-End Example

Suppose experts introduce a Sanskrit technical expression for a new scientific concept.

## Ordinary Sanskrit LLM

It receives translated passages containing the term.

It learns the term statistically if it sees enough examples.

## Proposed System

The terminology record supplies:

```text
approved expression
candidate derivation
compound relationship
concept ID
English equivalent
definition
equation
code example
source textbook
review status
```

The model also receives multiple parser outputs.

Later it encounters a new related expression that never appeared in training.

The system can:

1. identify familiar derivational components;
2. generate several structural interpretations;
3. connect them to the known concept graph;
4. use context to rank the alternatives;
5. retrieve the relevant definition and evidence;
6. apply the concept to a new problem;
7. explain the result in Sanskrit, English, Hindi, or another supported language;
8. expose its derivational interpretation and sources.

That is qualitatively different from merely generating fluent Sanskrit.

---

# 11. What Should Change in the Present Proposal

The vision remains useful, but the institutional version needs several refinements.

| Present formulation | Stronger institutional formulation |
|---|---|
| Sanskrit as an asserted “cognitive substrate” | Sanskrit-anchored Pāṇinian intermediate representation with measurable causal use |
| Pāṇinian Agent as a sequential front-end | Multi-tool probabilistic derivation lattice jointly fused with the transformer |
| Pāṇinian-aware tokenizer alone | Compact native token stream plus off-sequence morphology graph |
| Sanskritized documents as ordinary corpus | Provenance-rich technical knowledge commons |
| Approximately 360B-token initial target | Quality-first staged corpus, scaled only after architectural validation |
| Approximately 2× context / 50% cost saving | Testable efficiency hypothesis across modern domains |
| Sanskrit as parent of most Indian languages | Shared Pāṇinian computational representation for cross-Indic transfer |
| Sanskrit identifiers as code benefit | Optional output; code and equations used primarily for concept grounding |
| Visible reasoning chains as interpretability | Causal derivation and grounding traces, tested through ablation |

The current 360-billion-token target is premature. First demonstrate that explicit structure improves learning. Only then scale the corpus.

Likewise, the context-window and cost claims should remain experimental targets rather than promised outcomes.

---

# 12. Where This Model Can Be Genuinely Competitive

It should not initially claim it will defeat the largest commercial models on all general knowledge.

It should target dimensions where the architecture creates an advantage.

## Novel-Term Understanding

Correctly interpret and apply well-formed but unseen derived expressions.

## Sample Efficiency

Learn a new technical concept from fewer grounded examples.

## Technical Sanskrit

Produce consistent scientific terminology, definitions, equations, and explanations.

## Morphological Fidelity

Maintain grammatical correctness across derivation, inflection, Sandhi, and compounds.

## Token and Memory Efficiency

Use a Sanskrit-native tokenizer and compact representation, then measure:

- tokens per equivalent passage;
- KV-cache memory;
- latency;
- FLOPs per correct answer;
- concepts represented per context window.

## Cross-Lingual Transfer

Introduce knowledge through one language and apply it through Sanskrit-anchored semantic structures in another.

## Auditability

Expose:

- candidate derivations;
- selected interpretation;
- confidence;
- terminology record;
- source evidence.

## Small-Model Competence

Demonstrate that explicit structure allows a smaller model to approach or exceed a larger purely statistical model on targeted tasks.

That could be more institutionally and scientifically meaningful than merely releasing another 7B or 70B model.

---

# 13. The Defensible Uniqueness Statement

Subject to a formal literature, code, licence, and patent audit, the following wording is defensible:

> **As of August 2026, we have not identified a publicly documented open-weight system that jointly learns from probabilistic Pāṇinian derivation lattices, a Sanskrit-anchored semantic representation, and provenance-grounded modern technical concepts, and then demonstrates causal improvement on strict unseen-concept composition and cross-lingual transfer benchmarks.**

This wording does not falsely claim that the individual components are new.

It claims novelty in:

- trainable integration;
- uncertainty-aware representation;
- modern grounding;
- causal validation;
- open institutional infrastructure.

That is the part existing projects appear not to provide end to end.

---

# Final Conclusion

The strongest interpretation of Sanskrit for this project is not merely:

> Sanskrit is morphologically rich.

It is:

> **Sanskrit comes with an unusually explicit external model of linguistic derivation that can generate, analyze, connect, and verify language forms.**

Existing Sanskrit projects have already implemented important fragments of that model:

- Saṃsādhanī and Vidyut provide rule-based analysis and generation;
- Sanskrit Heritage provides alternative analyses;
- ByT5-Sanskrit and SanskritShala provide neural linguistic expertise;
- SansGPT and Dhee provide generative baselines;
- Sāmayik and IndicTrans2 provide contemporary translation resources;
- WordNet and USR provide lexical and semantic structure;
- Voyager provides retrieval;
- ParamTatva and the Panini Tokenizer provide structural/tokenization experiments;
- PINGALA provides a model for symbolic control of neural generation;
- BharatGen and related models provide general knowledge and larger backbones.

The institution should not replace any of them.

It should create the missing layer that allows them to work together:

\[
\boxed{
\text{existing Sanskrit expertise}
+
\text{probabilistic Pāṇinian representation}
+
\text{modern concept grounding}
+
\text{joint foundation-model learning}
+
\text{strict causal evaluation}
}
\]

That would transform the proposal from **“another Sanskrit LLM”** into an open national programme for **Pāṇinian-grounded foundation-model research**.

Its competitive asset would not be Sanskrit fluency alone.

It would be the ability to show that explicit linguistic structure can make a model:

- learn novel concepts from fewer examples;
- generalize compositionally;
- consume fewer tokens under a native representation;
- transfer knowledge across languages;
- produce more auditable outputs;
- achieve targeted competence with lower model and compute requirements.

That is a sufficiently distinct institutional direction—and it uses the existing ecosystem as its foundation rather than treating it as competition.

---

# References

- [A Pāṇinian Foundation for Indic Language Processing](https://arxiv.org/abs/2606.24172)
- [Compound Type Identification in Sanskrit](https://aclanthology.org/2022.coling-1.358.pdf)
- [Sanskrit Word Segmentation](https://aclanthology.org/C16-1048.pdf)
- [Pāṇinian Kāraka Relations in NLP](https://aclanthology.org/P93-1015.pdf)
- [Saṃsādhanī / Sanskrit Computational Linguistics Platform](https://sanskrit.uohyd.ac.in/scl/)
- [Vidyut](https://github.com/ambuda-org/vidyut)
- [Sanskrit Heritage Platform](https://sanskrit.inria.fr/)
- [ByT5-Sanskrit](https://aclanthology.org/2024.findings-emnlp.805/)
- [SanskritShala](https://aclanthology.org/2023.acl-demo.10/)
- [SHR++](https://aclanthology.org/2020.lrec-1.874/)
- [SansGPT](https://aclanthology.org/2024.icon-1.50/)
- [DheeYantra](https://huggingface.co/dheeyantra)
- [AIKosh](https://aikosh.indiaai.gov.in/)
- [IndicTrans2](https://ai4bharat.iitm.ac.in/areas/model/NMT/IndicTrans2/)
- [Sāmayik](https://aclanthology.org/2024.lrec-main.1245/)
- [Sanskrit WordNet](https://aclanthology.org/W19-7509.pdf)
- [Universal Semantic Representation](https://aclanthology.org/2025.bhasha-1.2.pdf)
- [Sanskrit Voyager](https://aclanthology.org/volumes/2025.emnlp-demos/)
- [Panini Tokenizer](https://huggingface.co/ArthaLabs/panini-tokenizer)
- [ParamTatva Sanskrit Transformer](https://github.com/ParamTatva-org/sanskrit)
- [PINGALA](https://arxiv.org/abs/2603.24413)
- [Kimi Research Conversation](https://www.kimi.com/share/1a00f7e8-e732-8bff-8000-0000b6739d10)
