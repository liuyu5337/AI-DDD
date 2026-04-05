---
name: security-check
description: Review selected changes from a security perspective
disable-model-invocation: true
context: fork
agent: security-reviewer
---

# Skill Usage

## Perform a security review for / 对以下内容进行安全审查

$ARGUMENTS

## Required output
- findings
- risk level
- attack path
- remediation advice
