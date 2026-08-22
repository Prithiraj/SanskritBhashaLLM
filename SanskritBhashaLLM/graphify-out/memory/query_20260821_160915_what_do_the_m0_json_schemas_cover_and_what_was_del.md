---
type: "query"
date: "2026-08-21T16:09:15.492155+00:00"
question: "What do the M0 JSON schemas cover and what was deliberately left to the validator?"
contributor: "graphify"
outcome: "useful"
source_nodes: ["M0 JSON Schema Pack v0.1 (6 schemas)"]
---

# Q: What do the M0 JSON schemas cover and what was deliberately left to the validator?

## Answer

Six Draft-2020-12 schemas in m0-artifacts/schemas/ all metaschema-valid: common defs (incl CompilerManifest with MT-1..9 hash map and generic attribution const), source_bundle B (ContextKey with GLOBAL reserved via not-const, analysis groups cardinality=1, task theory claim forms), compiled_instance I_m (scope forest, inheritance edges with permitted_properties, rules strict|default + stratum, grounded exceptions, blocks, priority edges with alignment, optional groups, constraints), model_payload (additionalProperties=false + allOf-not prohibition of query_results/fired_rules/proofs/gold fields), execution_audit (tagged union; COMPLETE requires EVALUATED+hash; INVALID/EXHAUSTED carry no answers; exhausted_counter enum), telemetry_manifest (mandatory zeros as const 0). Semantic rules (variable safety, acyclicity, stratification, overlap) deliberately left to M1 validator per README.

## Outcome

- Signal: useful

## Source Nodes

- M0 JSON Schema Pack v0.1 (6 schemas)