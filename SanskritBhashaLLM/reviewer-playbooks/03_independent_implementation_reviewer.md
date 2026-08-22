# Playbook — Independent Implementation Reviewer (DQ1-M0 / M1)

**Version:** 0.1 · **Date:** 21 August 2026
**Your mandate:** could a competent engineer implement this without calling the author? Then, at M1: is the code what the spec says, deterministic, and free of hard-coding?
**You are NOT reviewing:** research validity or Sanskrit content.

---

## 1. Required reading

1. Doc 08 §§9–10 (schema + operational semantics), §16 (fixtures), §19–22 (M1 contract + tests), §23 (seal/custody)
2. Compile_T Specification v0.1 (stages S0–S8, obligations O1–O7, error handling)
3. TreatmentSignature v0.1 §4 (derivability — no discretionary step)

## 2. Now (M0 stage) — implementability review

- [ ] Each S0–S8 stage has checkable inputs/outputs; no stage reads a later stage
- [ ] Every error path fails closed (`INVALID_SOURCE`); no discretionary fallback anywhere
- [ ] MT tables are algorithmically complete: for each lawful T-statement form, a mapping exists or a defined rejection occurs
- [ ] You could write the source/target JSON Schemas from Doc 08 §9 + these specs **without asking the owner any semantic question** — that is the §18.1 test. List every question you *would* have to ask; each one is a blocking finding.

## 3. Later (M1 stage) — acceptance review

### D1 — Determinism and projections
- [ ] Byte-identical semantic + deterministic-audit projections across replays
- [ ] Telemetry separate, complete, own hash; measured values need not repeat (§19.4)
- [ ] Canonical ordering before hashing; hash field omitted from its own preimage

### D2 — Test adequacy
- [ ] All 16 public fixtures pass; invalid fixtures fail closed
- [ ] Hidden acceptance set: 100% semantic conformance vs independent oracle; any mismatch = Fail (§20.1, §22.1)
- [ ] Exhaustive small-instance oracle comparison passes
- [ ] Metamorphic suite green (permutation, renaming, irrelevance additions)
- [ ] Mutation score: disabling any claimed operator kills ≥1 test (§20.3)

### D3 — No hard-coding (§20.4)
- [ ] No fixture-ID branching, embedded gold conclusions, hash lookups of hidden fixtures, nonce special-cases
- [ ] Static inspection + renamed hidden variants both clean

### D4 — Custody discipline
- [ ] Implementer (and you, if you reviewed code) had no access to sealed fixtures before unseal event
- [ ] Access log complete; first unseal immutable; reruns use fresh sealed sets (§23.4)

## 4. Your unique power

You are the only reviewer who can empirically confirm "an independent engineer can implement M1 without asking the mechanism author to decide semantics" (Doc 08 §18.1). Treat every ambiguity you hit as a finding, not a question to resolve informally.

## 5. Record

Shared template in `00_REVIEW_OPERATIONS.md` §3. At M1 you additionally file the reproducibility report: environment manifest, build-from-frozen-artifacts result, replay hashes.
