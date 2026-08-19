# premium-ui-design-docs

**AI 产品设计总控 Skill** — 一个 Router，编排 16 个顶级设计 Skill，做出有审美的网站/App/页面。

仓库：https://github.com/linux503/premium-ui-design-docs

官网（GitHub Pages）：https://linux503.github.io/premium-ui-design-docs/

## 这是什么？

不是又一个 UI Prompt，而是一套 **AI Design Operating System**：

1. 识别你在做设计（「页面不好看」「优化 UI」「SwiftUI 改版」…）
2. 路由到 `NEW / REDESIGN / AUDIT / FIX / MATCH`
3. 自动选用对应外部专家 Skill（Anthropic `frontend-design`、OpenAI `frontend-skill`、`ckw-design`、`swiftui-design-skill`…）
4. 强制 Anti-AI Slop + 100 分 Design Audit
5. 不破坏原有业务逻辑

## 快速开始

```bash
# 安装总控 Skill（全局）
git clone https://github.com/linux503/premium-ui-design-docs.git ~/.cursor/skills/premium-ui-design-docs
```

然后在 Cursor 里说：

> 这个页面有点普通，优化一下。

或：

> 使用 premium-ui-design，读取这个 GitHub 仓库，帮我重设计这个 Landing Page。

详细安装见 [INSTALL.md](./INSTALL.md)。

## 核心文件

| 文件 | 作用 |
|---|---|
| [`premium-ui-design/SKILL.md`](./premium-ui-design/SKILL.md) | 总控入口（Cursor 自动发现） |
| [`premium-ui-design/references/skill-registry.md`](./premium-ui-design/references/skill-registry.md) | 16 个推荐 Skill + 安装命令 |
| [`premium-ui-design/core/skill-router.md`](./premium-ui-design/core/skill-router.md) | 工作流 × 平台 → Skill 路由矩阵 |
| [`premium-ui-design/prompts/cursor.md`](./premium-ui-design/prompts/cursor.md) | 可复制 Cursor 指令 |

## 编排的 16 个推荐 Skill

**Web / 通用：** `frontend-design` · `frontend-skill` · `claude-code-ui-ux-skill` · `ckw-design` · `frontend-design-review` · `ux-designer-skill`

**App / 移动：** `mobile-app-ui-design` · `swiftui-design-skill` · `mobile-app-design` · `ios-design-agent-skill` · `ios-swiftui-design-language` · `apple-design-skill` · `mobile-ui-ux-designer` · `swiftui-design-tokens` · `liquid-glass-skill` · `ui-ux-pro-max`

完整表格与 `npx skills add` 命令见 [skill-registry.md](./premium-ui-design/references/skill-registry.md)。
