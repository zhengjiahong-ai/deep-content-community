# 全组证据登记表

> 维护人：M4  
> 创建日期：2026-11-10  
> 依据：`docs/EVIDENCE_GUIDELINES.md` 第 3 节  
> 用途：本表是最终报告脚注的唯一上游。正文中每一条重要结论，都必须能在本表找到一行对应记录。

## 0. 使用规则

1. 一行一条证据，一条证据只支持一个具体陈述。`Claim` 必须具体，不能写"产品体验很好"这类无法核对的判断。
2. 编号格式 `E-<成员>-<三位序号>`，例如 `E-M4-001`。各成员只使用自己的号段，避免编号冲突。
3. `Type` 只能填 **FACT**、**INFERENCE**、**HYPOTHESIS** 三种之一，定义见 `docs/EVIDENCE_GUIDELINES.md` 第 1 节。
4. `Published` 拿不到发布日期时写"未标明"，不要猜。
5. `Accessed` 填**实际打开该页面**的日期（YYYY-MM-DD）。没有亲自打开、只是从他人文档看到的，Type 后加 `(转引)`。
6. 厂商自述、应用商店介绍、官方帮助中心属于"企业公开宣称"，`Limitation` 必须写"厂商自述"，不能单独用来证明产品效果或用户满意度。
7. 修改他人登记过的行时，在该行末尾追加备注，不要直接覆盖原记录。
8. 未核实、查不到的信息，如实写"未核实"或"未标明"，不得为了表格整齐而填写推测值。

## 1. 号段分配

| 成员 | 号段 | 负责研究范围 |
| --- | --- | --- |
| M1 | `E-M1-001` 起 | 真实访谈、用户任务链、小宇宙价值主张、宏观环境 |
| M2 | `E-M2-001` 起 | 小宇宙、微信读书、喜马拉雅；小宇宙客户细分/渠道/客户关系 |
| M3 | `E-M3-001` 起 | Snipd、Readwise Reader、Cubox；小宇宙核心资源/关键业务/重要合作 |
| M4 | `E-M4-001` 起 | flomo、豆瓣、Obsidian、即刻；小宇宙收入来源/成本结构；关键趋势 |
| 共用 | `E-SHARED-001` 起 | 第一阶段归档材料、跨成员转引入口、通用参考资料 |

## 2. 登记表

| ID | Claim | Type | Source | URL | Published | Accessed | Scope | Limitation | Used in | 登记人 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| E-SHARED-001 | 小宇宙 App Store 页面存在，公开介绍涉及播客发现、时间点评论、互动与收听记录 | FACT (转引) | Apple App Store｜小宇宙 | https://apps.apple.com/cn/app/id1488894313 | 未标明 | 2026-11-10 | 中国大陆区 iOS | 转引自 `docs/COMPETITOR_RESEARCH_MATRIX.md` 第 4 节，登记人未亲自打开原页面；厂商自述 | 竞品生态、M2 研究入口 | M4 |
| E-SHARED-002 | 微信读书 App Store 页面存在，公开介绍涉及书籍发现、书中观点讨论、阅读数据与笔记 | FACT (转引) | Apple App Store｜微信读书 | https://apps.apple.com/cn/app/id952059546 | 未标明 | 2026-11-10 | 中国大陆区 iOS | 转引同上；未亲自核验；厂商自述 | 竞品生态、M2 研究入口 | M4 |
| E-SHARED-003 | 喜马拉雅提供主播帮助中心，可用于核验创作者计划与内容供给机制 | FACT (转引) | 喜马拉雅主播帮助中心 | https://www.ximalaya.com/helper/ | 未标明 | 2026-11-10 | 中国大陆 | 转引同上；未亲自核验 | 小宇宙重要合作对照、M2 | M4 |
| E-SHARED-004 | Snipd 官网公开介绍播客片段保存、转录、摘要、问答与导出能力 | FACT (转引) | Snipd 官网 | https://www.snipd.app/ | 未标明 | 2026-11-10 | 全球 | 转引同上；未亲自核验；厂商自述 | M3 内容捕捉研究入口 | M4 |
| E-SHARED-005 | Readwise Reader 官方文档覆盖多来源阅读、高亮、批注与 Highlights 同步 | FACT (转引) | Readwise Reader Docs | https://docs.readwise.io/reader/docs | 未标明 | 2026-11-10 | 全球 | 转引同上；未亲自核验；厂商自述 | M3 研究入口 | M4 |
| E-SHARED-006 | Cubox 官网与帮助中心公开介绍收藏、阅读、高亮、想法、搜索、回顾与分享 | FACT (转引) | Cubox 官网 / 帮助中心 | https://cubox.pro/ ；https://help.cubox.pro/reader/9183/ | 未标明 | 2026-11-10 | 中国大陆 | 转引同上；未亲自核验；厂商自述 | M3 研究入口 | M4 |
| E-SHARED-007 | flomo 帮助中心公开说明快速记录、标签、相关笔记、回顾与 AI 能力 | FACT (转引) | flomo 帮助中心 | https://help.flomoapp.com/ | 未标明 | 2026-11-10 | 中国大陆 | 转引同上；M4 将在本表补充亲自核验后的分项证据 | 3.3 个人知识管理、BMC 收入对照 | M4 |
| E-SHARED-008 | Obsidian 官方帮助文档说明反向链接（backlinks）与笔记链接关系 | FACT (转引) | Obsidian Help | https://obsidian.md/help/plugins/backlinks | 未标明 | 2026-11-10 | 全球 | 转引同上；M4 将在本表补充亲自核验后的分项证据 | 3.3 知识关联、M3 研究入口 | M4 |
| E-SHARED-009 | 豆瓣 App Store 页面与社区指导原则页存在，可用于核验书影音条目、评分评论与小组治理 | FACT (转引) | Apple App Store｜豆瓣；豆瓣社区指导原则 | https://apps.apple.com/cn/app/id907002334 ；https://www.douban.com/about/guideline | 未标明 | 2026-11-10 | 中国大陆 | 转引同上；未亲自核验；厂商自述 | 3.4 内容社区、BMC 治理成本 | M4 |
| E-SHARED-010 | 即刻 App Store 页面存在，公开介绍涉及兴趣圈子、动态、评论与同好连接 | FACT (转引) | Apple App Store｜即刻 | https://apps.apple.com/cn/app/id966129812 | 未标明 | 2026-11-10 | 中国大陆 | 转引同上；未亲自核验；厂商自述 | 3.4 内容社区 | M4 |
| E-SHARED-011 | 第一阶段已归档 8 份真实访谈（U01—U08）与 16 份 AI 模拟记录 | FACT | 仓库文件 `research/user-interviews/`、`research/ai-simulations/` | 仓库内路径 | 未标明 | 2026-11-10 | 本组便利样本 | 便利抽样，不能外推总体 | 1.2、4.2 | M4 |
| E-SHARED-012 | 项目唯一硬期限为 2026-11-30 20:00（北京时间），由 M1 在 Moodle 提交整合 PDF | FACT | `README.md`、`docs/COURSE_DELIVERABLES.md` | 仓库内路径 | 未标明 | 2026-11-10 | 本项目 | 依据教师原始作业说明，仓库未存原件 | 全文交付节奏 | M4 |

## 3. 核验状态统计

| 状态 | 数量 | 说明 |
| --- | ---: | --- |
| 已亲自核验 | 0 | 登记人直接打开页面并记录事实 |
| 转引待核验 | 10 | E-SHARED-001 至 E-SHARED-010 |
| 仓库内事实 | 2 | E-SHARED-011、E-SHARED-012 |

> 本表创建时只有转引入口，属于"研究起点"而非"已完成核验"。各成员核验后必须把自己的行改为已核验，并补 `Published`、`Scope`、`Limitation`。

## 4. 各成员待补来源清单

| 成员 | 需要补的来源 |
| --- | --- |
| M1 | 8 份访谈的日期与访谈员；小宇宙价值主张的官方表述；宏观 4 项所需统计口径与原始发布机构 |
| M2 | 小宇宙、微信读书、喜马拉雅的实测记录（设备/版本/日期）；三平台会员价格页面 |
| M3 | Snipd、Readwise Reader、Cubox 的定价页与导出说明页；AI 功能的官方限制说明 |
| M4 | flomo、豆瓣、Obsidian、即刻的官方页面与实际体验记录；小宇宙收入/成本的可核实入口；关键趋势所需行业数据原始来源 |

## 5. 已知问题

1. `docs/COMPETITOR_RESEARCH_MATRIX.md` 第 3 节比较表仍全部为"待填"，需要各成员按列填写，并在本表登记支撑证据。
2. 18 个外部环境子方向的**教材原文名称与主要问题**在仓库中尚无任何记录，四人共用同一缺口。
3. `research/phase1/PHASE1_FINDINGS_2026-11-08.md` 引用的 `research/user-interviews/M3-interview-summary.md` 在仓库中不存在，属断链，需原记录人确认。
