---
name: run-test-check
description: Add, run, and analyze JUnit 5 / Vitest tests for a change
disable-model-invocation: true
context: fork
agent: tester
---

Test the following feature or changed area / 测试以下功能或改动范围:
$ARGUMENTS

Required output:
- test scope
- added or updated tests
- execution result
- failure analysis
- coverage gaps
