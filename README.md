# Codex Skills

这个仓库用于存放可复用的 Codex skill。

## 目录结构

- `skills/game-ad-creative-analyst/`：游戏买量广告素材分析与迭代 skill。
- `skills/weread-assistant/`：微信读书助手 skill。

## 维护规则

- 每个 skill 必须放在 `skills/<skill-name>/` 下。
- 每个 skill 必须包含 `SKILL.md`，并在 frontmatter 中包含 `name` 和 `description`。
- 不上传原始广告视频、投放报表、账号数据、密钥、token、cookie 或本地缓存。
- 示例中的敏感值必须使用环境变量或占位符。

## 使用方式

复制需要的 skill 目录到本地 Codex skills 目录，或按你的 Codex 环境的 skill 安装方式导入。
