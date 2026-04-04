---
name: response-error-standard
description: Unified response, error-code, and exception-handling rules for this project
disable-model-invocation: true
user-invocable: false
---
# Response and Error Standard / 响应与错误规范

## Unified Response / 统一响应
- Use a stable response envelope / 使用统一响应包裹结构
- Recommended fields: code, message, data, requestId
- Do not expose stack traces, SQL text, or framework internals / 不暴露堆栈、SQL、框架细节
- Separate business failure from system failure clearly / 区分业务失败与系统失败

## Pagination / 分页
- Convert pagination results to project-defined DTOs / 分页结果转换为项目 DTO
- Do not expose MyBatis-Plus Page objects directly / 不直接暴露 MP Page
- Recommended fields: records, total, pageNo, pageSize

## Error Codes / 错误码
- Use stable, semantic string-based error codes / 使用稳定、语义化字符串错误码
- Keep shared error codes separate from module-specific error codes / 公共与模块错误码分离
- Do not hardcode random error strings in controllers / 不在 Controller 中硬编码魔法错误码

## Exception Handling / 异常处理
- Use global exception handling / 使用全局异常处理
- Handle business, validation, permission, and unknown exceptions separately / 分类处理业务、校验、权限、未知异常
- Include requestId or trace info when appropriate / 合适时返回 requestId 或 trace 信息
