---
name: engineering-core
description: Shared execution checklist aligned with repository-wide engineering rules
disable-model-invocation: true
user-invocable: false
---

# Engineering Core / 工程执行清单

Source of truth / 规则来源:
- `.claude/rules/engineering-rules.md`
- `.claude/rules/docs-rules.md`
- `.claude/rules/testing-rules.md`

Use this skill to operationalize the rules, not to redefine them.

## Checklist / 执行清单
1. Identify affected modules and files first.
2. Keep scope minimal and avoid unrelated refactors.
3. Check compatibility impact before editing.
4. Update tests for meaningful behavior changes.
5. Update docs when behavior, API, SQL, or setup changes.
6. End with a finish report: changed files, key decisions, tests status, known risks.
