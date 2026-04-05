---
name: openapi-dto-error-template
description: OpenAPI + DTO + unified response and error templates
disable-model-invocation: true
user-invocable: false
---

# OpenAPI DTO Error Template / 接口 DTO 与错误模板

## Use for
- request DTO template
- response DTO template
- page response template
- unified error response template

## Rules
- field meaning must be explicit
- response DTO should not mirror persistence objects mechanically
- include requestId in error envelope when appropriate
