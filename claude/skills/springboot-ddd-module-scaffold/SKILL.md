---
name: springboot-ddd-module-scaffold
description: Scaffold a pragmatic DDD backend module for Spring Boot 3.x + Java 17 + MyBatis-Plus + OpenAPI First + SQL-script DB changes
context: fork
agent: backend-coder
disable-model-invocation: true
---
Scaffold a backend module for the following business requirement:

$ARGUMENTS

Project constraints:
- Java 17+
- Spring Boot 3.x
- MyBatis-Plus
- OpenAPI First
- Pragmatic DDD
- SQL-script-based DB changes
- JUnit 5

You must generate or propose, when appropriate:
1. Module responsibility summary
2. Suggested package structure
3. OpenAPI contract draft
4. Controller endpoints
5. Request DTOs and response DTOs
6. Application service interfaces / classes
7. Command and query models
8. Domain model / rule / domain service only where business complexity justifies it
9. Repository interface
10. MyBatis-Plus Mapper and DO model
11. Repository implementation in infrastructure layer
12. Assembler / converter classes
13. SQL schema/data change scripts
14. JUnit 5 test skeletons
15. Notes about assumptions, risks, and areas requiring manual refinement

Hard constraints:
- Do not over-model simple CRUD requirements.
- Do not leak MyBatis-Plus Page/Wrapper/DO objects into API contracts.
- Do not put business rules into controllers, DTOs, Mapper interfaces, or DO classes.
- Keep controllers thin.
- Keep use-case orchestration in application layer.
- Keep domain rules in domain layer only where complexity exists.
- Deliver SQL changes as scripts, not as implicit ORM migration.
- Prefer code that matches the existing project style over abstract perfection.

Required output format:
- module summary
- package structure
- API draft
- file scaffold list
- sample class skeletons
- SQL script plan
- test skeleton plan
- risks and follow-up notes