# CLAUDE.md

## 开发规则

**写 Fresh 代码前必须：**
1. 调用 `deno-skill/deno-frontend` skill，或
2. 阅读 `/home/djch/projects/fresh/docs/latest` 相关文档

不要凭记忆写代码，Fresh 2.x 的 API 可能与旧版本不同。

## Fresh 2.x 规范

- 路由导出名必须用 `handler`（单数），不能用 `handlers`（复数）
  - 原因：Deno linter 目前只接受 `handler`
  - PR: https://github.com/denoland/deno_lint/pull/1495

## 开发服务器

- Fresh 2 + Vite 开发服务器默认端口是 **5173**（不是 8000）
- 如果 5173 被占用，Vite 会自动尝试 5174、5175...

## Supabase

- 项目 ID: ckudrvhvhbhqzhzmvasl
- 存储桶: files (public)
