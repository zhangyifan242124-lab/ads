# 安装游戏广告素材分析 Skill

本文件用于让 AI Agent 自动安装 `game-ad-creative-analyst` skill。

## 安装目标

- 仓库：https://github.com/zhangyifan242124-lab/ads
- Skill 目录：`skills/game-ad-creative-analyst`
- 本地安装后应满足：`~/.codex/skills/game-ad-creative-analyst/SKILL.md` 存在

## 安装步骤

1. 克隆仓库到临时目录或用户常用 GitHub 目录。

```bash
git clone https://github.com/zhangyifan242124-lab/ads.git
```

2. 创建 Codex skills 目录。

```bash
mkdir -p ~/.codex/skills
```

3. 复制 skill 目录。

```bash
cp -R ads/skills/game-ad-creative-analyst ~/.codex/skills/game-ad-creative-analyst
```

4. 验证安装结果。

```bash
test -f ~/.codex/skills/game-ad-creative-analyst/SKILL.md
```

## 使用方式

安装完成后，重启 Codex 或开启新对话，然后可以这样调用：

```text
使用 $game-ad-creative-analyst 分析这条游戏广告素材，并给出投放优化建议。
```

## 注意事项

- 只安装 `skills/game-ad-creative-analyst`。
- 不需要复制广告视频、投放报表或其他业务文件。
- 如果本地已经存在同名 skill，先询问用户是否覆盖。
