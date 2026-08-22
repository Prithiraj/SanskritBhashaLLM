# M0 Artifacts — Master Index and Status

**Programme:** Sanskrit-Derived Efficient LLM · **Work package:** DQ1-M0 (Doc 08)
This file indexes every DQ1-M0 artifact and mirrors Doc 08 §17 status. Rows here do not modify the contract; §17 remains owner-maintained.

## 1. Artifact inventory (Doc 08 §17 cross-reference)

| Doc 08 §17 artifact row | File(s) here | Status |
|---|---|---|
| M0 normative contract | `../08_DQ1_Mechanism_Resolution_M0_M1_Contract.md` | Draft |
| TreatmentSignature | [`../10_M0_TreatmentSignature_v0.1.md`](../10_M0_TreatmentSignature_v0.1.md) — machine-readable YAML in §2; provenance table §5 (7 rows incl. carrier) | Draft |
| Target compiler package | [`../11_M0_Compile_T_Specification_v0.1.md`](../11_M0_Compile_T_Specification_v0.1.md) + mapping tables MT-1…MT-9 inventory | Spec Draft; implementation Missing |
| Canonical source JSON Schema | [`schemas/source_bundle.schema.json`](schemas/source_bundle.schema.json) | Draft v0.1.1 |
| Target representation JSON Schema | [`schemas/compiled_instance.schema.json`](schemas/compiled_instance.schema.json) | Draft v0.1.1 |
| Operational semantics | [`operational_semantics_v0.1.md`](operational_semantics_v0.1.md) — normative rules OS-V/B/S/I/E/C/R/A/T + pinned-decisions table D-1…D-14 + F06 worked trace | Draft |
| ModelPayload schema | [`schemas/model_payload.schema.json`](schemas/model_payload.schema.json) | Draft |
| ExecutionAudit schema | [`schemas/execution_audit.schema.json`](schemas/execution_audit.schema.json) | Draft |
| TelemetryManifest schema | [`schemas/telemetry_manifest.schema.json`](schemas/telemetry_manifest.schema.json) | Draft |
| Attribution ledger | Within Doc 08 §6.5 + provenance binding in TS §5 | Draft within contract |
| Mapping-card set | [`mapping_cards_v0.1.md`](mapping_cards_v0.1.md) — MC-1…MC-7, per-card decision blocks | Draft; ~34 citation loci flagged `[verify]` for Sanskrit reviewer |
| Claim traceability table | Doc 08 §13 (draft) + TS §3 C1–C8 constraint→mediator rows | Draft within artifacts |
| Public fixture set | [`fixtures/F01…F16 *.bundle.json`](fixtures/README.md) — 15 source bundles + F16 combined clean-room; F14 as compiled-instance variants file | Draft, schema-validated |
| Evaluator-only oracle set | [`fixtures/*.oracle.json`](fixtures/README.md) — property-expectation format per fixture | Draft |
| Hidden-fixture generation & custody spec | [`hidden_fixture_custody_spec_v0.1.md`](hidden_fixture_custody_spec_v0.1.md) — bounds, coverage matrix, 100% semantic threshold, seed commitment/escrow, unseal event, disjointness registry | Draft; custodian/witness TBD |
| Cost-counter specification | Draft within Doc 08 §21 + telemetry schema fields | Draft within contract/schema |
| Representation-neutral compiler interface | Compile_T spec §§1–3, 5 (control-symmetry note) | Draft |
| Control-development charter | [`control_development_charter_v0.1.md`](control_development_charter_v0.1.md) — formulations U/G/A/C/X, neutral I/O contract §3, competence tests CT-1…CT-6, budget parity, veto rights | Draft; U+G builder contract approval required before freeze (PA-pass fix) |
| Prior-art kill-screen matrix | [`../09_M0_Prior_Art_Kill_Screen_Matrix_v0.1.md`](../09_M0_Prior_Art_Kill_Screen_Matrix_v0.1.md) — 14 families, residual R1–R4, Generic recommendation | Draft; citations unverified |
| Review checklist | [`review_checklist_v0.1.md`](review_checklist_v0.1.md) — sections A–F mapped to reviewer roles, every line cites authority | Draft |
| Version/hash manifest | [`version_hash_manifest_v0.1.md`](version_hash_manifest_v0.1.md) — canonicalization scheme + template; mechanical generator refuses unfreezable packages | Scheme Draft |

## 2. Schemas (`schemas/`) — technical notes

All six files validate against JSON Schema Draft 2020-12 metaschema.

| File | Covers (Doc 08 §9 objects) |
|---|---|
| `common.schema.json` | shared $defs: identifiers, polarity, literals, conditions, substitution patterns, statuses (**aggregated query_status excludes BOTH** — branch-local only), ResourceConfig, CompilerManifest (`attribution_label` const-pinned to Generic; MT-hash map ^MT-[1-9]$) |
| `source_bundle.schema.json` | Signature, ContextKey (GLOBAL reserved via not-const), AnchorIntent, Entity (constants), Concept, NeutralEvent, NeutralRoleEdge, NeutralAnalysisGroup + NeutralAnalysis (with `assumed_fact_refs`), NeutralFact, NeutralRequest, task-theory T claim forms, Query |
| `compiled_instance.schema.json` | CompiledFact/Event/RoleEdge/AnalysisGroup/Analysis/Request, Scope forest, InheritanceEdge, Rule (strict\|default + stratum), Exception, Block, PriorityEdge, OptionalGroup, Constraint, Query, ResourceConfig, CompilerManifest |
| `model_payload.schema.json` | ModelPayload; structural prohibition of post-inference/evaluator field families (§15.1) via additionalProperties=false + allOf/not |
| `execution_audit.schema.json` | Tagged union COMPLETE / INVALID_INSTANCE / RESOURCE_EXHAUSTED (§19.4): failures structurally cannot carry answers; branch records; skeptical-v1 states |
| `telemetry_manifest.schema.json` | Representation / execution / environment / labour ledgers; §21.5 mandatory zeros as const 0 |

### Deliberate schema-vs-validator split
JSON Schema enforces **structure only**. Semantic rules live in the M1 validator (§10.1): variable occurrence/safety, type-correctness vs Σ, scope single-parent + acyclicity, inheritance/priority acyclicity, optional-group non-overlap, stratification dependency-graph rule, GLOBAL-only self-activation facts.

### Amendment log (schema pack)
| Version | Date | Change |
|---|---|---|
| 0.1 | 21 Aug 2026 | Initial six schemas; Pass-2 alignment added first-class Concept/NeutralEvent/RoleEdge (+compiled twins), separate Analysis objects, BOTH removed from aggregated enum, env memory required |
| 0.1.1 | 21 Aug 2026 | Fixture-driven: `assumed_fact_refs` on analyses for branch-local sense assumptions (F16 requirement, §16.2) |

If reviewers overturn the Generic relabel at M0 review, the schema's const pin must be amended and rehashed under §23.5 — by design.

## 3. Fixtures conventions (see also fixtures/README.md)

1. Branch-local assumptions via analysis `assumed_fact_refs`
2. Request-context predicates: reserved zero-arity predicates derived from request_context fields (e.g., `ctx_special_collections()`)
3. Class-node inheritance via explicit class constants carrying GLOBAL parent facts
4. Oracles are property expectations (not full audits)
5. F14 variants are **compiled instances** (the §10.1 validator layer); their manifests carry placeholder hashes until freeze

## 4. Reviewer notes

- Implementation reviewer: "implement without asking" test applies to schemas + Compile_T spec — every question you'd need to ask is a blocking finding.
- Methods reviewer: check model_payload prohibitions vs §15.1; execution_audit union vs §19.4; kill-screen citations (its §7 checklist).
- Sanskrit reviewer: mapping cards MC-1…MC-7 with `[verify]` loci; MC-6 proposes Relabel (blocking → purely Generic) — ratification forces a versioned TS/ledger amendment.
