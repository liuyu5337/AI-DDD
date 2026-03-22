---
name: openapi-dto-error-template
description: Generate OpenAPI-first contract drafts, request/response DTO templates, pagination templates, and error-code templates for backend/frontend aligned development
context: fork
agent: api-architect
disable-model-invocation: true
---
Generate an OpenAPI-first contract and DTO/error templates for the following requirement:

$ARGUMENTS

Project constraints:
- OpenAPI First
- Unified response envelope
- Stable semantic error codes
- Frontend-backend separated architecture
- Spring Boot 3.x backend
- Vue 3 frontend

You must generate or propose, when appropriate:
1. Module or endpoint responsibility summary
2. Endpoint list and HTTP methods
3. Request DTO draft
4. Response DTO draft
5. Unified page response DTO draft where relevant
6. Unified response envelope example
7. Shared error-code suggestions
8. Module-specific error-code suggestions
9. Validation rules and required fields
10. Compatibility notes and assumptions
11. Frontend integration notes

Hard constraints:
- Do not expose persistence DO or MyBatis-Plus types directly.
- Do not leave field meaning ambiguous.
- Do not invent hidden backend behavior without stating assumptions.
- Keep field naming stable and semantically clear.
- Separate shared error codes from module-specific error codes.
- For paginated APIs, use project-defined page response structures, not framework-native page objects.

Required output format:
- summary
- endpoint draft
- request DTO template
- response DTO template
- page response template if needed
- unified response example
- error-code template
- validation and compatibility notes