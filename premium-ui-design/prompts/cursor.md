# Cursor 总控指令（可直接复制）

## 方式 A：自然语言（推荐）

直接说即可，无需点名 Skill：

> 这个页面不好看，优化一下。

> 帮我设计一个 SaaS Dashboard，要有高级感，不要 AI 模板感。

> 这个 SwiftUI 设置页重新设计，苹果风。

---

## 方式 B：显式总控 + 读取 GitHub

```text
使用 premium-ui-design 总控设计 Skill。

先读取 GitHub 仓库：
https://github.com/linux503/premium-ui-design-docs

必读文件：
1. premium-ui-design/SKILL.md
2. premium-ui-design/core/skill-router.md
3. premium-ui-design/references/skill-registry.md

然后对当前项目执行：
- 工作流：（NEW / REDESIGN / AUDIT / FIX / MATCH）
- 平台：（Web / iOS / macOS / Android / Flutter / RN）
- 产品类型：（Landing / SaaS / Dashboard / App …）

强制纪律：
1. 禁止直接写 UI 代码 → 先 Design Intelligence + Art Direction
2. 按 skill-router 选定 1 主 + 1 辅外部 Skill 并融入其原则
3. Anti-AI Slop 自检
4. 100 分 Design Audit + Gate
5. Design Critic 独立审查
6. 不改业务逻辑

输出必须包含：
- Router 摘要（工作流 / 平台 / 主Skill / Art Direction）
- 设计决策清单
- UI/UX 结构方案
- 关键状态设计
- Audit 评分表
- 迭代计划
```

---

## 方式 C：只做审查

```text
使用 premium-ui-design 的 AUDIT 工作流。
读取 https://github.com/linux503/premium-ui-design-docs 的 design-audit 规则。
对当前页面做 100 分制评分，Anti-AI Slop 严重问题一票否决。
主 Skill：frontend-design-review（Web）或 ios-design-agent-skill（iOS）。
```

---

## 方式 D：从零做产品页

```text
使用 premium-ui-design，NEW 工作流。
平台：Web，产品：AI SaaS Landing Page。
主 Skill：frontend-skill，辅助：ui-ux-pro-max。
先给 3 个 Art Direction 方向让我选，选定后再实现。
```
