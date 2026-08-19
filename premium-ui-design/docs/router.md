# Router：NEW / REDESIGN / AUDIT / FIX / MATCH

本 Router 只负责“选择流程”。真正的设计产物由各工作流模块生成。

## Router 输入
- 用户需求描述（可能包含：重设计/审查/修复/参考图）
- 平台线索（Web / iOS / macOS / Android / Flutter / React Native）
- 产品类型线索（Landing Page / SaaS / Dashboard / Admin / E-commerce / AI Product）
- 已有代码/界面上下文（如用户提供页面、截图、组件）

## Router 输出
- 工作流类型：`NEW | REDESIGN | AUDIT | FIX | MATCH`
- 平台：`web | ios | macos | android | flutter | react-native`
- 产品类型：`landing | saas | dashboard | admin | ecommerce | ai-product | other`
- Art Direction（最多 1 段，必须可执行）

## 第一层：工作流判定
- 出现“新建/从 0/新页面/新功能 UI”：`NEW`
- 出现“重设计/优化但已有页面”：`REDESIGN`
- 出现“审查/哪里不好/给评分/找问题”：`AUDIT`
- 出现“某个具体问题/某个组件难看/间距不对”：`FIX`
- 出现“参考图/截图/复刻风格”：`MATCH`

## 第二层：平台适配策略选择（强制不抄平台）
- Web：Responsive + Typography + Layout + Conversion UX + Motion + A11y
- iOS：Apple HIG + SwiftUI + Native Navigation + SF Symbols + Dynamic Type + Haptics
  - 原则：不要把 Web 搬进 iPhone
- macOS：Toolbar/Sidebar/Inspector/Menu Bar/Window/Sheet/Popover/Keyboard Shortcut
  - 原则：Mac App 像 Mac App
- Android：Material 3 + Compose + Adaptive Layout + Dynamic Color
  - 原则：iOS ≠ Android
- Flutter / React Native：核心品牌一致 + 平台差异化适配（navigation/back/dialog）

## 第三层：产品类型 → Art Direction 粗策略
- Landing Page：Conversion UX 优先（首屏主动作/信息层级/CTA）
- SaaS：一致性 + 功能层级（settings/onboarding/empty/error）
- Dashboard：信息密度策略（不要把所有数据 Card 化）
- Admin / 后台：效率 + 可读性（表格/筛选/快捷操作/批量行为）
- E-commerce：决策链路（搜索/筛选/商品卡/结算）
- AI Product：信任与反馈（状态、进度、错误恢复、可解释性）

## Art Direction（必填输出格式）
- Primary visual idea：____
- Typography stance：system-first / custom with constraints：____
- Layout strategy：grid/stack/rail：____
- Motion stance：Level 1 + 少量 Level 2：____
- Avoid（3 条以内）：____

