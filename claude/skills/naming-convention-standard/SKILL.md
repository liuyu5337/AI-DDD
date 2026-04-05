---
name: naming-convention-standard
description: "Naming consistency rules for backend, frontend, API, and SQL artifacts"
disable-model-invocation: true
user-invocable: false
---

# Naming Convention Standard / 命名规范

## General
- prefer explicit business names
- the same concept should keep the same name across layers when possible
- avoid unclear abbreviations

## Backend
- XxxCreateRequest / XxxUpdateRequest / XxxQueryRequest
- XxxResponse / XxxPageResponse
- XxxApplicationService / XxxDomainService if truly needed

## Frontend
- useXxx composables
- XxxPage / XxxDialog / XxxForm component naming
