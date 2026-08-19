# Skill Router（总控 → 外部专家）

`premium-ui-design` 根据 **工作流 × 平台 × 产品类型** 自动选用外部 Skill。  
每次任务最多加载 **1 个主 Skill + 1 个辅助 Skill**，避免上下文爆炸。

---

## 路由流程

```text
用户设计需求
    ↓
premium-ui-design 识别：NEW / REDESIGN / AUDIT / FIX / MATCH
    ↓
识别平台：Web / iOS / macOS / Android / Flutter / RN
    ↓
识别产品类型：Landing / SaaS / Dashboard / App / Admin …
    ↓
选定主 Skill + 辅助 Skill（见下表）
    ↓
执行 Design Intelligence → Art Direction → 实现 → Audit → Critic
```

---

## 工作流 × 平台 路由表

### Web

| 工作流 | 产品类型 | 主 Skill | 辅助 Skill |
|---|---|---|---|
| NEW | Landing Page / 官网 | `frontend-skill` | `frontend-design` |
| NEW | SaaS / Dashboard | `frontend-design` | `ui-ux-pro-max` |
| NEW | 需要强设计系统 | `claude-code-ui-ux-skill` | `ckw-design` |
| REDESIGN | 任意 Web | `ckw-design` | `frontend-design` |
| AUDIT | 任意 Web | `frontend-design-review` | `ux-designer-skill` |
| FIX | 配色/字体/间距 | `claude-code-ui-ux-skill` | — |
| FIX | 交互/表单/导航 | `ux-designer-skill` | — |
| MATCH | 参考图复刻 | `frontend-skill` | `ckw-design` |

### iOS / macOS（SwiftUI）

| 工作流 | 场景 | 主 Skill | 辅助 Skill |
|---|---|---|---|
| NEW | 新 App / 新页面 | `swiftui-design-skill` | `ios-swiftui-design-language` |
| NEW | 需要 Design System | `ios-swiftui-design-language` | `swiftui-design-tokens` |
| NEW | iOS 26+ / Liquid Glass | `liquid-glass-skill` | `apple-design-skill` |
| REDESIGN | 已有 SwiftUI UI | `swiftui-design-skill` | `apple-design-skill` |
| AUDIT | 审查现有 App | `ios-design-agent-skill` | `apple-design-skill` |
| FIX | Token 不统一 | `swiftui-design-tokens` | — |
| FIX | HIG 合规 | `apple-design-skill` | — |

### Android

| 工作流 | 主 Skill | 辅助 Skill |
|---|---|---|
| NEW / REDESIGN | `mobile-app-design` | `ui-ux-pro-max`（stack: jetpack-compose） |
| AUDIT | `mobile-ui-ux-designer` | `ux-designer-skill` |

### Flutter / React Native（跨平台）

| 工作流 | 主 Skill | 辅助 Skill |
|---|---|---|
| NEW / REDESIGN | `mobile-app-ui-design` | `mobile-app-design` |
| 全流程 UX | `mobile-ui-ux-designer` | `ui-ux-pro-max` |
| AUDIT | `mobile-app-design` | `ux-designer-skill` |

### 不确定平台 / 综合任务

| 场景 | 主 Skill |
|---|---|
| 从零选风格 + 配色 + 字体 | `ui-ux-pro-max` |
| 大型知识库检索 | `claude-code-ui-ux-skill` |
| 提高品味、避免模板感 | `ckw-design` |

---

## 阶段 × Skill 分工

| 阶段 | 负责 | 外部 Skill 参与 |
|---|---|---|
| Design Intelligence | `premium-ui-design` | `ckw-design`（design-thinking） |
| Art Direction | `premium-ui-design` | `frontend-skill` / `swiftui-design-skill` |
| Design System | `premium-ui-design` | `ios-swiftui-design-language` / `swiftui-design-tokens` / `ui-ux-pro-max` |
| 实现 | Builder | 平台主 Skill |
| Design Audit | `premium-ui-design`（100 分） | `frontend-design-review` / `ios-design-agent-skill` |
| Design Critic | `premium-ui-design` | `ios-design-agent-skill`（iOS）/ `ckw-design`（Web） |

---

## 给 Cursor 的执行指令（内部）

选定 Skill 后，在回复开头声明：

```text
[premium-ui-design Router]
工作流: REDESIGN
平台: Web
产品: SaaS Dashboard
主 Skill: ckw-design
辅助 Skill: frontend-design
Art Direction: （一句话）
```

然后按 `premium-ui-design` 流程执行，并融入主/辅 Skill 的专项原则。
