# premium-ui-design-docs

**AI 产品设计总控 Skill** — 一个 Router：识别你在做 UI/UX 设计，然后自动编排工作流并路由到对应专家 Skill，最后用 **100 分 Design Audit + Anti-AI Slop 门禁**收口交付。

[官网（GitHub Pages）](https://linux503.github.io/premium-ui-design-docs/) · [仓库](https://github.com/linux503/premium-ui-design-docs)

---

## 一句话能触发

在 Cursor 里说：

> 这个页面有点普通，优化一下。

它会先做 Design Intelligence + Art Direction，再选择 `NEW / REDESIGN / AUDIT / FIX / MATCH` 工作流，并给出可执行的实现与审查清单。

---

## 快速开始

### 1) 安装总控 Skill（全局）

```bash
git clone https://github.com/linux503/premium-ui-design-docs.git ~/.cursor/skills/premium-ui-design-docs
```

详细安装见 [`INSTALL.md`](./INSTALL.md)。

### 2) 可选：安装 Web / iOS 专家 Skill（增强审美）

#### Web

```bash
npx skills add https://github.com/anthropics/skills --skill frontend-design
npx skills add connerkward/ckw-design-skill
```

#### iOS（SwiftUI）

```bash
npx skills add wholiver/swiftui-design-skill
npx skills add dickwu/apple-design-skill
```

---

## Cursor 用法示例

- `NEW`：帮我做一个高级感 SaaS Landing Page
- `REDESIGN`：重排这个 Dashboard 的信息层级（别 AI 模板感）
- `AUDIT`：审查现有页面哪里丑、哪里需要改，并给修改计划
- `FIX`：定向修复按钮/表单状态设计（loading/disabled/error）
- `MATCH`：用参考图复刻布局与层级（不盲抄）

---

## 核心入口文件

| 文件 | 作用 |
|---|---|
| [`premium-ui-design/SKILL.md`](./premium-ui-design/SKILL.md) | 总控入口（Cursor 自动发现） |
| [`premium-ui-design/references/skill-registry.md`](./premium-ui-design/references/skill-registry.md) | 16 个推荐 Skill + 安装命令 |
| [`premium-ui-design/core/skill-router.md`](./premium-ui-design/core/skill-router.md) | 工作流 × 平台 → Skill 路由矩阵 |
| [`premium-ui-design/prompts/cursor.md`](./premium-ui-design/prompts/cursor.md) | 可复制 Cursor 指令模板 |

完整表格见 [`skill-registry.md`](./premium-ui-design/references/skill-registry.md)。
