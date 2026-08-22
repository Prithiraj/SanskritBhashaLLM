# DQ1-M0 Consolidated Review Checklist

## Pre-Freeze Verification Sheet (Doc 08 §17, §18.1, §23.3)

**Version:** 0.1 — Draft · **Date:** 22 August 2026
**Use:** one sheet per reviewer; completed sheets join the freeze package. Every line cites its authority; an unticked box blocks Freeze.

## A. Contract & boundary (methods reviewer)

- [ ] Doc 08 v0.2 reviewed in full; no unresolved semantic TBDs (§18.1)
- [ ] TreatmentSignature §2 constraints statable without Sanskrit terminology; §6.1 relabel test passes *as Generic*
- [ ] Kill screen citations verified or struck; Generic recommendation ratified or overturned (09 §7)
- [ ] Estimands separate: semantic-equivalence vs resource-equivalence never conflated (§5.4)
- [ ] Public-claim language ≤ implemented boundary (§7.5); excluded legacy mappings intact (§7.4)

## B. Formal semantics & schemas (methods + implementation reviewers)

- [ ] All six schemas metaschema-valid; §9 object inventory complete (28/28 rows)
- [ ] Aggregated vs branch-local status enums correct (BOTH branch-local only)
- [ ] ModelPayload prohibitions structurally enforce §15.1; audit union enforces §19.4
- [ ] Compile_T obligations O1–O7 witnessed; metamorphics M-Q/K/O/R/I specified
- [ ] Operational-semantics artifact exists as **separate normative file** (currently outstanding) and refines without contradicting Doc 08 §§9–10

## C. Fixtures & custody (implementation reviewer + custodian)

- [ ] F01–F16 bundles schema-valid; oracles independently hand-derived by ≥1 reviewer (§18.1)
- [ ] F14 variants fail-closed at compiled layer; placeholder hashes noted for replacement at freeze
- [ ] Custody spec complete: bounds, coverage matrix, 100% semantic threshold, mutation kill set, seed commitment/escrow, unseal event, disjointness registry
- [ ] Custodian + witness named with keys before generation (spec §1)

## D. Attribution provenance (Sanskrit/Pāṇinian reviewer)

- [ ] MC-1…MC-7 each decided Approve/Relabel/Reject with notes
- [ ] `[verify]` loci checked against editions; corrections recorded on cards
- [ ] MC-6 disposition (blocking → purely Generic?) ratified → if Relabel, TS §5 + ledger amendment queued under §23.5
- [ ] Attested microfixture authored/approved and added to fixture set (§16.3)
- [ ] Excluded-mappings paragraph confirmed against §7.4

## E. Controls & fairness (methods reviewer + U/G builders)

- [ ] Charter approved; U **and** G builders signed the §3 I/O contract pre-freeze (§18.1)
- [ ] CT-1…CT-6 accepted as absolute gates in writing
- [ ] Owner disclosure register delivered to builders; sufficiency floors certified
- [ ] No target-only mandatory state in shared interface; veto rights acknowledged

## F. Freeze mechanics (owner + all)

- [ ] All artifacts hashed per manifest scheme (`version_hash_manifest_v0.1.md`)
- [ ] Four governance signatures + U/G builder signatures on the **same normative hash** (§23.2 quorum)
- [ ] Disclosure register published inside package
- [ ] Outstanding-artifact gate: every `TBD` role in the manifest template is resolved (operational-semantics file, Decode_T witnesses, review records, disclosure register, custodian/witness names); no checkbox above unticked
