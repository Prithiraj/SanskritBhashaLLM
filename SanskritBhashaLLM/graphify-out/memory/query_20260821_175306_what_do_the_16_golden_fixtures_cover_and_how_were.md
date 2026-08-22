---
type: "query"
date: "2026-08-21T17:53:06.498485+00:00"
question: "What do the 16 golden fixtures cover and how were they validated?"
contributor: "graphify"
outcome: "useful"
source_nodes: ["Public Golden Fixtures DQ1-M0-F01 to F16"]
---

# Q: What do the 16 golden fixtures cover and how were they validated?

## Answer

m0-artifacts/fixtures/ contains F01-F16 per Doc 08 section 16.1: scope-inactive+isolation, inheritance, property-block with second-path survival, default-only, grounded-exception locality, precedence chain with ordering-only transitive pairs, precedence tie CONFLICT, optionality branches, analysis ambiguity AMBIGUOUS, two-group Cartesian product, NO_VALID_ANALYSIS, conflict matrix (source/strict/default hierarchy), constraint stratum timing, 4 malformed-cycle compiled-instance variants fail-closed, deterministic resource exhaustion at branch_limit, and the combined clean-room library world with frozen query may_borrow(researcher,vel)=CONTRADICTED exactly as section 16.2 pins. Fixture-driven schema amendment v0.1.1: analyses gained assumed_fact_refs for branch-local sense assumptions; request-context predicates convention (ctx_special_collections) pinned in README. Validation: 15/15 source bundles OK against source schema, 4/4 F14 compiled variants OK against compiled_instance schema (initial f14a failure - scopes are compiled-layer - caught and fixed).

## Outcome

- Signal: useful

## Source Nodes

- Public Golden Fixtures DQ1-M0-F01 to F16