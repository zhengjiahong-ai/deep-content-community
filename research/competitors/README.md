# M3 竞品与基础设施研究（第二阶段）

> 负责人：M3（内容捕捉与阅读工具、基础设施与行业影响力）
> 依据：`docs/TASK_ASSIGNMENTS.md` v2.0（2026-11-08）
> 开始日期：2026-11-08
> 证据基准日：2026-11-08（网页来源的访问日期都是这天）

## 1. 这个目录里有什么

任务书给 M3 的七项交付都在这里。另有一份给 M1 的模块影响说明，对应任务书 §8 的要求，不算额外任务。

| 任务书交付 | 文件 | 状态 |
| --- | --- | --- |
| Snipd 深度研究 | `snipd.md` | 研究 + 实测（v4.3.22） |
| Readwise Reader 深度研究 | `readwise-reader.md` | 研究 + 实测（Public Beta Update #14） |
| Cubox 深度研究 | `cubox.md` | 研究 + 实测（v8.4.1） |
| 内容捕捉产品比较矩阵 | `content-capture-matrix.md` | 实测版 |
| 小宇宙 BMC：核心资源、关键业务、重要合作 | `../bmc/xiaoyuzhou-bmc-m3.md` | 公开资料 + 后台实测（v3.4.4） |
| 基础设施总体评估 | `../bmc/infrastructure-assessment.md` | 实测修订版 |
| 行业影响力 5 项 | `industry-forces.md` | 5/5 |
| 给 M1 的模块影响说明 | `../errc/m3-new-bmc-input.md` | 供 M1 整合 |

另外两份是配套：`industry-forces.md` 开头附了课程口径的五个子方向；`EVIDENCE_M3.md` 是证据登记表（E-302 起），给 M4 汇总用。

## 2. 我按这几条写

- 结论后面标 `[FACT]`、`[INFERENCE]` 或 `[HYPOTHESIS]`（`docs/EVIDENCE_GUIDELINES.md:8-14`）。
- 功能状态只用五种标签：实测支持、官方资料支持、第三方资料提及、未核实、不适用（`docs/COMPETITOR_RESEARCH_MATRIX.md:90-95`）。
- 数据和价格以实测、官方页面为准，不猜，也不替别人填默认值。
- 没找到入口就写清楚查了哪里，不写“产品没有这个功能”（`docs/EVIDENCE_GUIDELINES.md:58`）。
- 价格、会员权益、AI 额度都记页面和访问日期；未公开的收入、成本、用户数不写。
- 第三方估算只当参考，不拿一个数字当事实。
- AI 模拟访谈（`research/ai-simulations/M3-*`）不作为这里的证据。

## 3. 不碰已经被验证的能力

`docs/PROJECT_BRIEF.md:121-127` 说得很清楚：Snipd 已经覆盖播客片段捕捉、转录、摘要、问答和导出；Readwise Reader 和 Cubox 已经覆盖多来源保存、标注、检索和回顾。所以“片段保存”“跨来源收藏”“AI 摘要”这些，我不再当市场空白。

这份研究只看三件事：捕捉一个片段要几步、是不是在消费现场完成；来源上下文（时间点、页码、原文链接）能不能留住并跳回；能力边界和成本，包括 AI 语言和额度、导出和平台依赖、中文播客支持。

这三条对应任务书 `TASK_ASSIGNMENTS.md:144-150` 的关键问题。
