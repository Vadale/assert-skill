# Select roles only for work they actually perform

Use the existing team/conventions. A separate role is justified by expertise,
work volume or genuine independent review, not a fixed roster. S normally uses
the main session with honest self-review. One implementation WP at a time;
planning/doc/review may be parallel only with separate bounds and no conflicting
writes. Separate worktrees are not an excuse to copy uncommitted state implicitly.

| Role | Bounded mission and access |
|---|---|
| architect / Astra planning | Plan/current WP, architecture choices and ADRs; no product code. |
| coder / owner | Implement one authorized WP; demonstrate actual acceptance. |
| tester | Independent expected values/edge/error cases; owns assigned tests and records failures. |
| reviewer | Read-only technical findings with severity, location, evidence, consequence and bounded next check. |
| security-auditor | Read-only review of actual sensitive surfaces/dependencies/permissions; do not certify universal security. |
| doc-writer | Useful instructions in artifact language, synchronized with actual behavior; do not invent executed examples. |
| session-writer | Proportionate local diary/checkpoint, often performed by the owner/doc-writer. |
| simplifier | Reader-oriented cleanup under Core/T/P/D controls; not automatic code deletion. |
| release-reviewer | Read-only audience/permission/content review using publication-fit-review or sharing fallback. |

Mandate anatomy: identity/designated reader, invariants, bounded mission, process
and output, never-do. Give only relevant inputs, allowed paths/tools and expected
output. Read-only roles report; the owner performs authorized fixes. Distinguish
procedural separation from permission enforcement. Independent review needs a
separate session; sequentially wearing two hats is self-review, not independence.

Prefer Astra Ultra for planning and difficult decisions when actually available
and authorized. Strong judgment for architecture, scientific/security/contract
review and delicate simplification. Mechanical inventory/reformatting can use an
appropriate cheaper model if available. Do not invent model IDs, availability,
provider access, measured savings or consultation. Parent integrates the result;
only indispensable unresolved user choices stop otherwise authorized work.

Expose the selected mapping in the setup proposal, rather than silently choosing
a team: role, bounded mission, strong/economy tier, actual supported model/session
and review independence. Unknown availability remains unknown. A small project
can explicitly assign all relevant functions to the main session with self-review;
M/L receives only roles that have real work. If native model switching is absent,
record a procedural preference, not a completed switch or a new provider setup.

Reuse r-statistical-analysis for suitable statistical execution, project-continuity
for consequential close/resume, publication-fit-review for planned/existing sharing
and its release-reviewer role. Use other installed software/skills only for actual
tasks. Missing companions are not installation authority or a reason to load every
other skill; use self-contained checks and disclose consequential capability gaps.

Minimal procedures when materializing them:
- `new-wp`: verify current checkpoint, authority/decisions, allowed files, acceptance
  and relevant baseline; assign one owner, execute and preserve evidence.
- `session-close`: save current objective/identity, decisions, actual checks and
  limitations, useful diary lesson and next authorized step. No upload by default.
- Sharing: materialize the relevant steps in [sharing](sharing.md) if the companion
  skill cannot be used; short links to unavailable resources are not a fallback.
