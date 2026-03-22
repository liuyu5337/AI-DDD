---
name: engineering-core
description: Shared engineering constraints and delivery rules for this project
disable-model-invocation: true
user-invocable: false
---
# Engineering Core

## General Rules
- Understand the task before editing.
- Keep changes minimal and scoped.
- Prefer consistency with the existing codebase.
- Do not introduce unrelated refactors.
- Do not present pseudo code as complete implementation.

## Delivery Rules
- Identify affected files/modules before editing.
- Preserve backward compatibility unless explicitly allowed otherwise.
- Update tests for meaningful behavior changes.
- Update docs when API, behavior, SQL, setup, or usage changes.

## Finish Report
When finishing work, summarize:
- changed files
- key decisions
- tests status
- known risks or limitations