---
name: testing-junit5-vitest
description: Testing rules using JUnit 5 for backend and Vitest + Vue Test Utils for frontend
disable-model-invocation: true
user-invocable: false
---
# Testing Rules

## General
- Add or update tests for meaningful behavior changes.
- Prefer targeted, maintainable tests.
- Cover success paths, validation failures, and important edge cases.

## Backend
- Use JUnit 5.
- Prioritize application-service behavior and domain rules.
- Add controller/integration tests when contract behavior is important.

## Frontend
- Use Vitest + Vue Test Utils.
- Cover rendering states, interactions, validation, and critical component behavior.

## Delivery Rule
Completion reports must include:
- what was tested
- what passed or failed
- what remains untested