# DQ1-M0 Operational Semantics — Normative Reference

**Document type:** DQ1-M0 required artifact (Doc 08 §§9–10, §17 row "operational semantics")
**Version:** 0.1 — Draft for four-role review
**Date:** 22 August 2026
**Status:** Refines Doc 08 §§9–10 without contradicting them; on conflict, Doc 08 controls (§1 of that contract).

---

# OS-0. Conventions and State Model

- **OS-0.1** Inputs: a compiled instance valid against `schemas/compiled_instance.schema.json`, plus exactly one request `req` selected from `requests[]`. A run evaluates one (instance, request) pair.
- **OS-0.2** Branch-local state: `F_act` (visible facts), `F_der` (derived per stratum), `SUP` (support records: source / inherited / strict / default), `APP` (grounded applications with status), `PATHS` (supporting/blocked inheritance paths), `TRC` (trace events), counters (OS-R).
- **OS-0.3** Support polarity model is four-valued per ground literal: support⁺, support⁻, both, neither (Doc 08 §9.3). Absence ≠ falsity.
- **OS-0.4** All set iterations in this document are executed over canonically sorted sequences (OS-T.2); no semantic result may depend on iteration order.

## Decisions pinned here (previously implicit in Doc 08)

| ID | Decision |
|---|---|
| D-1 | Request-context predicates: for each reserved zero-arity predicate named by an activation condition, it holds iff the corresponding key exists in `request_context` with value `true` (convention fixed by fixtures README; e.g. `ctx_special_collections`). Materialized before scope evaluation as evaluator-computed facts; never stored in instances. |
| D-2 | Analysis `assumed_fact_refs`: injected at stratum 0 into `F_act` as **branch-local source support** (indefeasible). They participate in all rules like ordinary facts but exist only in branches selecting that analysis. |
| D-3 | Counting rules (normative, F15-critical): see OS-R.2. |
| D-4 | Canonical ground sort order: control classes ascending `BLOCK < EXCEPTION < INDEFEASIBLE_OPPOSITION < PRIORITY`; within class, by `(rule_id, canonical substitution string)`. |
| D-5 | Substitution enumeration order: variables lexicographic; constants in signature declaration order. Enumeration order never affects results (metamorphic M-O guards this). |
| D-6 | Priority alignment: `shared_argument_alignment` lists variable names; two grounded applications are *matched* iff every aligned variable binds to the identical constant in both substitutions (after pattern application). |
| D-7 | Exact-complement heads: same predicate, same argument terms, opposite polarity. Only such pairs can be defeated via priority. |
| D-8 | Strict closure recursion: positive same-stratum recursion permitted only among strict heads whose dependency region contains no default-derived predicate (§10.1 stratification rule); validator rejects violations statically. |
| D-9 | Optional selections: an inapplicable selected member remains selected, emits no applications, and is recorded with `applicable=false` (§9.4). |
| D-10 | Constraints: evaluated at their declared `evaluation_stratum` against current branch state; a satisfied constraint rejects the whole branch (`REJECTED_CONSTRAINT`, naming the constraint id). |
| D-11 | Anchors: exactly one anchor per request; different anchor ⇒ different Request object. Anchor usable iff complete root-to-anchor path active (§10.3). |
| D-12 | Visibility: `context_key=GLOBAL` facts always visible; scoped fact visible iff its scope lies on the active root-to-anchor path. Off-path scopes never exchange facts. |
| D-13 | Body satisfaction under conflict: a body literal is satisfied iff its exact-polarity ground literal has support; BOTH-support satisfies both polarities (§9.3). |
| D-14 | A strict rule consuming a committed default's head fires in a later stratum only; lower-stratum commitments are never retracted (§10.5). |

---

# OS-V. Validation (fail-closed; pre-branch)

V-1 Structural conformance to schema; duplicate ids; unknown refs ⇒ `INVALID_SOURCE`.
V-2 Scope forest: single parent per non-root scope; acyclic; anchor ∈ forest.
V-3 Inheritance graph acyclic.
V-4 Unconditional priority supergraph acyclic; conditional edges checked after instantiation-time reachability (static check on declared conditions' predicates).
V-5 Optional groups non-overlapping; `minimum_choices ≤ maximum_choices ≤ |members|`.
V-6 Stratification: build signed predicate-dependency graph over rule heads/bodies and control conditions; any cycle containing a defeasible or control dependency ⇒ reject (D-8 restated). Assign each rule/control its stratum from the graph; instance-declared strata must equal computed strata.
V-7 Variable safety (§9.2): every variable type-correct, occurs in a positive relational body literal or finite typed-domain binder; head variables occur in positive body literals.
V-8 GLOBAL-only self-activation: a scope's activation condition may read only GLOBAL-sourced facts, request context, or analysis bindings (§9.2).
V-9 Evaluator-only fields absent from execution input (§14.2).
V-10 Any violation ⇒ `execution_status=INVALID_INSTANCE`, `evaluation_state=NOT_EVALUATED`, deterministic validation trace only.

# OS-B. Branch construction

B-1 Let G = set of analysis groups, O = optional groups. Enumerate the exact Cartesian product: one member per group × every legal selection per optional group satisfying min/max (§10.2). Enumeration order per D-5.
B-2 Inject assumed facts (D-2) for the branch's selected analyses.
B-3 Reject a combination only under an explicit compatibility condition from the bundle; record rejection reason `REJECTED_COMPATIBILITY`.
B-4 If product size would exceed `branch_limit` ⇒ `RESOURCE_EXHAUSTED{counter:branches}` before any inference; no sampling or pruning (§10.2).

# OS-S. Scope activation (per branch)

S-1 Materialize request-context predicates (D-1).
S-2 Walk root→anchor path (unique, D-11). Scope active iff parent active (or root) AND activation condition true under: request context, branch analysis bindings, GLOBAL facts, and this branch's assumed facts? **No** — activation reads only GLOBAL + request context + bindings (V-8); assumed facts are NOT visible to activation of their own scope's ancestors... precisely: assumed facts carry their analysis's scope_id; they are visible in S-3 fact visibility but may not activate any scope (anti-circularity, §10.3).
S-3 Fact visibility: GLOBAL ∪ {scoped facts whose scope is on the active path} ∪ branch-assumed facts (for rule bodies only, not activation).
S-4 Path inactive at any hop ⇒ reject branch `REJECTED_INACTIVE_ANCHOR` naming the failing scope.

# OS-I. Inheritance and blocking

I-1 For each property p and target t: enumerate every permitted path (edge sequence respecting `permitted_properties`) through ACTIVE scopes only; count toward `inheritance_paths` counter.
I-2 Blocks: evaluate all blocks (from frozen lower-stratum snapshot) whose `property_or_relation=p`; a block removes exactly the matching edge/path instances it declares.
I-3 p reaches t iff ≥1 unblocked path remains; record supporting and blocked paths separately.
I-4 Committed inherited support is **indefeasible** at its declared stratum: defaults/priorities cannot defeat it later (§10.4). Blocked paths are counterfactual records only (never consumed by rules).
I-5 Opposite-polarity conclusions about the same (property, target) from unblocked paths ⇒ explicit conflict record (indefeasible opposition).

# OS-E. Stratified evaluation (per retained branch, ascending stratum s = 0…k)

E-0 Stratum 0: inject source facts (GLOBAL + visible scoped) and assumed facts (D-2) as indefeasible source support.
Repeat for each stratum:
E-1 Evaluate inheritance permissions and blocks whose conditions use the settled lower-stratum snapshot; materialize per I-1…I-4.
E-2 Compute least fixed point of applicable **strict** rules (positive same-stratum recursion per D-8); each firing attempt counts `logical_steps`; committed conclusions are indefeasible strict support.
E-3 Instantiate **defaults**: for each default rule, enumerate total satisfying substitutions (D-5); create grounded applications `{rule, substitution}`; count `grounded_applications`.
E-4 Evaluate every grounded exception from the frozen snapshot; mark each exactly-matched application (same rule_id AND identical substitution per pattern D-6 semantics restricted to exception patterns) `defeated_by_exception`.
E-5 Suppress applications opposed by source/inherited/strict support of opposite polarity on the head literal: `suppressed_by_indefeasible_opposition`.
E-6 Instantiate priority edges among remaining applications: matched per D-6/D-7; compute transitive closure as ordering relation. For pairs with exact-complement heads: defeat lower (`defeated_by_priority`). Same-polarity ordered pairs: recorded as ordering-only grounds, never defeating (§10.5 step 8).
E-7 Undefeated opposite-polarity defaults, equal or incomparable under closure ⇒ both remain; mark head literal conflicted (both-support).
E-8 Commit every other undefeated default head as defeasible support.
E-9 Evaluate hard constraints at their declared stratum (D-10); rejecting ⇒ drop branch with reason.
E-10 Record all grounds canonically sorted (D-4); emit trace events per transition.
E-11 Next stratum. Lower-stratum commitments immutable (D-14).

After final stratum: compute branch query states (OS-C), then aggregate across branches (OS-A).

# OS-C. Conflict semantics (per branch, per query q)

C-1 q state TRUE ⇔ support⁺(q) ∧ ¬support⁻(q); FALSE symmetric; NEITHER ⇔ no support either polarity; BOTH ⇔ both polarities supported (any mixture of source/inherited/strict/committed-default support).
C-2 Conflicts are reported per ground literal in `conflicts[]` with supporting polarities; unrelated conflicts do not alter other queries (§10.6).
C-3 Defaults never defeat indefeasible support (by E-5); indefeasible-vs-indefeasible opposition persists as BOTH.

# OS-R. Resource accounting (deterministic; semantic)

R-1 Wall/CPU/memory are telemetry only; they NEVER alter status (§10.7).
R-2 Counter definitions (each increment site normative):
- `logical_steps`: one per rule-body satisfaction attempt (strict or default), one per scope-condition evaluation, one per constraint evaluation, one per aggregation operation.
- `grounded_applications`: one per created grounded application (E-3).
- `inheritance_paths`: one per enumerated candidate path (I-1), blocked or not.
- `branches`: one per constructed combination (B-1), retained or rejected.
- `trace_events`: one per emitted trace event.
R-3 Limits from `resource_configs[req.resource_config_id]`. Breach ⇒ `RESOURCE_EXHAUSTED` carrying counter name + limit; deterministic trace prefix marked PARTIAL; no partial answers (§10.7).
R-4 Exhaustion checks occur at increment sites; checking itself is not counted.

# OS-A. Aggregation `skeptical-v1` (exclusive order)

A-1 No retained branch ⇒ `NO_VALID_ANALYSIS`.
A-2 Any branch BOTH(q) ⇒ `CONFLICT`.
A-3 All TRUE ⇒ `ENTAILED`. A-4 All FALSE ⇒ `CONTRADICTED`.
A-5 All NEITHER ⇒ `UNKNOWN`. A-6 Otherwise ⇒ `AMBIGUOUS`.
A-7 `analysis_status`: NONE / SINGLE / MULTIPLE from retained-branch count. Identical states across multiple analyses do not alone imply AMBIGUOUS (§10.8 note).

# OS-T. Trace, ordering, output separation

T-1 Every derived/blocked/defeated/rejected item carries a machine-readable reason (§11.10).
T-2 Canonical ordering: facts/rules/scopes by id; applications by (rule_id, canonical substitution string); grounds by D-4; trace events by emission step.
T-3 Identical input+configuration ⇒ byte-identical semantic projection and deterministic-audit projection incl. hashes (§19.4); telemetry separate and exempt.
T-4 Outputs: `ModelPayload` (pre-inference only) | `ExecutionAudit` (this semantics) | `TelemetryManifest`. No audit field enters payload (§15).
T-5 Failure variants carry no completed or partial query answers (§19.4).

---

# Worked micro-trace — fixture F06 (precedence chain)

Stratum 0: source facts special(t), odd(t), bird(t) → source support.
E-3: defaults instantiate: d_spec{X=t}, d_odd{X=t}, d_gen{X=t} (+3 apps, +3 steps).
E-4/E-5: no exceptions; no indefeasible opposition.
E-6: edges p1(d_spec>d_odd), p2(d_odd>d_gen) match (alignment X≡X, complement heads d_spec/d_odd, d_odd/d_gen). Closure adds (d_spec>d_gen) — same polarity ⇒ ordering-only. Defeats: d_odd (by spec), d_gen (by odd).
E-8: commit flies(t) from d_spec.
Query flies(t): support⁺ only ⇒ TRUE; single branch ⇒ ENTAILED. ✔ matches oracle A1–A3.

# Reviewer pointers

- Implementation reviewer: implement from OS-V…OS-T without consulting Doc 08 prose except for clause cross-checks; every question = blocking finding.
- Methods reviewer: verify D-1…D-14 table against §§9–10 for contradiction; confirm R-2 counters make F15 oracle determinate.
