# Review Operations — Shared Rules for DQ1-M0 Reviewers

**Version:** 0.1 · **Date:** 21 August 2026 · **Status:** Operational aid (not a governing contract)
**Governing documents:** Doc 08 §§18, 23; Doc 07 §11

---

## 1. The four roles and what each signature unlocks

| Role | Owns | Key inputs | Authority clause |
|---|---|---|---|
| Mechanism owner | Completeness, feasibility, artifact assembly | All M0 artifacts | Doc 08 §23.2 |
| Sanskrit/Pāṇinian reviewer | Historical/linguistic mapping honesty | Mapping cards, microfixture, TreatmentSignature §5 | §16.3, §23.2 |
| Independent methods reviewer | Treatment boundary, leakage, controls, stop rules, kill-screen verification | Docs 07+08, artifacts 09–11 | §18.1, §23.2 |
| Independent implementation reviewer | Independent implementability, code/tests/reproducibility (M1), no hard-coding | Compile_T spec, schemas, later M1 code | §19–22, §23.2 |

**Quorum rule:** M0 becomes Frozen only when all four approve **the same normative artifact hash**. Approval of different revisions does not form a quorum (Doc 08 §23.2).

## 2. Independence requirements

The three reviewers other than the mechanism owner must be independent of:

- target implementation (no authorship of PDSGRO code/spec);
- outcome-dependent authorship (no stake in whether the candidate passes).

Disclose prior collaboration with the owner or each other before accepting. Disclose any funding or employment relationship touching the programme.

## 3. Verdict vocabulary and record format

Per artifact, each reviewer records:

~~~text
Reviewer / role:
Artifact + SHA256:
Verdict: Approve | Amend | Reject
Blocking findings (numbered, each with clause reference):
Non-blocking notes:
AI-assistance disclosure (tools used, which findings are human-verified):
Date:
~~~

"Amend" must list every blocking finding with the exact clause it violates. A verdict without clause-referenced findings is not recordable.

## 4. AI-assistance policy (three tiers)

| Tier | Use | Rule |
|---|---|---|
| 1 — Autopilot | Mechanical checks: cross-references, schema validation, hash integrity, status-column audits | Output logged as advisory artifact; no human action needed unless it flags |
| 2 — AI drafts, human decides | Red-team passes, citation verification leads, fixture expected-output derivations, mapping-card drafts | Human reviewer must independently verify each finding they rely on; disclosure mandatory |
| 3 — Human only | All four signatures; microfixture approval; hidden-fixture custody; relabel ratification | No AI may hold the pen |

**Correlated-blindness mitigation:** when AI assisted artifact *authoring* (as it did for 09–11), reviewers should use a *different* model/vendor for AI-assisted review passes, and treat model-agreement as neither necessary nor sufficient for their verdict.

## 5. Effort scoping (honest estimates)

| Role | Current queue | Estimated first-pass effort |
|---|---|---|
| Sanskrit/Pāṇinian | TreatmentSignature §5; mapping-card framework; microfixture commissioning | 4–8 h |
| Methods | Docs 07–08 alignment; kill screen citations; TreatmentSignature §6.1 test; Compile_T O5–O7 witnesses | 8–16 h |
| Implementation | Compile_T spec implementability; (later) M1 code, tests, reproducibility | 4 h now; 20–40 h at M1 |
| Owner | Assembly, hash manifest, custody setup | ongoing |

## 6. Amendment flow after findings

Findings → owner disposition record → new artifact version + rehash → re-review of changed clauses only → fresh quorum attempt. Typographic-only changes take patch versions but still rehash (Doc 08 §23.5).

## 7. Current review queue (as of 21 Aug 2026)

| Artifact | Status | Needs |
|---|---|---|
| 09_M0_Prior_Art_Kill_Screen_Matrix_v0.1.md | Draft, unverified citations | Methods (checklist in its §7) |
| 10_M0_TreatmentSignature_v0.1.md | Draft | Methods §6.1 test; Sanskrit §5 wording |
| 11_M0_Compile_T_Specification_v0.1.md | Draft skeleton | Methods + Implementation |
| Doc 08 v0.2 itself | Pass-2 aligned, not Frozen | All four roles |
