# # Codex Skills · 游戏买量广告

存放可复用的 Codex Skills，目前专注于游戏买量广告方向。

---
## 推荐小白使用一句话成功安装
把这句话发给 Agent：
帮我安装游戏广告素材分析 skill：https://raw.githubusercontent.com/zhangyifan242124-lab/ads/main/docs/install.md
你的agent就会自己给你装好的

## 🎯 game-ad-creative-analyst

**游戏买量广告素材分析与迭代 Skill**

### 能帮你做什么

不只是"看视频讲了什么"，而是落到：

- 判断素材跑得好或跑不好的真实原因
- 区分素材问题和账户问题
- 给出账户处理动作（放量 / 迭代 / 暂停 / 补数据）
- 输出可交付给剪辑团队的素材迭代方向或 brief
- 识别平台审核与内容风险

支持平台：Meta、TikTok、Google、巨量引擎、腾讯广告、快手磁力引擎

---

### 适合谁用

游戏买量优化师、素材策划、出海发行团队。

---

### 使用方式

**第一步：建立游戏档案**

在 `profiles/` 下为每款游戏创建档案，包含：
- 游戏类型和核心玩法
- 主要卖点和目标人群
- 素材禁区
- 历史有效 / 失败套路
- 常用数据基准（CPI、CTR、ROAS 等）

游戏档案只需建一次，后续复盘直接复用，不用每次重写。

**第二步：提供本次任务上下文**

按 `references/task-context-template.md` 填写：
- 投放平台、地区、投放端（Android / iOS）
- 账户阶段和优化目标
- 素材数据（支持手动粘贴或 CSV）
- 本次卡点（CPI 高 / CTR 不差但装不动 / ROAS 差 / 素材疲劳等）

**第三步：发起分析**

把视频素材或数据发给 Claude，Skill 会自动判断：
- 单条素材深挖 还是 多条素材横评
- 当前卡点对应哪些关键指标
- 问题出在吸引力、转化承接、用户质量还是账户流量

---

### 示例输入

**场景一：单条素材诊断**
> 这条素材在越南 CTR 3.2%，但 CPI 比目标高了一倍，
> 首日付费率只有 2%，帮我判断问题出在哪里。

**场景二：多条素材横评**
> 我有5支水墨风武侠素材，同一个 Campaign，
> 越南跑得好但付费率低，新加坡和泰国装不动，
> 帮我找出差异和下一步迭代方向。

**场景三：输出素材 brief**
> 基于上面的分析，帮我给剪辑出一版下一条素材的 brief。

---

### 输出结构

每次分析输出：

1. **素材拆解**：首帧、前3秒钩子、核心卖点、视频结构、CTA、落地承接
2. **数据诊断**：基于卡点选关键指标，不平均解释所有字段
3. **审核风险**：风险等级、风险位置、修改建议
4. **账户动作**：继续测试 / 谨慎放量 / 迭代复测 / 暂停
5. **素材迭代方向**：保留什么、削弱什么、强化什么

> 默认输出方向级建议。需要完整分镜或测试矩阵时，明确说"给 brief"或"出测试方案"。

---

## 目录结构
skills/

└── game-ad-creative-analyst/

├── SKILL.md

├── profiles/          # 游戏档案（每款游戏一个文件）

└── references/

├── task-context-template.md

├── intake-questions.md

├── analysis-framework.md

├── platform-risk-check.md

└── output-template.md
---

## 维护规则

- 每个 Skill 放在 `skills/<skill-name>/` 目录下
- 每个 Skill 必须包含 `SKILL.md`，frontmatter 需包含 `name` 和 `description`
- 游戏档案放在 `profiles/`，核心玩法或卖点有稳定变化时才更新

---

## 后续计划

- [ ] 素材脚本生成 Skill
- [ ] 竞品素材对比分析 Skill
- [ ] 多市场投放策略 Skill
---

