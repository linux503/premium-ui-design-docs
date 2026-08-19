# Workflows（NEW / REDESIGN / AUDIT / FIX / MATCH）

每个工作流都必须遵循同一条纪律：
先 Design Intelligence → Art Direction → 方案生成 → Anti-AI Slop 自检 → Design Audit → 迭代。

## NEW（从 0 设计）
1) 填充 Design Intelligence 卡
2) 确定 Art Direction（导演意图）
3) 输出信息架构 + 层级布局草图
4) 生成最小 token + 关键组件与状态
5) UX/视觉层级策略 + motion/interaction 方案
6) Design Audit（100 分 + Gate）

## REDESIGN（重做已有 UI）
1) 诊断问题：层级/密度/一致性/可读性/可用性
2) 明确“哪些要改、哪些必须不动”（避免破坏业务逻辑）
3) 输出新层级体系（含状态与关键组件）
4) Anti-AI Slop：检查是否出现模板化脏模式
5) Audit + Gate + 迭代计划

## AUDIT（审查现状）
1) 先给出评分表（总分 100）
2) 必改项/可选项列表（按影响排序）
3) 提供最小修改路径（尽量不牵连业务）

## FIX（定向修复）
1) 指定修复范围（组件/页面/状态）
2) 给出替换方案与理由
3) 风险说明：改动可能带来的连锁影响
4) 必须再次自检 Anti-AI Slop

## MATCH（参考图复刻）
1) 解析参考图：Layout / Grid / Hierarchy / Typography / Color / Spacing / Radius / Components / Motion implication
2) 区分：应该学习的 vs 不应该复制的
3) 结合目标产品重新设计（不做“照抄风格”）

