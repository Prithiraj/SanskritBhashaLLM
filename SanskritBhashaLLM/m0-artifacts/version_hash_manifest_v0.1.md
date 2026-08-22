# DQ1-M0 Version/Hash Manifest — Scheme and Template

## M0 Required Artifact (Doc 08 §17; §23.3 freeze package)

**Version:** 0.1 · **Date:** 22 August 2026
**Status:** Scheme Draft — actual manifest generated mechanically at Freeze via `make_manifest.py` (to be written before quorum convenes).

---

# 1. Canonicalization scheme (normative)

1. Every artifact is serialized as UTF-8 bytes (JSON: `json.dumps(sort_keys=True, separators=(',',':'), ensure_ascii=False)`).
2. `artifact_hash = SHA256(bytes)`.
3. Hash fields inside self-describing artifacts omit themselves from their own preimage (Doc 08 §19.4 convention).
4. Filenames are part of identity only via the manifest's `path` field, never hashed into content hashes.

# 2. Manifest structure

~~~json
{
  "manifest_id": "m0-freeze-package",
  "contract_version": "Doc-08 v0.2 <normative sha256>",
  "created_utc": "<iso8601>",
  "quorum": {
    "roles": {
      "mechanism_owner": {"name": null, "hash_approved": null, "date": null},
      "sanskrit_paninian_reviewer": {"name": null, "hash_approved": null, "date": null},
      "independent_methods_reviewer": {"name": null, "hash_approved": null, "date": null},
      "independent_implementation_reviewer": {"name": null, "hash_approved": null, "date": null}
    },
    "control_builders_U_G": [{"family": "U", "name": null}, {"family": "G", "name": null}],
    "rule": "all governance roles approve the SAME package_hash (§23.2)"
  },
  "artifacts": [
    {"role": "normative_contract",      "path": "../08_DQ1_Mechanism_Resolution_M0_M1_Contract.md", "sha256": null},
    {"role": "treatment_signature",     "path": "../10_M0_TreatmentSignature_v0.1.md",              "sha256": null},
    {"role": "compile_t_spec",          "path": "../11_M0_Compile_T_Specification_v0.1.md",         "sha256": null},
    {"role": "kill_screen",             "path": "../09_M0_Prior_Art_Kill_Screen_Matrix_v0.1.md",    "sha256": null},
    {"role": "schema_common",           "path": "schemas/common.schema.json",                        "sha256": null},
    {"role": "schema_source",           "path": "schemas/source_bundle.schema.json",                 "sha256": null},
    {"role": "schema_compiled",         "path": "schemas/compiled_instance.schema.json",             "sha256": null},
    {"role": "schema_payload",          "path": "schemas/model_payload.schema.json",                 "sha256": null},
    {"role": "schema_audit",            "path": "schemas/execution_audit.schema.json",               "sha256": null},
    {"role": "schema_telemetry",        "path": "schemas/telemetry_manifest.schema.json",            "sha256": null},
    {"role": "fixtures_public",         "path": "fixtures/",                                         "sha256": "<per-file map>"},
    {"role": "oracles_public",          "path": "fixtures/*.oracle.json",                            "sha256": "<per-file map>"},
    {"role": "mapping_cards",           "path": "mapping_cards_v0.1.md",                             "sha256": null, "decisions": {"MC-1..7": "pending"}},
    {"role": "custody_spec",            "path": "hidden_fixture_custody_spec_v0.1.md",               "sha256": null},
    {"role": "control_charter",         "path": "control_development_charter_v0.1.md",               "sha256": null},
    {"role": "review_checklist",        "path": "review_checklist_v0.1.md",                          "sha256": null},
    {"role": "operational_semantics",   "path": "TBD_separate_artifact",                             "sha256": null},
    {"role": "microfixture_sanskrit",   "path": "TBD_pending_domain_reviewer",                       "sha256": null},
    {"role": "compile_t_mapping_configuration", "path": "../11_M0_Compile_T_Specification_v0.1.md", "sha256": null, "note": "MT-1..MT-9 tables + frozen configuration bind at freeze"},
    {"role": "decode_t_witness_set",            "path": "TBD_public_roundtrip_witnesses",           "sha256": null},
    {"role": "cost_counter_specification",      "path": "../08_DQ1_Mechanism_Resolution_M0_M1_Contract.md", "sha256": null, "note": "section 21 counters bind via telemetry schema"},
    {"role": "claim_traceability_ledger",       "path": "../10_M0_TreatmentSignature_v0.1.md",      "sha256": null, "note": "section 3 C1-C8 rows"},
    {"role": "compiler_interface_contract",     "path": "../11_M0_Compile_T_Specification_v0.1.md", "sha256": null, "note": "sections 1-3 + 5"},
    {"role": "review_records",                  "path": "TBD_completed_checklists_per_reviewer",    "sha256": null}
  ],
  "disclosure_register": {"path": "TBD_owner_labour_register", "sha256": null},
  "package_hash": "<sha256 over canonical manifest minus this field>"
}
~~~

# 3. Rules

- A role approving hash H covers exactly the artifact set in that manifest; any later byte change ⇒ new package_hash ⇒ re-quorum (§23.5).
- Placeholder roles (`null`/TBD) make the package **unfreezable by construction**: the mechanical generator refuses to emit `package_hash` while any required role is unresolved.
- The sealed hidden-set manifest (custody spec §6) is a *separate* cryptographic object, generated after freeze; its commitment is appended to a v+1 package record without reopening frozen artifacts.
