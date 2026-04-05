# Testing Rules

## General
- meaningful behavior changes require tests or explicit explanation why not
- tests should be focused and maintainable
- cover happy path, validation failure, and important edge cases

## Backend
- JUnit 5
- prioritize application service and domain rule coverage
- add controller / integration tests when contract behavior matters

## Frontend
- Vitest + Vue Test Utils
- cover render states, interactions, validation, and critical component behavior

## Delivery output
- what was tested
- what passed or failed
- what remains untested
