---
name: openapi-dto-error-template
description: Reusable template for API overview, DTOs, validation, and error model
disable-model-invocation: true
user-invocable: false
---

# API Output Template / API 输出模板

Use this template when producing API design output:

## API overview
- purpose
- actors
- compatibility notes

## Endpoint list
- method + path
- summary
- permission / auth assumption

## Request models
- field
- type
- required
- meaning
- validation

## Response models
- field
- type
- meaning

## Error model
- error code
- scenario
- message
- frontend handling note
