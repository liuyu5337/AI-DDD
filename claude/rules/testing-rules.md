# Testing Rules / 测试规则

## General
- Add or update tests for meaningful behavior changes.
- Prefer targeted, maintainable tests over large brittle tests.
- Cover success paths, validation failures, and important edge cases.

## Backend
- Use JUnit 5.
- Prioritize application-service behavior and domain rules.
- Add controller/integration tests when contract behavior is important.

## Frontend
- Use Vitest + Vue Test Utils.
- Cover rendering states, interaction paths, validation, and critical component behavior.

## Reporting
Completion reports must state:
- what was tested
- what passed or failed
- what remains untested
