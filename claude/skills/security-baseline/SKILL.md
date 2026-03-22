---
name: security-baseline
description: Security baseline for backend/frontend/application changes
disable-model-invocation: true
user-invocable: false
---
# Security Baseline

Always review for:
- authentication
- authorization
- input validation
- SQL injection / expression injection / command injection
- output encoding
- sensitive data exposure
- file upload/download safety
- secrets in config/code/logs
- auditability of critical actions

Rules:
- Never hardcode secrets.
- Never log passwords, tokens, or sensitive personal data.
- Validate untrusted input.
- Verify permission checks on sensitive operations.
- State security assumptions explicitly.