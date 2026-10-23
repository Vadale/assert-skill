# Simplifier checks

Materialize this resource in a code project's docs/simplifier-checks.md.
Translate prose to the chosen artifact language as needed; keep Core/T/P/D section
keys stable. During work read Core for simplification plus triggered sections only.

## Core

Optimize for the designated reader's understanding and maintenance, not deleted
lines or cleverness. Six missions: structure, measured performance, dependencies,
reasoned deduplication, resources, and readable code/comments/tests. Check real
callers/contracts before removing scaffolding or indirection. Two uses do not
force extraction, one does not force inline; preserve useful names/contracts and
constraint comments. Restore local duplication if flags/exceptions couple distinct
concepts. Correct documentation falsified by changes. Address bounded leaks,
unbounded growth and cleanup on error paths with relevant regressions; refer actual
vulnerabilities to security review, not a global audit by default.

Start from a relevant passing baseline. A red baseline pauses simplification for
diagnosis; authorized diagnosis/fix can continue. Preserve goldens, protected APIs,
areas and active guards; never weaken, skip or remove valid tests for green or
add a dependency just to simplify. Changes to public APIs, layouts, precision or
behavior need the appropriate decision. Cross-module signatures/dependency removal
need explicit scope. Rank benefit/risk, use small verified edits and finish local
formatter/linter; relevant subsets in iteration, required full checks at delivery
boundaries. Report commands/results, measured gains, limits and rejected ideas.

Trigger a bounded pass for concrete test disconnects, semantic duplication, forced
abstractions or unreadability in any size; L phase boundaries and roughly 500-line
M/L WPs also trigger review. Do not turn this into an automatic whole-project audit.
Read T for tests/removal/changed exercised paths, P for performance, D for delicate
rewrites. Triggers accumulate as the diff changes. Recover any missing triggered
section before the action; no control is dropped to save context.

## T — Tests, removals and exercised paths

Distinguish product/test callers and protect the real route before removing the
old one. Test-only is not dead: check public APIs, callbacks, dynamic registrations,
compatibility and intentional references. Inspect semantic redundancy, opaque
helpers and excessive mocking/fixtures; parameterize only for clearer cases and
failure attribution. Independent expected values must not reuse product logic.
Verify the fact/requirement represented by a reference even when the comparison
is green. If it is wrong, retain the original outcome and independently justify
the correction. If the guard is valid, fix the product. Never change expected
values just for green.

Unit and integration tests may protect different risks despite identical coverage.
Map each removed/merged case → behavior/boundary/regression → surviving check;
retiring a requirement needs an approved decision. Preserve uncertain protection.
Green and coverage do not prove equivalence. Tester checks protection, reviewer
checks delicate removal; disclose non-independent roles. For delicate edits use
a targeted negative probe, observe expected failure, restore and rerun. No broad
automatic mutation campaign or deletion to shorten a suite.

## P — Performance and optimization claims

Define metric/threshold, representative workload/environment and baseline; find
the bottleneck. Compare the complete relevant route before/after, with variability
and worst cases when pertinent. Do not extrapolate to an untested final environment.
Gains need numbers. Prefer clarity to marginal complex optimization; isolate and
justify complexity. Precision or behavior changes require agreed tolerances and
verification, not altered goldens. No automatic benchmark infrastructure or new
dependencies. Static text size, cache use and delegation are not measured total
token/time savings; include delegate costs when exposed or mark unavailable.

## D — Delicate rewrites and differential comparison

Identify a bounded reproducible reference by revision/hash plus command/fixture;
copy only if necessary. Match input/config/conditions, environment and relevant
seeds; agree equality/tolerances first. Intermediate states diagnose rather than
replace final behavior. Old code can be wrong: also use independent specifications
and boundary cases. Record reference purpose and retirement condition; preserve
intentional references even if called only by tests. If no useful reference exists,
state the limit and use independent requirements/cases instead of an equivalence
claim. Separate baseline, transformation, final integration and measurement when
combined work would otherwise obscure attribution; no extra phases for trivial edits.
