---
name: review-changes
description: Review recent code changes for architecture, quality, and maintainability
disable-model-invocation: true
context: fork
agent: reviewer
---
Review the following changes or scope / review 以下改动范围:

$ARGUMENTS

Required output:
- summary
- major findings
- minor findings
- missing tests
- suggested improvements
- verdict
