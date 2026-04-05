---
name: review-changes
description: Review changed code and identify risks before merge
disable-model-invocation: true
context: fork
agent: reviewer
---

# Skill Usage

## Review the following changes / 审查以下变更

$ARGUMENTS

## Required output
- summary
- major findings
- minor findings
- missing tests
- verdict
