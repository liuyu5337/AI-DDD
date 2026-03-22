---
name: run-test-check
description: Add, run, and analyze JUnit 5 / Vitest tests for a change
disable-model-invocation: true
context: fork
agent: tester
---
Test the following feature or changed area:

$ARGUMENTS

Required output:
- test scope
- added/updated tests
- execution result
- failure analysis
- coverage gaps