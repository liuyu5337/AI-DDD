# Security Rules

## Always check
- authentication
- authorization
- input validation
- SQL / command / expression / template injection
- XSS / CSRF / SSRF where relevant
- file upload / download safety
- sensitive data exposure
- secret leakage in code, config, log
- auditability of critical actions

## Hard constraints
- never hardcode secrets
- never log passwords, tokens, or sensitive personal data
- verify permission checks on sensitive operations
- validate untrusted input
- state security assumptions explicitly

## Sensitive operations
For create/update/delete/import/export/approve/login/permission-change operations, prefer:
- permission checks
- audit trail
- requestId / traceId
- operator identity
- result and failure reason
