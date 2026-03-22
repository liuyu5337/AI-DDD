---
name: security-check
description: Review changes for security risks
disable-model-invocation: true
context: fork
agent: security-reviewer
---
Perform a security review for:

$ARGUMENTS

Required output:
- findings by severity
- affected areas
- attack path
- remediation advice
- overall posture summary