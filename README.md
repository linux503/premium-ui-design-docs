# premium-ui-design-docs

**AI 产品设计总控 Skill** — 一个 Router：识别你在做 UI/UX 设计，然后自动编排工作流并路由到对应专家 Skill，最后用 **100 分 Design Audit + Anti-AI Slop 门禁**收口交付。

[进入官网](https://linux503.github.io/premium-ui-design-docs/) · [查看仓库](https://github.com/linux503/premium-ui-design-docs/)

> 官网入口：<https://linux503.github.io/premium-ui-design-docs/>

---

## 你会得到什么

- 一个 **总控设计 Skill**：不是单纯美化 UI，而是先识别任务，再路由到正确工作流
- 一套 **专业设计流程**：Design Intelligence → Art Direction → Implementation → Design Audit
- 一组 **外部专家 Skill 编排能力**：Web、iOS、SwiftUI、Dashboard、Landing Page 都能按场景调用
- 一个 **可直接访问的官网**：用于展示定位、安装方式、案例提示词与使用方法

---

## 一句话能触发

在 Cursor 里说：

> 这个页面有点普通，优化一下。

它会先做 Design Intelligence + Art Direction，再选择 `NEW / REDESIGN / AUDIT / FIX / MATCH` 工作流，并给出可执行的实现与审查清单。

---

## 自动路由规则（关键词触发 + 固定链路 + 统一 10 维度审查）

当 Cursor 遇到下面关键词时，自动调用本总控设计 Skill（`premium-ui-design`）：
`优化UI / redesign / 美化 / App设计 / 网站设计 / 官网设计 / SwiftUI / iOS / macOS / Android / Flutter / React Native / Landing Page / Dashboard`

内部自动判断链路（固定顺序）：

Web
→ Frontend Design
→ UI UX Pro（`ui-ux-pro-max`）
→ Responsive
→ Typography
→ Motion

iOS / macOS
→ Apple HIG
→ SwiftUI Design
→ Anti AI-Slop
→ Liquid Glass
→ SF Symbols
→ Native Components

Android
→ Material 3
→ Jetpack Compose
→ Android Navigation

Flutter / React Native
→ Mobile UI
→ iOS / Android 平台差异
→ Adaptive Design

最后统一跑一个 Design Audit（固定顺序，10 维度）：
视觉层级 → 字体 → 配色 → 间距 → 圆角 → 图标 → 组件 → 动效 → 响应式 → AI模板味

---

## 先看官网

如果你想先看展示效果、再决定怎么装怎么用，直接打开：

- [premium-ui-design 官网](https://linux503.github.io/premium-ui-design-docs/)

官网里已经包含：

- 产品定位
- Web / iOS 安装命令
- Cursor 用法示例
- 专业案例提示词
- 总控 Router 思路

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

## 适合什么场景

- 想让 Cursor 不只是“写组件”，而是先做设计判断
- 想优化官网、Landing Page、Dashboard、后台系统
- 想做更像 Apple 风格的 SwiftUI / iOS 页面
- 想让 AI 输出少一点模板感，多一点审美控制
- 想在交付前增加一层 Design Audit + Anti-AI Slop 门禁

---

## Cursor 用法示例

- `NEW`：帮我做一个高级感 SaaS Landing Page
- `REDESIGN`：重排这个 Dashboard 的信息层级（别 AI 模板感）
- `AUDIT`：审查现有页面哪里丑、哪里需要改，并给修改计划
- `FIX`：定向修复按钮/表单状态设计（loading/disabled/error）
- `MATCH`：用参考图复刻布局与层级（不盲抄）

---

## 专业案例提示词（可直接复制）

### 案例 1（Web NEW｜SaaS Landing Page）

```text
使用 premium-ui-design 总控设计 Skill。

任务类型：NEW
平台：Web
产品类型：SaaS Landing Page（AI 产品）

目标：首屏 5 秒内让用户理解“我们做什么 + 为什么可信 + 下一步怎么做”（并明确 CTA）。

要求：
1) 先输出 Design Intelligence 卡（Product / Audience / Core task / density / visual focus / avoid）
2) 再输出 Art Direction（一句话 + 主视觉理念 + typography/layout/motion 策略 + 3 条 avoid）
3) 输出一页可落地结构：Hero + Proof（数字/引用）+ Features（分层）+ Pricing teaser + FAQ + Footer
4) 覆盖完整 state/交互：默认、hover、disabled、loading、empty/error（表单/弹窗为准）
5) Anti-AI Slop 自检：任何“模板化脏模式”必须说明设计理由；严重命中则直接移除
6) 最后给出 100 分 Design Audit + Gate + 下一轮迭代计划
7) 工程实现建议：组件拆分、token 最小集、哪些不该动（禁止改业务逻辑）
```

### 案例 2（Web REDESIGN｜Dashboard 信息层级重构）

```text
使用 premium-ui-design 总控设计 Skill。

任务类型：REDESIGN
平台：Web
产品类型：Dashboard（后台管理风格）

上下文：
- 我会给你当前页面截图/代码片段
- 直觉问题：信息层级不清、模块同构模板感、表格/筛选交互状态不完整

强制规则：
1) 禁止大改业务逻辑/数据结构/权限接口；只改 UI 结构、层级、组件状态与交互
2) 必须先做 AUDIT：给出必改项/可选项（按影响排序）再进入 REDESIGN
3) Anti-AI Slop：任何“圆角卡片堆叠/同构模板/无意义渐变/不可读文案淡色”需要一票否决或给出理由
4) 输出：新信息架构 + 关键组件 state 表（Filters、Table、Empty/Error、Loading skeleton）
5) 最后输出 100 分 Audit + Gate + 最小改动清单（Next changes）
```

### 案例 3（iOS AUDIT+FIX｜SwiftUI Settings 苹果风）

```text
使用 premium-ui-design 总控设计 Skill。

任务类型：AUDIT 然后 FIX
平台：iOS
框架：SwiftUI
场景：Settings 页面（包含表单、开关、选择器、以及危险操作）

输入：我会贴 Settings 的 SwiftUI 视图代码（或截图）

审查目标（必须覆盖）：
- Apple HIG 气质是否原生（不要把 Web/模板感搬进 iPhone）
- 第一眼/第二眼/下一步路径是否清晰（Primary attention / Secondary attention / Primary action path）
- 完整交互 state：Default、Focused、Disabled、Loading、Empty、Error
- 可访问性落地：Dynamic Type、VoiceOver 语义（至少说明 label/traits/可访问顺序）
- Motion：Level 1 + 少量 Level 2（默认禁用无意义夸张动效）

输出：
1) Design Intelligence 卡（缺什么先追问）
2) Art Direction（苹果风 + 不做什么）
3) 100 分 Design Audit + Anti-AI Slop 门禁
4) FIX：逐条给“具体替换建议”（哪些 Section/控件怎么改、按钮文案怎么改、间距怎么改）
5) 工程实现建议：token 最小集、组件拆分方案、哪些不该动
```

---

## 核心入口文件

| 文件 | 作用 |
|---|---|
| [`premium-ui-design/SKILL.md`](./premium-ui-design/SKILL.md) | 总控入口（Cursor 自动发现） |
| [`premium-ui-design/references/skill-registry.md`](./premium-ui-design/references/skill-registry.md) | 16 个推荐 Skill + 安装命令 |
| [`premium-ui-design/core/skill-router.md`](./premium-ui-design/core/skill-router.md) | 工作流 × 平台 → Skill 路由矩阵 |
| [`premium-ui-design/prompts/cursor.md`](./premium-ui-design/prompts/cursor.md) | 可复制 Cursor 指令模板 |

完整表格见 [`skill-registry.md`](./premium-ui-design/references/skill-registry.md)。

---

## 推荐阅读顺序

1. 先看 [官网](https://linux503.github.io/premium-ui-design-docs/)
2. 再看 [`INSTALL.md`](./INSTALL.md)
3. 然后读 [`premium-ui-design/SKILL.md`](./premium-ui-design/SKILL.md)
4. 最后按需复制上面的案例提示词到 Cursor
