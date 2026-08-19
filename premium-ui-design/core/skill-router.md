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

## 平台自动判断链路（按你指定的链）

`premium-ui-design` 在完成工作流判定后，会按平台走固定链路（用于指导“该怎么设计/怎么审查”），最后统一跑 `Design Audit`。

### Web
Web
→ Frontend Design
→ UI UX Pro
→ Responsive
→ Typography
→ Motion

### iOS / macOS
iOS / macOS
→ Apple HIG
→ SwiftUI Design
→ Anti AI-Slop
→ Liquid Glass
→ SF Symbols
→ Native Components

### Android
Android
→ Material 3
→ Jetpack Compose
→ Android Navigation

### Flutter / React Native
Flutter / React Native
→ Mobile UI
→ iOS / Android 平台差异
→ Adaptive Design

### 最终统一审查（Design Audit：10 维度）
设计交付前，必须用下面 10 个维度统一审查（顺序固定）：
视觉层级 → 字体 → 配色 → 间距 → 圆角 → 图标 → 组件 → 动效 → 响应式 → AI模板味

每项 `0~10`，汇总为总分 `100`，并执行 Gate：
- `90–100`：可以交付
- `80–89`：自动优化明显问题
- `70–79`：必须重新 Review + 修改
- `<70`：Art Direction 或 Layout 有问题 → 重新设计

特殊门禁：
> 即使总分 > 90，只要 **AI模板味** 严重命中，也不能完成。

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
