# 安装与使用

## 最快开始（3 步）

### 1. 安装总控 Skill

```bash
# 全局（所有项目可用）
git clone https://github.com/linux503/premium-ui-design-docs.git ~/.cursor/skills/premium-ui-design-docs

# 或仅当前项目
git clone https://github.com/linux503/premium-ui-design-docs.git .cursor/skills/premium-ui-design-docs
```

重启 Cursor。之后说「这个页面不好看，优化一下」应自动触发。

### 2.（可选）安装外部专家 Skill

按场景选装，完整列表见 [`premium-ui-design/references/skill-registry.md`](./premium-ui-design/references/skill-registry.md)。

Web 最小套装：
```bash
npx skills add https://github.com/anthropics/skills --skill frontend-design
npx skills add https://github.com/openai/skills --skill frontend-skill
npx skills add connerkward/ckw-design-skill
```

iOS 最小套装：
```bash
npx skills add wholiver/swiftui-design-skill
npx skills add dickwu/apple-design-skill
```

### 3. 在 Cursor 里使用

**自然语言（推荐）**
> 这个 Landing Page 有点普通，帮我重新设计一下。

**显式调用**
> 使用 premium-ui-design，读取 https://github.com/linux503/premium-ui-design-docs ，优化这个 Dashboard。

**带平台**
> 用 premium-ui-design 给这个 SwiftUI 设置页做 REDESIGN，要有苹果风，避免 AI 模板感。

---

## 不安装外部 Skill 也能用吗？

可以。`premium-ui-design` 已内置：
- Design Intelligence（禁止直接写 UI）
- Anti-AI Slop 门禁
- 100 分 Design Audit + Gate
- 平台适配原则
- Skill Router（知道该参考哪些外部 Skill 的方法论）

安装外部 Skill 只是在专项上更强（例如 Liquid Glass API、可搜索配色库）。

---

## 远程读取 GitHub（不 clone）

在对话里直接说：

```text
读取 https://github.com/linux503/premium-ui-design-docs 的 premium-ui-design/SKILL.md
和 references/skill-registry.md，按 premium-ui-design 总控流程执行。
```

Cursor Agent 会拉取仓库内容并按 Router 执行。

---

## 目录说明

```
premium-ui-design/
├── SKILL.md                 # 总控入口（Cursor 自动发现）
├── core/skill-router.md     # 路由矩阵
├── references/skill-registry.md  # 16 个推荐 Skill + 安装命令
├── docs/                    # 设计流程模块
└── prompts/cursor.md        # 可复制总控指令
```
