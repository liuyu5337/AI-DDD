# API Rules

## Core principles
- OpenAPI First: design or update the contract before implementation
- Stable DTOs: do not expose DO / Entity / MyBatis-Plus types directly
- Backward compatibility by default unless task explicitly allows breaking changes
- Separate request DTO, response DTO, page DTO, and query DTO

## Endpoint design
- URL uses resource-oriented naming
- Query/list/search/export actions must define filter, sort, pageNo, pageSize behavior
- Write APIs must define idempotency requirements where relevant
- Sensitive APIs must define auth and permission assumptions explicitly

## Request / Response
- request fields must have clear meaning and validation rules
- response fields must not be ambiguous
- pagination should use project DTOs rather than framework page objects
- recommended unified response: `code`, `message`, `data`, `requestId`

## Error model
- shared and module-specific error codes must be separated
- validation, business, permission, and unknown errors should be handled distinctly
- never expose stack trace, SQL, or framework internals to clients

## Delivery output
For each changed API, mention:
- purpose
- request model
- response model
- validation
- error model
- compatibility notes
- frontend integration notes
