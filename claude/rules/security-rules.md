# Security Rules / 安全规则

Always review:
- authentication
- authorization
- input validation
- SQL / command / expression injection risk
- XSS / CSRF / SSRF risk where relevant
- file upload/download safety
- sensitive data exposure
- secret handling
- auditability for critical actions

## Non-negotiables
- Never hardcode secrets.
- Never log passwords, tokens, keys, or sensitive personal data.
- Validate untrusted input.
- Sensitive operations must have explicit permission checks.
- State security assumptions when they affect design or review conclusions.
