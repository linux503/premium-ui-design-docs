# Design Audit（100 分制 + Gate 门禁）

设计输出不能直接 `Done`。必须基于量化 rubric 审查并执行门禁。

## 评分表（总分 100）
- Visual Hierarchy：15
- Layout & Spacing：10
- Typography：10
- Color：10
- UX Clarity：15
- Platform Native：10
- Consistency：10
- Accessibility：5
- Responsive / Adaptive：5
- Brand Personality：5
- Anti-AI Slop：5
- （可选）Implementation clarity：0~5（当实现细节也是交付范围时）

## Gate 规则
- `90–100`：可以交付
- `80–89`：自动优化明显问题
- `70–79`：必须重新 Review + 修改
- `<70`：Art Direction 或 Layout 有问题 → 重新设计

特殊门禁：
> 即使总分 > 90，只要 Anti-AI Slop 严重命中，也不能完成。

## 必须输出的审查结果结构
- Top issues（必改项，按影响排序）
- Next changes（可选优化项）
- Risk notes（如果不改会怎样）
- Refined plan（下一轮如何修改）

