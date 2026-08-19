# 外部 Skill 注册表（推荐 16 + 总控）

`premium-ui-design` 不重复造轮子，而是**总控路由**到下列高质量 Skill。  
安装后由总控 Skill 按任务/平台自动选用；未安装时，总控会内化其核心原则（见 `core/skill-router.md`）。

> 仓库地址（给 Cursor 读取）：https://github.com/linux503/premium-ui-design-docs

---

## Web / 通用 UI（6 个）

| Skill | 适合做什么 | 审美 | 推荐 | GitHub | 安装（Cursor） |
|---|---|:---:|:---:|---|---|
| **frontend-design** | 新页面、Landing、Dashboard、美化现有 UI | ⭐⭐⭐⭐⭐ | 首选 | [anthropics/skills](https://github.com/anthropics/skills/tree/main/skills/frontend-design) | `npx skills add https://github.com/anthropics/skills --skill frontend-design` |
| **frontend-skill** | 高级官网、产品页、视觉层级、动效 | ⭐⭐⭐⭐⭐ | 首选 | [openai/skills](https://github.com/openai/skills/tree/main/skills/.curated/frontend-skill) | `npx skills add https://github.com/openai/skills --skill frontend-skill` |
| **claude-code-ui-ux-skill** | 大型 UI/UX 知识库、配色、字体、风格 | ⭐⭐⭐⭐⭐ | 强烈推荐 | [nicohodt/claude-code-ui-ux-skill](https://github.com/nicohodt/claude-code-ui-ux-skill) | `npx skills add nicohodt/claude-code-ui-ux-skill` |
| **ckw-design** | 提高设计品味，避免千篇一律 | ⭐⭐⭐⭐⭐ | 很推荐 | [connerkward/ckw-design-skill](https://github.com/connerkward/ckw-design-skill) | `npx skills add connerkward/ckw-design-skill` |
| **frontend-design-review** | 检查已做好的页面哪里丑、哪里要改 | ⭐⭐⭐⭐ | 很实用 | [microsoft/skills](https://github.com/microsoft/skills/tree/main/.github/skills/frontend-design-review) | `npx skills add https://github.com/microsoft/skills --skill frontend-design-review` |
| **ux-designer-skill** | UX、交互、表单、导航、移动端、WCAG | ⭐⭐⭐⭐ | 偏专业 UX | [szilu/ux-designer-skill](https://github.com/szilu/ux-designer-skill) | `npx skills add szilu/ux-designer-skill` |

---

## App UI / UX（10 个）

| Skill | 主要用途 | 推荐度 | GitHub | 安装（Cursor） |
|---|---|:---:|---|---|
| **mobile-app-ui-design** | App 页面设计、改版、Screen Flow、组件、Onboarding | ⭐⭐⭐⭐⭐ | [ceorkm/mobile-app-ui-design](https://github.com/ceorkm/mobile-app-ui-design) | `npx skills add ceorkm/mobile-app-ui-design` |
| **swiftui-design-skill** | iOS/macOS SwiftUI 高级审美、避免 AI 味 | ⭐⭐⭐⭐⭐ | [wholiver/swiftui-design-skill](https://github.com/wholiver/swiftui-design-skill) | `npx skills add wholiver/swiftui-design-skill` |
| **mobile-app-design** | iOS + Android + React Native 全平台设计规范 | ⭐⭐⭐⭐⭐ | [awesome-skills/mobile-app-design](https://github.com/awesome-skills/mobile-app-design) | `npx skills add awesome-skills/mobile-app-design` |
| **ios-design-agent-skill** | 检查现有 iOS App 哪里不好看 | ⭐⭐⭐⭐⭐ | [vermont42/iOS-Design-Agent-Skill](https://github.com/vermont42/iOS-Design-Agent-Skill) | `npx skills add vermont42/iOS-Design-Agent-Skill --skill ios-design-agent-skill` |
| **ios-swiftui-design-language** | SwiftUI Design System / Token / Components | ⭐⭐⭐⭐⭐ | [onatcipli/skills](https://github.com/onatcipli/skills/tree/main/skills/ios-swiftui-design-language) | `npx skills add onatcipli/skills --skill ios-swiftui-design-language` |
| **apple-design-skill** | Apple HIG + Liquid Glass + Apple 风格 | ⭐⭐⭐⭐⭐ | [dickwu/apple-design-skill](https://github.com/dickwu/apple-design-skill) | `npx skills add dickwu/apple-design-skill` |
| **mobile-ui-ux-designer** | Flutter / RN / iOS / Android UX 全流程 | ⭐⭐⭐⭐ | [mdrmuhaimin/agentic-skills](https://github.com/mdrmuhaimin/agentic-skills/tree/main/codex/mobile-ui-ux-designer) | `npx skills add mdrmuhaimin/agentic-skills --skill mobile-ui-ux-designer` |
| **swiftui-design-tokens** | SwiftUI 配色、字号、间距、圆角、动画统一 | ⭐⭐⭐⭐ | [eworthing/agent-skills](https://github.com/eworthing/agent-skills/tree/main/swiftui-design-tokens) | `npx skills add eworthing/agent-skills --skill swiftui-design-tokens` |
| **liquid-glass-skill** | iOS 26+ / macOS 26+ Liquid Glass | ⭐⭐⭐⭐ | [haider-nawaz/liquid-glass-skill](https://github.com/haider-nawaz/liquid-glass-skill) | `npx skills add haider-nawaz/liquid-glass-skill` |
| **ui-ux-pro-max** | Web + iOS + Android + Flutter + RN 综合 | ⭐⭐⭐⭐⭐ | [nextlevelbuilder/ui-ux-pro-max-skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill) | `npx skills add nextlevelbuilder/ui-ux-pro-max-skill` |

---

## 一键安装（推荐组合）

### 最小 Web 套装（4 个）
```bash
npx skills add https://github.com/anthropics/skills --skill frontend-design
npx skills add https://github.com/openai/skills --skill frontend-skill
npx skills add connerkward/ckw-design-skill
npx skills add https://github.com/microsoft/skills --skill frontend-design-review
```

### 最小 iOS / SwiftUI 套装（4 个）
```bash
npx skills add wholiver/swiftui-design-skill
npx skills add onatcipli/skills --skill ios-swiftui-design-language
npx skills add dickwu/apple-design-skill
npx skills add vermont42/iOS-Design-Agent-Skill --skill ios-design-agent-skill
```

### 全平台综合（1 个就够）
```bash
npx skills add nextlevelbuilder/ui-ux-pro-max-skill
```

### 安装总控 Skill 本身
```bash
git clone https://github.com/linux503/premium-ui-design-docs.git ~/.cursor/skills/premium-ui-design-docs
# 或项目内：
git clone https://github.com/linux503/premium-ui-design-docs.git .cursor/skills/premium-ui-design-docs
```

Cursor 会读取 `.cursor/skills/premium-ui-design-docs/premium-ui-design/SKILL.md`。

---

## 使用原则

1. **总控优先**：永远先走 `premium-ui-design` 的 Design Intelligence → Router → Audit。
2. **外部 Skill 是专家**：按 `core/skill-router.md` 选用，不堆叠全部 Skill。
3. **未安装也能用**：总控已内化 Anti-AI Slop、Audit 100 分制、平台原则；安装外部 Skill 只是加强专项能力。
4. **不破坏业务**：外部 Skill 只指导视觉/交互/结构，不改业务逻辑。
