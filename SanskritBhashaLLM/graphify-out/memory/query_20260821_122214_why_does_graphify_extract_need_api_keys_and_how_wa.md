---
type: "query"
date: "2026-08-21T12:22:14.770680+00:00"
question: "Why does graphify extract need API keys and how was Doc 08 indexed without one?"
contributor: "graphify"
outcome: "useful"
source_nodes: ["DQ1-M0 Mechanism Specification Freeze", "PDSGRO-0.1 Paninian-Derived Scope-Gated Rule Organizer", "ModelPayload Pre-Solution Artifact"]
---

# Q: Why does graphify extract need API keys and how was Doc 08 indexed without one?

## Answer

graphify extract calls an external LLM API for semantic extraction; no key and no active claude subscription existed. Instead the opencode agent performed the semantic extraction itself and wrote 22 nodes + 24 links + 1 hyperedge for Doc 08 directly into graph.json following the existing schema (id prefix 08_dq1_mechanism_resolution_m0_m1_contract_). Doc 08 M0/M1/PDSGRO machinery is now queryable; manifest.json left untouched so a future keyed extraction can still canonicalize hashes.

## Outcome

- Signal: useful

## Source Nodes

- DQ1-M0 Mechanism Specification Freeze
- PDSGRO-0.1 Paninian-Derived Scope-Gated Rule Organizer
- ModelPayload Pre-Solution Artifact