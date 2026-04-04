---
name: security-baseline
description: Security baseline for backend/frontend/application changes
disable-model-invocation: true
user-invocable: false
---
# Security Baseline / 安全基线

Always review for / 始终检查:
- authentication / 认证
- authorization / 授权
- input validation / 输入校验
- SQL injection / expression injection / command injection / 注入风险
- output encoding / 输出编码
- sensitive data exposure / 敏感信息暴露
- file upload/download safety / 文件上传下载安全
- secrets in config/code/logs / 配置、代码、日志中的密钥
- auditability of critical actions / 关键操作审计

Rules / 规则:
- Never hardcode secrets
- Never log passwords, tokens, or sensitive personal data
- Validate untrusted input
- Verify permission checks on sensitive operations
- State security assumptions explicitly / 明确安全假设
