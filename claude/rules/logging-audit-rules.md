# Logging and Audit Rules

## Logging
- logs should have diagnostic value
- include requestId / traceId when possible
- include business identifiers when useful
- avoid noisy logs without actionability
- never log secrets or sensitive data

## Audit
Sensitive operations should be auditable:
- create / update / delete
- approve / reject
- import / export
- permission changes
- login or security-sensitive actions

## Recommended audit fields
- operator
- operation time
- module
- target object
- action type
- result
- failure reason
- requestId / traceId
