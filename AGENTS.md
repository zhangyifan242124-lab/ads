# 工作区规范

## 目标

这个目录用于维护准备上传到 GitHub 的 Codex skills，只存放可公开或可共享的 skill 本体与必要说明。

## 目录约定

- `skills/<skill-name>/`：每个可复用 skill 单独一个目录。
- 每个 skill 目录必须包含 `SKILL.md`。
- 可选资源放在 skill 内部的 `references/`、`scripts/`、`assets/`、`agents/` 等目录。

## 禁止内容

- 不放原始广告视频、截图批量输出、投放报表、账号数据、客户私有资料。
- 不放 `.env`、token、cookie、API key、密码、证书或其他密钥。
- 不放本地缓存、构建产物、临时分析输出。

## 命名规则

- Skill 目录使用 lowercase hyphen-case，例如 `game-ad-creative-analyst`。
- 引用文档使用 lowercase hyphen-case，文件名能直接说明用途。

## 验证要求

- 上传前检查每个 `SKILL.md` 都有 frontmatter，且包含 `name` 和 `description`。
- 上传前检查仓库状态，确认没有误加入私有数据或大文件。
- `git push`、创建远程仓库、公开发布前必须得到用户确认。
