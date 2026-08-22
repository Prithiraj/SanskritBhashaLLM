# DQ1-M0 Mapping Cards

## Pāṇinian Inspiration Provenance under the Generic Attribution Label

**Document type:** DQ1-M0 required artifact set (Doc 08 §16.3 mapping-card requirement, §6.5 attribution ledger)
**Version:** 0.1 — AI-drafted for Sanskrit/Pāṇinian reviewer verification
**Date:** 21 August 2026
**Candidate:** PDSGRO-0.1 · **Attribution label:** `generic_sanskrit_inspired_scope_machinery`
**Citation confidence convention:** `[verified-high]` = standard, safely citable; `[verify]` = drafter is not certain of exact loci; reviewer must confirm before any public use.

> **Purpose after relabel:** these cards no longer support uniqueness claims. They document that each generic mechanism has a genuine, honestly-described historical inspiration, so the public phrase *"inspired and populated by Pāṇinian analysis"* (Doc 08 §18.3) is defensible. Each card ends with the reviewer's Approve / Relabel / Reject decision per §16.3.

---

## MC-1 — Governing scope ← *adhikāra*

| Field | Content |
|---|---|
| Ledger row | Governing scope — "Adhikāra-inspired engineering hypothesis" |
| Primary sources | Aṣṭādhyāyī 1.1.49 *ṣaṣṭhī sthāne yogā* — a rule stated in the genitive case governs subsequent rules until discharged `[verified-high]`. Continuation doctrine: an adhikāra persists (*anuvṛtti*) until terminated by conflict, express cancellation, or completion of its domain; commencement rules at 1.2.x `[verify exact sūtra]`. Kāśikā on 1.1.49; Kielhorn, *Paribhāṣenduśekhara*, paribhāṣās on adhikāra continuation `[verify numbers]`; Joshi & Roodbergen commentary vol. on 1.1.49 `[verify]`. |
| Translation sketch | "The genitive (rule) stands in place of (a governing regulation)": one statement acquires continuing force over a family of operations. |
| Interpretive assumptions | (a) Adhikāra creates a region of validity entered once and exited by explicit conditions; (b) it is operationally enforced during the derivation sequence. Competing analyses: whether adhikāra is a distinct meta-rule category or an ordinary rule with special persistence semantics — debated across Kāśikā/Nāgeśa and modern commentators `[verify positions]`. |
| Computational correspondence | Scope = region of rule/fact applicability; activation condition = entry condition; single-parent nesting = governing contexts within governing contexts; anchor = the operative context selected for one evaluation. **Limits:** Pāṇinian adhikāra is dynamic within a linear *prakriyā* (derivation time), not a static request-gated scope graph; there is no runtime anchor selection, no sibling isolation guarantee, and termination uses grammatical discharge, not resource counters. The correspondence is structural analogy, not equivalence. |
| Prior-art subtraction | Kill screen F10/F11: Drools agenda-groups, contextual/modular LP provide organizationally equivalent scoping. Residual: none. |
| Proposed disposition | **Approve as inspiration-only** (Generic label). |

**Reviewer decision:** Approve / Relabel / Reject — Name: ______ Signature: ______ Date: ______ Notes: ______

---

## MC-2 — Inherited context ← *anuvṛtti*

| Field | Content |
|---|---|
| Ledger row | Inherited context — "Anuvṛtti-inspired engineering hypothesis" |
| Primary sources | Anuvṛtti = continuation of technical terms/conditions from an earlier rule into later ones of its domain. Doctrine distributed through the Aṣṭādhyāyī's practice; codified in the paribhāṣā tradition on term continuation (Kielhorn ed.) `[verify numbers]`; standard discussions in Joshi–Roodbergen introductions `[verify]`. |
| Translation sketch | "Carrying-forward": what a governing rule states continues to apply to the operations it governs. |
| Interpretive assumptions | (a) Persistence is default-until-cancelled; (b) cancellation is explicit (a new statement or terminating rule). Debates: scope of anuvṛtti across sūtra boundaries; interaction with adhikāra termination `[verify]`. |
| Computational correspondence | Inherited context = properties transmitted along declared paths to descendants. **Limits:** anuvṛtti carries word-meanings of technical terms forward inside one grammar; our mechanism transmits typed properties along explicit edges with per-path permission lists, pre-materialization blocks, and indefeasible commitment — a different, richer machinery that only *resembles* anuvṛtti at the metaphor level. Direction also differs: grammar persists terms downward in derivation order; ours propagates properties across an inheritance DAG at evaluation time. |
| Prior-art subtraction | Kill screen F7/F8/F9: nonmonotonic inheritance networks, F-logic override, default unification cover it. Residual: none unique; R2 (blocked-path counterfactual recording) is engineering hardening. |
| Proposed disposition | **Approve as inspiration-only** (Generic label). |

**Reviewer decision:** Approve / Relabel / Reject — Name: ______ Signature: ______ Date: ______ Notes: ______

---

## MC-3 — Default + protected exception ← *utsarga–apavāda*

| Field | Content |
|---|---|
| Ledger row | Default and protected exception — "Utsarga–apavāda-inspired engineering hypothesis" |
| Primary sources | The interpretive doctrine of general rule (*utsarga*) and restricting exception (*apavāda*) in Mīmāṃsā and dharma interpretation; exceptions defeat the general rule only within their specified domain. Standard references: Śabara-bhāṣya and Tantravārttika passages on utsarga-apavāda relations `[verify loci]`; Kane, *History of Dharmaśāstra*, interpretation-theory discussion `[verify vol/page]`. Grammatical reflex: vipratiṣedha resolution where the specific prevails. |
| Translation sketch | The general prescription applies unless a specific exception restricts it; the exception is not a second general rule but a bounded override. |
| Interpretive assumptions | (a) Exceptions must be specific and grounded relative to the general case; (b) absent an exception, the utsarga operates. Debates: how far an apavāda extends; priority ordering between multiple apavādas `[verify]`. |
| Computational correspondence | Defeasible default applies generally; exception defeats it within a stated condition. **Limits:** the tradition resolves conflicts via ordered principles (specificity, later-rule precedence), not instance-grounded defeat records; our exceptions target exact `(rule_id, substitution)` pairs — finer-grained than anything in the tradition. The correspondence justifies the vocabulary "protected exception" as inspiration, nothing stronger. |
| Prior-art subtraction | Kill screen F1–F4, F6: Reiter defaults, defeasible logic, ASPIC+ undercutting, courteous LP all cover default-plus-exception machinery. Residual: R1 (grounded-instance locality) — engineering refinement, generically statable. |
| Proposed disposition | **Approve as inspiration-only** (Generic label). |

**Reviewer decision:** Approve / Relabel / Reject — Name: ______ Signature: ______ Date: ______ Notes: ______

---

## MC-4 — Explicit precedence ← rule-order tradition

| Field | Content |
|---|---|
| Ledger row | Explicit precedence — "Pāṇinian-informed and broadly procedural; candidate organization, not unique primitive" |
| Primary sources | Kielhorn PP 12 *vipratiṣedhe paraṃ kāryam* ("when two rules conflict, the later applies") `[verified-high]`; supporting principles: antaraṅga–bahiraṅga, nitya–anitya, apavāda-over-utsarga ordering `[verify standard loci]`. |
| Translation sketch | Under conflict, the later-stated operation wins. |
| Interpretive assumptions | Precedence in Pāṇini is *derived* from several ordered principles rather than stored as an explicit edge set. Debates: relative ranking of the ordering principles themselves `[verify]`. |
| Computational correspondence | Acyclic typed priority relation resolving conflicting grounded applications. **Limits:** ours is first-class, conditional, pattern-aligned, and instantiated post-filtering; the tradition's is implicit in rule sequence plus meta-principles. Analogy only. |
| Prior-art subtraction | Kill screen F2: superiority relation in defeasible logic kills any residual claim. Residual: none. |
| Proposed disposition | **Approve as inspiration-only**; ledger wording already concedes non-uniqueness. |

**Reviewer decision:** Approve / Relabel / Reject — Name: ______ Signature: ______ Date: ______ Notes: ______

---

## MC-5 — Optional alternatives ← *vā* optionality

| Field | Content |
|---|---|
| Ledger row | Optional alternatives — "Pāṇinian-informed and broadly procedural" |
| Primary sources | The particle *vā* marking optional operations throughout the Aṣṭādhyāyī (e.g., pragṛhya and sandhi alternatives) `[verified-high as convention; verify illustrative sūtras]`; scholarly treatments of optionality in Pāṇinian derivations `[verify]`. |
| Translation sketch | "Or": either application yields a valid derivation. |
| Interpretive assumptions | Options yield equally valid alternative derivations; some schools treat certain options as contextually ranked. Debates: whether all vā-options are genuinely symmetric `[verify]`. |
| Computational correspondence | Bounded choice group enumerated pre-inference into parallel branches, aggregated skeptically. **Limits:** Pāṇinian options live inside one accepted derivation; ours preserve alternatives as simultaneous branches with query-level aggregation — a different consumption model motivated by auditability. |
| Prior-art subtraction | Kill screen F3: ASP choice rules kill novelty. Residual: none. |
| Proposed disposition | **Approve as inspiration-only.** |

**Reviewer decision:** Approve / Relabel / Reject — Name: ______ Signature: ______ Date: ______ Notes: ______

---

## MC-6 — Property-specific blocking ← weak historical analogue

| Field | Content |
|---|---|
| Ledger row | Property-specific blocking — "Pāṇinian/Sanskrit-informed and generic non-monotonic control" |
| Primary sources | No direct Aṣṭādhyāyī counterpart identified by the drafter. Nearest interpretive notions: *bādha* (overriding prohibition) in Mīmāṃsā/dharma analysis; lexicalized-compound behavior resisting compositional inheritance as a folk analogue `[all verify — historicity weak]`. |
| Translation sketch | A specific prohibition stops a general transmission without touching siblings. |
| Interpretive assumptions | If any: prohibitions are domain-bounded overrides. This card is the weakest historically. |
| Computational correspondence | Path-level suppression of exactly one property on one edge/path pattern while parallel paths and unrelated properties continue. **Limits:** largely retrojective; the mechanism is honestly a generic non-monotonic device (Horty/Touretzky exception links, F-logic override). |
| Prior-art subtraction | Kill screen F7/F8 fully cover. Residual: none. |
| Proposed disposition | **Relabel** — drop "Pāṇinian-informed"; classify purely Generic in the TreatmentSignature provenance table. |

**Reviewer decision:** Approve / Relabel / Reject — Name: ______ Signature: ______ Date: ______ Notes: ______

---

## Excluded legacy mappings (no cards required — Doc 08 §7.4)

Recorded to prevent scope creep: *it-marker*-like hidden control semantics and *asiddha*-like temporary-state isolation are **excluded** from PDSGRO-0.1 and may never be cited as claimed contributions; generic rule stratification must not be rebranded as asiddha evidence.

---

## Reviewer workflow

1. Verify every `[verify]` tag against the cited editions; correct or strike.
2. Give per-card Approve / Relabel / Reject with notes; any Reject names the offending claim text.
3. Confirm the excluded-mappings paragraph matches your understanding of §7.4.
4. Sign each card; the signed set joins the M0 freeze package and binds TreatmentSignature §5 wording.
5. Amendment coupling: if MC-6's Relabel is ratified (blocking → purely Generic), TreatmentSignature §5 and the Doc 08 §6.5 ledger wording change via a versioned amendment with rehash (§23.5) — never silently.

---

## MC-7 — Predicate-participant / event-role carrier ← *kāraka* doctrine (held constant)

| Field | Content |
|---|---|
| Ledger row | Predicate-participant/event-role carrier — "Pāṇinian-informed linguistic representation, **held constant here**" |
| Primary sources | Kāraka definitions in the Aṣṭādhyāyī 1.4.23–1.4.55 (*kārakam*, *dhruvam apāye 'pādānam*, *sādhakatamaṃ karma*, etc.) `[verify individual loci]`; vibhakti-to-kāraka mapping tradition; computational line: Kulkarni et al. dependency/kāraka parsing `[verified-high as prior art]`. |
| Translation sketch | Participants are classified by their relation to the action (independent of surface case expression). |
| Interpretive assumptions | The neutral bundle's `NeutralEvent`/`NeutralRoleEdge` objects encode a role-type layer abstracted from this doctrine. Debates about kāraka inventory boundaries do not affect M0/M1 because the carrier is shared by every condition. |
| Computational correspondence | Typed events with role edges = predicate-centred participant structure. **Limits:** no claim that the bundle implements Pāṇinian kāraka theory faithfully; it borrows only the participant-role abstraction. Because the carrier is held constant across target, universal, and generic conditions, it can contribute **no differential causal effect** (Doc 08 §6.3). |
| Prior-art subtraction | Not applicable — carrier is not part of the treatment locus. |
| Proposed disposition | **Approve as held-constant provenance**; no uniqueness or superiority claim permitted at any gate (§7.5 already bars event-role claims from M0/M1 results). |

**Reviewer decision:** Approve / Relabel / Reject — Name: ______ Signature: ______ Date: ______ Notes: ______
