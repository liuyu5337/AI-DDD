---
name: ci-pipeline-guardrails
description: Generate CI/CD guardrails, pre-merge checks, and pre-release checklists for backend, frontend, API, SQL, testing, and documentation quality in this project
context: fork
agent: tester
disable-model-invocation: true
---
Prepare CI pipeline guardrails and quality-gate guidance for the following change, module, or project:

$ARGUMENTS

Project expectations:
- Spring Boot 3.x + Java 17 backend
- MyBatis-Plus infrastructure
- Vue 3 + Element Plus frontend
- OpenAPI First
- SQL-script-based DB changes
- JUnit 5 + Vitest + Vue Test Utils
- Security-sensitive changes should be reviewable

You must generate, when appropriate:
1. Backend build and test gate suggestions
2. Frontend build and test gate suggestions
3. API contract and DTO consistency checks
4. SQL script checks
5. Documentation checks
6. Security review checks
7. Pre-merge checklist
8. Pre-release checklist
9. Known-risk reminder items

Hard constraints:
- Do not mark checks as passed without evidence.
- Keep gates practical and executable.
- Distinguish mandatory gates from recommended checks.
- Make SQL, API, test, and documentation completeness explicit.
- Mention gaps honestly when evidence is missing.

Required output format:
- mandatory gates
- recommended checks
- pre-merge checklist
- pre-release checklist
- missing evidence or risks