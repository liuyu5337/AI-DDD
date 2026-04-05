---
name: ci-pipeline-guardrails
description: CI pipeline minimum quality gates and pre-release guardrails
disable-model-invocation: true
user-invocable: false
---

# CI Pipeline Guardrails / CI 流水线门禁

## Minimum gates
- build passes
- relevant tests pass
- static checks pass if configured
- package artifact is reproducible
- version / changelog updated when needed

## Release-minded rule
- do not bypass failing gates without explicit reason
