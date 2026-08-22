---
type: "query"
date: "2026-08-22T16:00:19.109650+00:00"
question: "What did the two review cycles cover and what does the operational-semantics artifact pin?"
contributor: "graphify"
outcome: "useful"
source_nodes: ["Operational Semantics v0.1 (OS rules)"]
---

# Q: What did the two review cycles cover and what does the operational-semantics artifact pin?

## Answer

Cycle A on checklist+manifest: Pass 1 found manifest missing 7 section23.3 rows (mapping/configuration, Decode_T witnesses, cost-counter, traceability, compiler-interface, review records) and hardcoded checklist section-F states - fixed; first fix attempt silently no-opped on wrong anchor (caught by pass-2 recheck), corrected against real file content; Pass 2 ALIGNED with full inventory present. Then built m0-artifacts/operational_semantics_v0.1.md: rule families OS-V(10) OS-B(4) OS-S(5) OS-I(5) OS-E(12, mirroring Doc08 section10.5 steps) OS-C(3) OS-R(4, normative counter definitions making F15 determinate) OS-A(7 skeptical-v1 pseudocode) OS-T(5 canonical ordering/output separation); pinned-decisions table D-1..D-14 resolving previously implicit choices (request-context predicates, assumed-fact injection at stratum 0 as indefeasible branch-local source support, ground sort order BLOCK<EXCEPTION<INDEFEASIBLE_OPPOSITION<PRIORITY, alignment semantics, anti-circular activation); F06 worked micro-trace matches oracle. Cycle B Pass 1 found D-15 dangling reference (fixed); apparent failures OS-R/OS-T/R1 were checker artifacts (first-occurrence split + wording), corrected checker; Pass 2 ALIGNED.

## Outcome

- Signal: useful

## Source Nodes

- Operational Semantics v0.1 (OS rules)