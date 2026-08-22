# Prior-Art Kill Screen Matrix

## DQ1-M0 Required Artifact for PDSGRO-0.1

**Document type:** DQ1-M0 artifact (Doc 08 §17 row: "prior-art kill-screen matrix")
**Version:** 0.1 — Draft for verification
**Date:** 21 August 2026
**Candidate under test:** Pāṇinian-Derived Scope-Gated Rule Organizer, version 0.1 (PDSGRO-0.1)
**Authority:** Document 08 §§6.1, 17, 18.1, 26; Document 06 DQ1
**Status:** AI-drafted from model knowledge. **Every citation and coverage claim below requires verification by the independent methods reviewer before this matrix can support an M0 Freeze decision.** Confidence tags are per-row.

---

# 1. Purpose and Verdict Rules

This matrix answers one question from Doc 08 §6.1:

> Is PDSGRO-0.1 representationally or organizationally isomorphic to the strongest identified prior generic compiler, leaving **no residual target-only factorization, topology, indexing, or mediation constraint** after prior-art subtraction?

## 1.1 Decision rule

| Outcome after subtraction | Consequence (Doc 08 §6.1 / §18.3) |
|---|---|
| Residual is empty, or expressible only with Sanskrit terminology | Relabel **Generic Sanskrit-inspired scope machinery**; engineering continues under downgraded attribution |
| Residual states a non-isomorphic organizational constraint (factorization, topology, indexing, or mediation) testable against controls | Retain **Pāṇinian-labelled residual hypothesis**; carry residual into TreatmentSignature |
| Behaviour depends on undefined authenticity or hidden judgment | Stop condition, not a relabel |

## 1.2 Subtraction procedure

For each prior family: (1) name closest systems; (2) map their constructs onto PDSGRO primitives; (3) record what they demonstrably do **not** provide; (4) state what remains of each PDSGRO claim after removing everything the family already covers. The residual across **all** families, not any single family, decides the label.

## 1.3 Threat levels

- **KILL** — family provides an organizationally equivalent construct; primitive cannot be claimed as target-only.
- **STRONG** — near-equivalent construct exists; only minor parameterization differs.
- **PARTIAL** — related construct with materially different semantics.
- **WEAK** — no meaningful counterpart.

---

# 2. Claim Side: PDSGRO-0.1 Primitive Inventory

From Doc 08 §§5–11 (attribution ledger, schema, operational semantics):

| # | Primitive (ledger label) | Claimed source inspiration | Core computational content |
|---|---|---|---|
| P1 | Governing scope | Adhikāra | Rooted scope forest, ≤1 parent, activation conditions, path-only fact visibility |
| P2 | Inherited context | Anuvṛtti | Property transmission along permitted inheritance paths |
| P3 | Default + protected exception | Utsarga–apavāda | Defeasible rules; exceptions targeting exact grounded `(rule_id, substitution)` pairs |
| P4 | Property-specific blocking | Generic non-monotonic control | Path-level suppression of one property on one edge/path pattern |
| P5 | Explicit precedence | Broadly procedural | Acyclic priority over grounded applications via substitution patterns + argument alignment |
| P6 | Optional alternatives | Broadly procedural | Bounded non-overlapping choice groups enumerated pre-inference |
| P7 | Ambiguity preservation | Śābdabodha-adjacent | Analysis groups; Cartesian branch product; no silent collapse |
| P8 | Conflict semantics | Paraconsistent | FOUR-state truth (TRUE/FALSE/NEITHER/BOTH); conflict query-specific at aggregation |
| P9 | Stratified evaluation | Generic | Strict/default stratification; lower-stratum conclusions never retracted |
| P10 | Deterministic audit + resource accounting | Generic engineering | Canonical traces, counters, exhaustion status, hashed artifacts |

P9 and P10 are already classified generic by Doc 08 itself; they are listed for completeness only.

---

# 3. Family-by-Family Analysis

## F1. Reiter Default Logic

Closest systems: Reiter, "A Logic for Default Reasoning," *Artificial Intelligence* 13 (1980). Variants: justified/constrained/rational (Mikitiuk & Truszczynski; Delgrande et al.).

| PDSGRO primitive | Coverage | Notes |
|---|---|---|
| P3 defaults | STRONG | Defaults α:β/γ with consistency justifications are the canonical formalism |
| P3 protected exceptions | PARTIAL | Exceptions = failed justification (global consistency check); **no named-target grounding of an exception to one `(rule_id, substitution)` application** |
| P5 precedence | WEAK | No priority mechanism; multiple extensions instead of resolved conflicts |
| P1/P2/P4/P6/P7 | WEAK | Absent |

Residual after subtraction: grounded-exception locality; precedence; scopes; inheritance blocking; optionality-as-branches.

## F2. Defeasible Logic (Nute; Antoniou–Billington)

Closest systems: Nute (1987–1994); Antoniou, Billington, Governatori & Maher, defeasible logic framework (DL, d-prolog lineage; *AIJ* and KI papers c. 1996–2001). Implementations: SPIDDLE, Deimos, Flora-2 `defeasible` package, Nute's PROLOG implementations.

| Primitive | Coverage | Notes |
|---|---|---|
| P3 defaults | STRONG | Defeasible rules r: d ⇒ c are core |
| P3 exceptions | STRONG | Exception rules (`⇸`) defeat conclusions; but target **conclusions/predicates**, not grounded application instances |
| P5 precedence | **KILL** | The **superiority relation** ρ on rule *labels* resolves conflicting applicable rules — same role as PriorityEdge |
| P8 conflict | PARTIAL | DL is skeptical and paraconsistent-tolerant in some variants, but no explicit BOTH-support aggregation policy |
| P1/P2/P4/P6/P7 | WEAK | No scopes, inheritance paths, blocks, or choice groups |

Residual: superiority ≈ P5 kills the precedence claim. Remaining: instance-level (not rule-level) exception targeting; scopes; inheritance+blocking; optionality.

## F3. Answer Set Programming

Closest systems: Gelfond & Lifschitz stable models (1988); ASP solvers (clingo/gringo, DLV). Constructs: strong negation, choice rules, weak constraints, optimization, preferences (Sakama & Inoue, "Prioritized logic programming," 1996; Brewka et al. ordered disjunction/preferences).

| Primitive | Coverage | Notes |
|---|---|---|
| P3 defaults | STRONG | Negation-as-failure defaults; strong negation for explicit falsity |
| P6 optionality | **KILL** | Choice rules `{a;b}=1..k` enumerate answer sets — same generate step as OptionalGroups |
| P7 ambiguity | STRONG | Multiple answer sets = preserved alternatives; projection/aggregation is post-hoc |
| P5 precedence | STRONG | Preference orders on rules/answer sets (well-studied) |
| P8 conflict | PARTIAL | Inconsistent programs typically have no answer set; paraconsistent ASP variants exist (e.g., Belnap-annotated) but are not mainstream |
| P1/P2/P4 | WEAK | No built-in scoped visibility or path-blocked inheritance |

Residual: scopes; inheritance-path blocking; grounded-instance exception locality; deterministic audit semantics (ASP solving is not audit-oriented).

## F4. Courteous Logic Programs / RuleML

Closest systems: Grosof, Labrou & Chan, "A Declarative Approach to Business Rules in Courteous Logic Programs" (AAAI 1999 era); IBM CommonRules; RuleML courteous extensions.

| Primitive | Coverage | Notes |
|---|---|---|
| P3+P5 | **STRONG→KILL** | Prioritized defaults + **mutual-exclusion handlers** with priority resolution of conflicts; explicitly designed for "exceptions with precedence" business rules |
| P8 conflict | STRONG | Courteous semantics guarantees consistent conclusions by prioritized conflict elimination — opposite design goal to PDSGRO's conflict *preservation* |
| P1/P2/P4/P6/P7 | WEAK | Not provided |

Residual: PDSGRO deliberately *preserves* unresolved conflicts (CONFLICT/BOTH) where courteous LP *eliminates* them; that is a genuine semantic difference, but it is a **generic** paraconsistent-vs-prioritized design axis, not a Pāṇinian one.

## F5. Well-Founded Semantics with Explicit Negation

Closest systems: Pereira & Alferes WFSX (1992); XSB Prolog tabling engine.

| Primitive | Coverage | Notes |
|---|---|---|
| P3 | STRONG | Default negation coexisting with explicit negation; undefined third value |
| P8 | PARTIAL | Three-valued (T/U/F), not four-valued BOTH; no branch-wise aggregation |
| Others | WEAK | |

Residual: minimal beyond F2/F3 findings.

## F6. Structured Argumentation (ASPIC+, Pollock)

Closest systems: Prakken (2010) and Modgil & Prakken (*AIJ* 2013) ASPIC+; Pollock OSCAR. Constructs: strict/defeasible inference rules; rebutting/undercutting defeat; preferences over arguments (last-link/weakest-link).

| Primitive | Coverage | Notes |
|---|---|---|
| P3 | STRONG | Undercutting defeat targets the *inference application*, conceptually close to grounding-local exceptions |
| P5 | STRONG | Argument preferences ≈ precedence among applications |
| P7 | STRONG | Multiple acceptable arguments = preserved alternatives |
| P8 | PARTIAL | Status assignment skeptical; BOTH-style four-valued labelling appears in some AF semantics (e.g., conflict-tolerant labellings) |
| P1/P2/P4/P6 | WEAK | No scopes/inheritance/blocks/choice groups |

Residual: undercutting ≈ instance-level defeat weakens the "grounded exception" novelty further. Remaining: scopes, inheritance+blocking, optionality groups.

## F7. Nonmonotonic Inheritance Networks

Closest systems: Touretzky's Taxonomic Transitive-closure Logarithmic (TTL) theory (1984/86); Horty, Thomason & Touretzky skeptical inheritance (*AIJ* 1990); Etherington & Reiter.

| Primitive | Coverage | Notes |
|---|---|---|
| P2 inheritance | **KILL** | Path-based property transmission along class links is the defining mechanism |
| P4 blocking | **KILL** | **Exception links block propagation on specific paths**; red-herring detection handles preclusion — direct ancestor of property-specific path blocking |
| P3 | PARTIAL | Defeasible path conclusions; not rule-grounding-level |
| P8 | PARTIAL | Skeptical vs credulous split; ambiguous paths yield no conclusion rather than BOTH |
| P1 | PARTIAL | Networks are hierarchic (single-parent-ish trees/DAGs) but without activation conditions or request-context gating |
| P5/P6 | WEAK | |

Residual: activation-conditioned scopes; rule bodies/heads (networks propagate properties, not evaluate conjunctive rules); optionality groups; precedence.

## F8. F-logic / FLORA-2 Frames

Closest systems: Kifer, Lausen & Wu F-logic (JACM 1995); FLORA-2 (Yang, Kifer & Zhao) with dynamic modules, multiple inheritance with override, defeasible rules.

| Primitive | Coverage | Notes |
|---|---|---|
| P2+P4 | STRONG | Inheritance with explicit override/blocking per predicate; non-monotonic multiple inheritance |
| P1 | PARTIAL | **Modules/namespaces gate visibility** — structurally close to scopes, though without activation conditions or single-parent forest discipline |
| P3 | STRONG | FLORA-2 supports defeasible rules with overrides |
| P5 | PARTIAL | Override-by-subclass ordering, not arbitrary acyclic priority patterns |

Residual: activation-conditioned request-gated scopes; grounded-instance exceptions; optionality; audit.

## F9. Grammar Formalisms with Defaults

Closest systems: DATR (Evans & Gazdar, *JNL* 1996); default unification in HPSG — Flickinger's EFG/LKB "efficient default unification" (2000); Carpenter's typed feature structures with default inheritance (1992-ish).

| Primitive | Coverage | Notes |
|---|---|---|
| P2+P4 | STRONG | Default inheritance with per-path override in lexical type hierarchies |
| P7 | PARTIAL | Multiple analyses in parsing lattices, but not first-class branch objects |
| Others | WEAK | |

Note: this family matters because it shows **linguistically-motivated** default+blocking machinery predates the programme; it supports the Doc 08 ledger's own "generic non-monotonic control" classification of P4.

## F10. Production-Rule Systems

Closest systems: OPS5 (Brownston et al. 1985), CLIPS, Jess; modern: **Drools** (salience, agenda-groups, activation-groups, no-loop, lock-on-active), ILOG JRules/ODM.

| Primitive | Coverage | Notes |
|---|---|---|
| P5 | **KILL** | Salience = explicit rule priority; refraction prevents re-firing |
| P1 | **STRONG→KILL** | Drools **agenda-groups** with focus() = runtime-selected active rule scopes; entry-points gate fact visibility — organizationally very close to governing scope + anchor |
| P3 | PARTIAL | Conflicts resolved by salience/recency strategy, not protected exceptions |
| P6 | PARTIAL | Activation-group(max) fires one of a group — crude optionality |
| P7/P8 | WEAK | Working memory has no ambiguity-preservation or paraconsistent states |
| P2/P4 | WEAK | No declarative inheritance-path machinery |

Residual: PDSGRO's differences here are semantic discipline (deterministic total order, auditability, no recency tie-breaks — Doc 08 explicitly bans incidental order) rather than organizational novelty. **Drools agenda-groups are the single strongest scope prior art found and must be cited in the TreatmentSignature subtraction.**

## F11. Scoped / Contextual / Modular Logic Programming (incl. Scoped Datalog)

Closest systems: **scoped Datalog** (module-scoped Datalog dialects and context-logic treatments of Datalog); Miller's modular logic programming (1989); Giordano & Martelli contextual LP / situated LP; multi-context systems (Giunchiglia & Serafini 1994); RDF named graphs + SPARQL datasets (scope via graph selection).

| Primitive | Coverage | Notes |
|---|---|---|
| P1 | STRONG | Context/module scoping of rules and facts is well established; bridge rules between contexts ≈ controlled cross-scope flow |
| P2 | PARTIAL | Bridge-rule propagation is rule-based, not path-permission-based |
| P4 | PARTIAL | Blocking expressed negatively (omit bridge), not as first-class property-specific path block |
| Activation conditions | PARTIAL | Context activation typically static or bridge-guarded; request-context-gated activation with root-to-anchor path validity is a stricter discipline |

Residual: the *combination* of single-parent forest + unique root-to-anchor activation + GLOBAL-only self-activation facts (no circular visibility) is a tightened discipline, arguably engineering hardening rather than new organization.

## F12. Four-Valued / Paraconsistent Reasoning

Closest systems: Belnap's FOUR (1977); bilattice-based annotated logic programming (Blair & Subrahmanian 1988+); Arieli & Avron bilattice consequence.

| Primitive | Coverage | Notes |
|---|---|---|
| P8 | **KILL** | TRUE/FALSE/NEITHER/**BOTH** truth states are exactly Belnap's four values; skeptical-v1 aggregation order is a specific (generic) choice among known bilattice query policies |

Residual: none for P8 as a *mechanism*; only its integration into branch-local audit remains, which is generic engineering.

## F13. Graph Query Engines

Closest systems: Cypher/Gremlin variable-length paths; SPARQL property paths; SHACL shapes.

| Primitive | Coverage | Notes |
|---|---|---|
| P2/P4 traversal mechanics | PARTIAL | Path enumeration and filters exist, but no defeasible semantics, defaults, or conflict states |
| Others | WEAK | |

Verdict: infrastructure, not mechanism competition.

## F14. Stratified Negation

Apt, Blair & Walker (1988); Przymusinski (1989). Already classified generic by Docs 07/08. **KILL** for P9 as claimed novelty; retained only as required termination machinery.

---

# 4. Sanskrit-Computational Prior Art (Attribution-Ledger Specific)

These implement the *inspiration mechanisms themselves* computationally, so they bound what "Pāṇinian-derived" can add:

| System | Mechanism implemented | Threat to ledger rows |
|---|---|---|
| Huet's Sanskrit Heritage derivation engine (INRIA, c. 2000s) | Pāṇinian rule application with **rule-conflict resolution between competing sūtras** during derivation | Governing scope / precedence mappings: mechanisms demonstrably computable outside this programme |
| Saṃsādhanī Aṣṭādhyāyī simulator (Univ. of Hyderabad) | Ordered rule application, adhikāra/anuvṛtti-style context carry-over in prakriyā | Same |
| Vidyut `prakriyā` (ambuda) | Full derivational traces with rule ordering | Same |
| Kulkarni et al. Sanskrit parsing line (kāraka/dependency) | Event-role analysis | Carrier-layer prior art (already held constant) |

Consequence: mapping cards for adhikāra/anuvṛtti/utsarga-apavāda must cite these and state the residual as **organization-for-a-different-consumption-model** (LLM-facing structural channel), not mechanism invention. This aligns with Doc 08's own ledger ("research hypotheses, not claims that these computational primitives originated uniquely in Sanskrit").

---

# 5. Component × Family Coverage Grid

Legend: ● kill-level coverage ◐ partial ○ absent

| Primitive | F1 | F2 | F3 | F4 | F6 | F7 | F8 | F10 | F11 | F12 |
|---|---|---|---|---|---|---|---|---|---|---|
| P1 scope | ○ | ○ | ○ | ○ | ○ | ◐ | ◐ | ● | ● | ○ |
| P2 inheritance | ○ | ○ | ○ | ○ | ○ | ● | ● | ○ | ◐ | ○ |
| P3 default+exception | ● | ● | ● | ● | ● | ◐ | ● | ◐ | ○ | ○ |
| P4 path blocking | ○ | ○ | ○ | ○ | ○ | ● | ● | ○ | ◐ | ○ |
| P5 precedence | ○ | ● | ● | ● | ● | ○ | ◐ | ● | ○ | ○ |
| P6 optionality | ○ | ○ | ● | ○ | ○ | ○ | ○ | ◐ | ○ | ○ |
| P7 ambiguity | ○ | ○ | ● | ○ | ● | ◐ | ○ | ○ | ○ | ◐ |
| P8 BOTH/conflict | ○ | ◐ | ◐ | ● | ◐ | ◐ | ○ | ○ | ○ | ● |

Reading: **every column of PDSGRO primitives is covered at kill or strong level by at least one generic family.** No primitive survives as individually novel.

---

# 6. Residual Claim Candidates After Subtraction

What no single family provides, and only *combinations* approximate:

R1. **Grounded-instance exception locality**: exceptions defeating exactly one `(rule_id, substitution)` application while sibling groundings survive (F2/F6 operate at conclusion/argument level; F1 at justification level).
R2. **Indefeasible-committed inheritance with pre-materialization path blocks**: blocked paths recorded counterfactually, unblocked paths committed as indefeasible support immune to later default/priority defeat (F7/F8 have blocking, but not inside a stratified strict/default evaluator with this commitment semantics).
R3. **Request-gated scope activation discipline**: single-parent forest, unique root-to-anchor validity, GLOBAL-only self-activation facts, off-path isolation (F10/F11 approximate; the tightened no-circularity discipline is parameterization).
R4. **Conflict-preserving branch evaluation packaged with deterministic audit/resource accounting** for information-equivalent comparison as an LLM structural channel (F4/F12 eliminate or abstract conflicts; none target model-facing payload separation).

## 6.1 Honest classification of the residual

R1–R3 read as **tightened parameterizations and integrations of known generic mechanisms**; R4 is an engineering packaging decision. On the current evidence the candidate is **organizationally isomorphic to the union of F2+F7+F10+F11+F12**, and Doc 08 §6.1's relabel trigger ("representationally and organizationally isomorphic to the strongest identified prior generic compiler") is **prima facie satisfied at the combination level**.

## 6.2 Provisional recommendation

**Relabel PDSGRO-0.1 as "Generic Sanskrit-inspired scope machinery"** unless the TreatmentSignature can articulate a target-only constraint that survives §6.1 — i.e., a factorization/topology/indexing/mediation property that changes a *measured mediator* (irrelevant rule activation, invalid candidate propagation, active structural context size, avoidable branching) relative to the strongest competent combination control, and that cannot be restated without Sanskrit terminology.

Per Doc 08 §18.3, genericity is an attribution result, not an engineering failure: M1 implementation proceeds unchanged either way; only public claim language narrows.

---

# 7. Reviewer Verification Checklist

Before this matrix may support an M0 Freeze decision, the independent methods reviewer must:

1. Verify each citation's bibliographic details (author/year/venue marked from model knowledge; several need page-level confirmation).
2. Spot-check the three highest-threat claims: **Drools agenda-groups ≈ P1**; **Antoniou–Billington superiority ≈ P5**; **Horty/Touretzky exception links ≈ P4**.
3. Run supplementary searches for anything newer than training data (2024–2026): "scoped defeasible logic", "context-aware rule engines LLM structure channels", "paraconsistent rule audit frameworks".
4. Confirm no patent/licence encumbrance affects reimplementing the covered mechanisms.
5. Record the relabel decision (or residual retention with named constraint) in the M0 freeze package with hashes.

**Search queries executed by drafting agent:** none (offline knowledge pass). All literature search is pending reviewer tooling.

---

# 8. Amendment Log

| Version | Date | Change | Author | Status |
|---|---|---|---|---|
| 0.1 | 21 August 2026 | Initial matrix: 14 families, grid, residual R1–R4, provisional relabel recommendation | AI-drafted (opencode agent) | Draft — unverified |
