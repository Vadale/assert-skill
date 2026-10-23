# Claude Code target

This adapter prepares a Claude Code project. Actual execution/delegation requires
the real host, available tools and current authority; another host can prepare
these files without claiming a native Claude run.

For a new project, use `CLAUDE.md` as the short authoritative entry and a thin
`AGENTS.md` pointer when portability is useful. Preserve an existing opposite
arrangement; never maintain two divergent rule sets. Record both selected languages.
Keep common plan/checkpoint/acceptance rules from lean setup.

When a team is justified, place selected roles in `.claude/agents/<role>.md`.
Read [roles](roles.md) for mandates. Native role frontmatter uses stable English
keys/name, a concise trigger description and the minimum actual tool set:

```yaml
---
name: reviewer
description: Review the assigned candidate and report evidenced findings without editing it.
tools: Read, Glob, Grep
---
```

Write the role's human-language description/body in the chosen artifact language;
the sample is structural, not an English override. Omit a fixed `model` unless
an available supported model choice is actually established. Personal preference
for Astra does not make it a Claude-native model identifier. Select an authorized
available equivalent or disclose the limitation; do not change providers/accounts.
Read-only roles do not receive Write/Edit/Bash merely for convenience. Other
path/access boundaries remain procedural unless the actual host enforces them.
Do not claim setting a model/tool name proves activation or isolation.

When useful, materialize `new-wp` and `session-close` under
`.claude/skills/<name>/SKILL.md` with name/description frontmatter and the actual
project procedure. Keep those procedures focused and linked to the current
PLAN/ROADMAP/HANDOFF; do not paste the full method into every role/skill.
S does not need a team. No speculative hooks, global settings, services or
permission changes. Native invocations differ from Codex; do not present `$name`
as a universal Claude command.

For publication-fit-review, connect an existing accessible skill to the selected
release-reviewer mandate; do not copy an invented absolute installation path.
If absent, materialize the minimal sharing procedure instead. Check generated
references within the project. Files or role definitions prepared for this target
are not evidence of a successful Claude session, independent review or tool run.
