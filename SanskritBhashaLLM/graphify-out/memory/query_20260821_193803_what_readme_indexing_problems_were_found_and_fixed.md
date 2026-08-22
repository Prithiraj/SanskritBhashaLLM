---
type: "query"
date: "2026-08-21T19:38:03.719560+00:00"
question: "What README/indexing problems were found and fixed?"
contributor: "graphify"
outcome: "useful"
source_nodes: ["M0 JSON Schema Pack v0.1 (6 schemas)"]
---

# Q: What README/indexing problems were found and fixed?

## Answer

Found: (1) no top-level README - corpus of 11 numbered docs + pilot + 3 directories had no index; (2) m0-artifacts/README only indexed schemas, not fixtures/mapping-cards/custody-spec/kill-screen/TS/Compile_T; (3) SHA256SUMS.txt stale - absolute paths to predecessor filenames from 19 Aug, sha256sum -c failed on all entries. Fixed: created top-level README.md with reading-order doc table (exact filenames), M0 artifact section, reviewer-playbooks pointer, status snapshot (DQ0 provisional/DQ1 unanswered), integrity-manifest note; rewrote m0-artifacts/README.md as master inventory cross-referencing every Doc 08 section17 row to file+status; archived old manifest to SHA256SUMS_2026-08-19_archive.txt and regenerated SHA256SUMS.txt with relative paths over current corpus (verifies clean); automated link check ALL RESOLVE and doc index coverage COMPLETE 11/11.

## Outcome

- Signal: useful

## Source Nodes

- M0 JSON Schema Pack v0.1 (6 schemas)