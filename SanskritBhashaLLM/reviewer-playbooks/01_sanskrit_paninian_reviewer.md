# Playbook — Sanskrit/Pāṇinian Reviewer (DQ1-M0)

**Version:** 0.1 · **Date:** 21 August 2026
**Your mandate:** protect the programme from overclaiming Sanskrit/Pāṇinian attribution; approve only mappings you would defend to a śāstric scholar.
**You are NOT reviewing:** code, statistics, or engineering feasibility.

---

## 1. Required reading (in order)

1. Doc 08 §§5.4–6.5 (attribution estimands + ledger), §7.4 (excluded legacy mappings), §16.3 (microfixture + mapping cards), §18.1 (mapping-approval exit criteria)
2. TreatmentSignature v0.1 — especially §5 (inspiration provenance) and §2 `attribution_label`
3. Kill Screen Matrix v0.1 §4 (Sanskrit-computational prior art: Huet Heritage engine, Saṃsādhanī simulator, Vidyut prakriyā)

## 2. Your decisions

### D1 — Attribution-label ratification
Confirm or amend: `generic_sanskrit_inspired_scope_machinery` with Pāṇinian content as inspiration-only.
*Test:* would you sign a public statement that the implementation does **not** reproduce the Aṣṭādhyāyī and claims no uniqueness from it?

### D2 — Mapping cards (one per retained Pāṇinian-labelled claim)
Each card must contain (Doc 08 §16.3): authoritative source citation + translation; interpretive assumptions; competing scholarly analyses; exact computational correspondence **and its limits**; residual claim after prior-art subtraction; your Approve/Relabel/Reject.
Current card set: adhikāra→scope, anuvṛtti→inheritance, utsarga–apavāda→default/exception (TreatmentSignature §5). AI can draft cards for your markup; the verdict is yours alone.

### D3 — Attested microfixture commissioning
One compact real example exercising ≥1 mapping with genuine ambiguity or protected exception (Doc 08 §16.3). You author or explicitly approve it; it must not embed the benchmark answer. *This decision cannot be delegated to AI.*

## 3. Red flags that must trigger Relabel/Reject

- Any wording implying the mechanism is uniquely Pāṇinian or historically authentic;
- A mapping whose computational correspondence ignores scholarly disagreement;
- Inspiration language migrating into normative sections (§2 of the signature);
- Claims about kāraka/morphology layers outside the M0 boundary (§7.5).

## 4. Standing question for you

Is there an attested passage you consider a clean instance of scope-governed rule application with a protected exception, suitable as the microfixture? If yes, propose it; if no, say so plainly — a negative answer is a valid record and the fixture waits.

## 5. Record

Use the shared verdict template in `00_REVIEW_OPERATIONS.md` §3. Disclose AI assistance per §4.
