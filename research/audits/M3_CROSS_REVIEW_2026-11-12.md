# M3 交叉审核记录（2026-11-12）

> 审核人：M3
> 审核日期：2026-11-12；发布前复核与整理日期：2026-11-13。文件名沿用本轮指定日期。
> 基线：`bd73e0de22a019ecc30de0bbd3625f9f0b039126`（origin/main）。2026-11-13再次fetch后未变化。
> 方法：逐项回溯仓库原始记录、交叉比较证据登记与正文、定向查阅官方页面、查看已有审计及全部open/closed Issues与PR；区分FACT、INFERENCE、HYPOTHESIS和UNKNOWN。
> 结论：新增4项，必须修正2项、建议修正2项。均经用户批准发布；本文记录审核，不修改研究正文或冻结决策。

## 0. 问题清单

| 编号 | 问题 | 严重程度 | Issue |
|---|---|---|---|
| M3-01 | 研究证据：收费机制与厂商文案不能证明用户付费动机和心理趋势 | 必须修正 | [#10](https://github.com/zhengjiahong-ai/deep-content-community/issues/10) |
| M3-02 | 成本比较：flomo图片存储和Obsidian云服务被排除，比较范围不一致 | 建议修正 | [#11](https://github.com/zhengjiahong-ai/deep-content-community/issues/11) |
| M3-03 | 豆瓣能力边界：不能把读书笔记等同于付费电子书阅读 | 必须修正 | [#12](https://github.com/zhengjiahong-ai/deep-content-community/issues/12) |
| M3-04 | 即刻收入结构：一次未见广告不能证明几乎全靠会员 | 建议修正 | [#13](https://github.com/zhengjiahong-ai/deep-content-community/issues/13) |

## M3-01 研究证据：收费机制与厂商文案不能证明用户付费动机和心理趋势

已发布：[GitHub Issue](https://github.com/zhengjiahong-ai/deep-content-community/issues/10)。

审核基线：`bd73e0de22a019ecc30de0bbd3625f9f0b039126`。本项审核产品证据到用户结论的推导，不判断相关需求不存在。

| 项目 | 内容 |
|---|---|
| 涉及文档 | [research/competitors/jike.md:65](https://github.com/zhengjiahong-ai/deep-content-community/blob/bd73e0de22a019ecc30de0bbd3625f9f0b039126/research/competitors/jike.md#L65)（另见100、105）；[research/competitors/personal-knowledge-vs-community.md:102](https://github.com/zhengjiahong-ai/deep-content-community/blob/bd73e0de22a019ecc30de0bbd3625f9f0b039126/research/competitors/personal-knowledge-vs-community.md#L102)（另见121、168–170）；[research/errc/m4-new-bmc-input.md:88](https://github.com/zhengjiahong-ai/deep-content-community/blob/bd73e0de22a019ecc30de0bbd3625f9f0b039126/research/errc/m4-new-bmc-input.md#L88)；[research/trends/key-trends-m4.md:75](https://github.com/zhengjiahong-ai/deep-content-community/blob/bd73e0de22a019ecc30de0bbd3625f9f0b039126/research/trends/key-trends-m4.md#L75)（另见76、89）。 |
| 问题类型 | 结论过强 / 证据无效 |
| 具体问题 | 即刻卡把“愿意为控制可见性与信息过滤付费的核心用户”标为 FACT（E-447、E-453），并推出用户为“谁能看到”而非“存得更好”付费；ERRC进一步称它比“更好的知识结构”更好卖。但 E-447 是登录方式，E-448 是付费入口观察，E-453 是会员权益，没有购买动机、功能归因或转化比较。比较稿102行同样从收费项推出用户愿意为基础设施/身份表达付费。趋势稿75–76、89行又把即刻“限时日记”和豆瓣“文化足迹”的厂商文案，当成普遍心理、用户资产态度及公开表达门槛上升的证据。产品机制和定位可以确认为 FACT；上述需求、偏好与时间趋势目前为 UNKNOWN／HYPOTHESIS。它们已被用于收费设计和外部机会/威胁判断，会使待验证假设看起来已经得到用户证据支持。 |
| 修改建议 | 保留有出处的收费机制及厂商定位；将付费动机、可见性相对知识结构的销售优势、表达顾虑普遍性及上升趋势降为 HYPOTHESIS，删除确定性排序。若要保留强结论，补真实购买动机/选择或同口径跨期证据。同步修正产品卡、比较稿、趋势稿和ERRC中的同源推论；不据此更改已冻结方向。 |
| 严重程度 | 必须修正 |

证据定位：[docs/EVIDENCE_REGISTRY.md:62](https://github.com/zhengjiahong-ai/deep-content-community/blob/bd73e0de22a019ecc30de0bbd3625f9f0b039126/docs/EVIDENCE_REGISTRY.md#L62)（E-427 厂商自述、实测未确认）；[docs/EVIDENCE_REGISTRY.md:82](https://github.com/zhengjiahong-ai/deep-content-community/blob/bd73e0de22a019ecc30de0bbd3625f9f0b039126/docs/EVIDENCE_REGISTRY.md#L82)（E-447–E-455）；[research/competitors/obsidian.md:96](https://github.com/zhengjiahong-ai/deep-content-community/blob/bd73e0de22a019ecc30de0bbd3625f9f0b039126/research/competitors/obsidian.md#L96)为同类付费动机推论。2026-11-12复核[即刻 App Store](https://apps.apple.com/cn/app/id966129812)仍有“限时日记”文案与会员报价，这支持厂商陈述存在，不支持群体心理或购买原因。未把 Android 未见入口解释为所有平台没有该功能。

去重：#8讨论P0/P1验证顺序，M4-04讨论监管证据类型；二者均未处理这里的收费/营销证据到用户行为结论的跃迁。

发布前澄清：产品存在付费功能是机制事实；真实用户购买动机、不同权益相对吸引力、群体心理上升趋势均未验证，不据此判定需求不存在。

## M3-02 成本比较：flomo图片存储和Obsidian云服务被排除，比较范围不一致

已发布：[GitHub Issue](https://github.com/zhengjiahong-ai/deep-content-community/issues/11)。

审核基线：`bd73e0de22a019ecc30de0bbd3625f9f0b039126`。

| 项目 | 内容 |
|---|---|
| 涉及文档 | [research/bmc/revenue-cost-assessment-m4.md:80](https://github.com/zhengjiahong-ai/deep-content-community/blob/bd73e0de22a019ecc30de0bbd3625f9f0b039126/research/bmc/revenue-cost-assessment-m4.md#L80)（表中84–85行）；[research/bmc/xiaoyuzhou-revenue-cost-m4.md:125](https://github.com/zhengjiahong-ai/deep-content-community/blob/bd73e0de22a019ecc30de0bbd3625f9f0b039126/research/bmc/xiaoyuzhou-revenue-cost-m4.md#L125)（129–130行）；对照[research/competitors/obsidian.md:60](https://github.com/zhengjiahong-ai/deep-content-community/blob/bd73e0de22a019ecc30de0bbd3625f9f0b039126/research/competitors/obsidian.md#L60)（60–66行）。 |
| 问题类型 | 逻辑矛盾 / 结论过强 |
| 具体问题 | 财务比较将flomo写成“仅文字”“只承担文字存储”，由文字不占配额推出边际成本接近零；Obsidian收入列包含Sync/Publish，成本却按“本地存储”写成不承担托管、接近零。flomo官方文档实际列出图片/附件存储；Obsidian官方Sync提供远端存储，Publish包含网站托管，产品卡65行也已列云服务与带宽。这里把完整收费业务的收入与本地客户端/纯文字子场景的成本配在一起，不能支持轻工具与小宇宙的成本强弱比较。 |
| 修改建议 | 统一比较口径：区分Obsidian免费本地客户端、Sync和Publish，区分flomo文字与图片/附件；收入和成本覆盖同一服务范围。可列出相应存储、同步、流量等成本驱动因素，但配额政策不能证明成本金额或边际成本接近零；实际成本曲线和审核负担保留UNKNOWN。 |
| 严重程度 | 建议修正 |

外部核验（2026-11-12）：[flomo存储与导出](https://help.flomoapp.com/basic/storage.html)明确图片存储与文字不计配额是不同规则；[Obsidian Sync](https://obsidian.md/sync)列存储容量并支持图片、音视频、PDF同步；[Obsidian Publish](https://obsidian.md/publish)包含网站托管。本次核实的是服务边界，没有测量内部云账单或毛利。

去重：A-04已指出小宇宙RSS不能证明低成本；本项新增的是竞品本地/云服务范围混用及flomo存储对象遗漏，不重复报告小宇宙RSS成本问题。

发布前澄清：用户免费存储配额不等于服务商零成本；Obsidian免费本地客户端与Sync/Publish付费云服务必须分别比较。

## M3-03 豆瓣能力边界：不能把读书笔记等同于付费电子书阅读

已发布：[GitHub Issue](https://github.com/zhengjiahong-ai/deep-content-community/issues/12)。

审核基线：`bd73e0de22a019ecc30de0bbd3625f9f0b039126`。

| 项目 | 内容 |
|---|---|
| 涉及文档 | [research/competitors/douban.md:41](https://github.com/zhengjiahong-ai/deep-content-community/blob/bd73e0de22a019ecc30de0bbd3625f9f0b039126/research/competitors/douban.md#L41)（41–43、55、91、98、102、108、112）；[research/competitors/personal-knowledge-vs-community.md:28](https://github.com/zhengjiahong-ai/deep-content-community/blob/bd73e0de22a019ecc30de0bbd3625f9f0b039126/research/competitors/personal-knowledge-vs-community.md#L28)；[docs/COMPETITOR_RESEARCH_MATRIX.md:103](https://github.com/zhengjiahong-ai/deep-content-community/blob/bd73e0de22a019ecc30de0bbd3625f9f0b039126/docs/COMPETITOR_RESEARCH_MATRIX.md#L103)；传播到[research/errc/m4-new-bmc-input.md:61](https://github.com/zhengjiahong-ai/deep-content-community/blob/bd73e0de22a019ecc30de0bbd3625f9f0b039126/research/errc/m4-new-bmc-input.md#L61)及82行、[research/bmc/xiaoyuzhou-revenue-cost-m4.md:164](https://github.com/zhengjiahong-ai/deep-content-community/blob/bd73e0de22a019ecc30de0bbd3625f9f0b039126/research/bmc/xiaoyuzhou-revenue-cost-m4.md#L164)。 |
| 问题类型 | 证据无效 / 结论过强 |
| 具体问题 | 豆瓣卡称笔记绑定付费电子书，未购买者只剩作品级表达，继而将其解释成片段讨论受到版权/付费墙限制。可是卡22行明确没有体验笔记编辑界面，E-443只记录“有笔记功能；电子书需购买后才能阅读”，并注明未验证划线/片段锚定。2026-11-12公开网页核验发现，《围城》条目下有按页码组织的摘录笔记及回应；样例笔记显示第319页、摘录和回复，可公开读取。电子书全文访问条件不能直接外推为全部笔记、摘录与回应的条件。此误读同时缩小了现有替代方案，并被ERRC用来支持“只存片段与链接则版权成本无”的判断。 |
| 修改建议 | 将书籍条目的读书笔记、页码摘录与回应，同电子书阅读器内阅读/划线分开描述；把尚未操作的写入权限、精确回跳及付费边界标UNKNOWN。修正产品卡及两张比较表，撤回以E-443证明“电子书要买才能做笔记”及新方案版权成本为零的推论；版权成本仍待独立证据，不由这个竞品页面决定。 |
| 严重程度 | 必须修正 |

原始证据：[docs/EVIDENCE_REGISTRY.md:78](https://github.com/zhengjiahong-ai/deep-content-community/blob/bd73e0de22a019ecc30de0bbd3625f9f0b039126/docs/EVIDENCE_REGISTRY.md#L78)（E-443）。
新增网页核验：[《围城》的笔记列表](https://book.douban.com/subject/1008145/annotation)、[第319页笔记及回应](https://book.douban.com/annotation/18363273/)。只证明本次可访问页面的结构；没有登录发笔记/回复，没有购买电子书，不声称已验证阅读器原句回跳或全部账号权限，也不作法律结论。

去重：#7、A-08和M4-09处理无讨论的泛化；本项针对E-443的具体证据错配和付费边界，原有记录未指出该问题及其版权成本传播。

主要反证（2026-11-13核验）：[豆瓣官方帮助中心：笔记](https://help.douban.com/evaluation?app=4#t2-q1)说明可在图书条目点击“写笔记”创建该书笔记；同页将读书笔记描述为批注、摘抄及随感，并说明可标记原文。不能把电子书阅读全文的购买门槛等同于全部读书笔记的使用门槛。本轮未登录操作的具体账号权限仍为UNKNOWN；以E-443推出版权成本为零的结论应撤回。

## M3-04 即刻收入结构：一次未见广告不能证明几乎全靠会员

已发布：[GitHub Issue](https://github.com/zhengjiahong-ai/deep-content-community/issues/13)。

审核基线：`bd73e0de22a019ecc30de0bbd3625f9f0b039126`。

| 项目 | 内容 |
|---|---|
| 涉及文档 | [research/competitors/jike.md:69](https://github.com/zhengjiahong-ai/deep-content-community/blob/bd73e0de22a019ecc30de0bbd3625f9f0b039126/research/competitors/jike.md#L69)（另见74、90、109）；[research/bmc/xiaoyuzhou-revenue-cost-m4.md:136](https://github.com/zhengjiahong-ai/deep-content-community/blob/bd73e0de22a019ecc30de0bbd3625f9f0b039126/research/bmc/xiaoyuzhou-revenue-cost-m4.md#L136)；[research/bmc/revenue-cost-assessment-m4.md:91](https://github.com/zhengjiahong-ai/deep-content-community/blob/bd73e0de22a019ecc30de0bbd3625f9f0b039126/research/bmc/revenue-cost-assessment-m4.md#L91)。 |
| 问题类型 | 结论过强 / 逻辑矛盾 |
| 具体问题 | 即刻卡把会员列为“主力”收入，并由“实测无广告”推出“几乎全靠会员”，压缩版继续沿用；财务比较据此称即刻不投广告、靠会员“活得下去”。但E-454仅是一位普通账号一次首页和圈子浏览未见广告；E-431明确官网未公开收入结构，不能证明没有其他收入；卡74行也注明营收、会员人数和转化率未公开。已发现收费入口不足以判断会员贡献、广告收入是否存在或订阅能否覆盖经营成本。 |
| 修改建议 | 保留“存在会员收费入口”“本次所测页面未见广告”“官网有商务合作联系方式”；会员占比、其他收入及经营可持续性标UNKNOWN。删除“主力／几乎全靠会员／靠会员活得下去”的确定性论断，同步收敛两份财务对照。无需为此估算营收。 |
| 严重程度 | 建议修正 |

来源定位：[docs/EVIDENCE_REGISTRY.md:66](https://github.com/zhengjiahong-ai/deep-content-community/blob/bd73e0de22a019ecc30de0bbd3625f9f0b039126/docs/EVIDENCE_REGISTRY.md#L66)（E-431）；[docs/EVIDENCE_REGISTRY.md:87](https://github.com/zhengjiahong-ai/deep-content-community/blob/bd73e0de22a019ecc30de0bbd3625f9f0b039126/docs/EVIDENCE_REGISTRY.md#L87)（E-452–E-454）；[research/competitors/jike.md:22](https://github.com/zhengjiahong-ai/deep-content-community/blob/bd73e0de22a019ecc30de0bbd3625f9f0b039126/research/competitors/jike.md#L22)（未覆盖付费权益体验）。本项不反向声称即刻必有广告或已经亏损。

去重：M4-01针对小宇宙分成/费率证据冲突；本项针对即刻收入构成与可持续性，现有Issue及审核记录未覆盖。

## 1. 审核范围、通过项及去重

A完成：U01–U08、research/phase1/PHASE1_FINDINGS_2026-11-08.md、research/m1/M1_RESEARCH_INTEGRATION_2026-11-12.md、M1_PHASE_CLOSURE_2026-11-12.md。逐案证据见下方用户研究核验索引；新增0，已有#8、M4-07。
B完成：research/bmc/下xiaoyuzhou-bmc-complete、xiaoyuzhou-bmc-m1/m2/m3、xiaoyuzhou-bmc-financial-assessment、overall-assessment、customer-interface-assessment、infrastructure-assessment、m2-value-proposition-swot-evidence、xiaoyuzhou-revenue-cost-m4、revenue-cost-assessment-m4（均.md）；research/errc/m3-new-bmc-input.md、m4-new-bmc-input.md及research/m1/M1_ERRC_NEW_BMC_2026-11-12.md。
C完成：research/competitors/market-forces.md与industry-forces.md（后者仅核对组内衔接）；research/trends/key-trends-m4.md、research/m1/M1_KEY_TRENDS_2026-11-12.md、M1_MACRO_ENVIRONMENT_2026-11-12.md。
D完成：research/competitors/xiaoyuzhou-user-journey.md、wechat-read-user-journey.md、ximalaya.md、content-platform-matrix.md、flomo.md、obsidian.md、douban.md、jike.md、personal-knowledge-vs-community.md、content-capture-matrix.md；docs/COMPETITOR_RESEARCH_MATRIX.md；docs/EVIDENCE_REGISTRY.md和research/competitors/EVIDENCE_M3.md相关证据行。M3三产品原有审计结果复用，不声称重做全部体验。
E完成：四项候选均重新读原文/原始证据行，针对托管服务和豆瓣笔记做官方/原站页面核验，并重读三份既有audit、刷新全部Issues/PR与main。四项同根传播已各自合并。

### 外部环境18项覆盖与判定

| 类别 | 逐项覆盖及本轮判断 | 文件定位 |
|---|---|---|
| 市场5项 | 市场分类、需求和诉求、市场问题、切换成本、收入吸引力均有事实、影响、O/T及局限；归纳边界通过。原报告统计未全部独立复核。 | market-forces.md:15–75 |
| 行业5项 | 现有竞争者、新进入者、替代品、供应链厂商、利益相关者均有分析；仅验组内衔接。成本/费率/使用率推论延续A-04至A-08，不新增。 | industry-forces.md:30–178 |
| 趋势4项 | 技术、行业管理/监管、社会文化、社会经济均已提交；M1稿保留平台与行业统计区分。监管证据错配及双稿归入M4-04/05；使用率不能推出低频归入A-07；厂商文案推出社会心理趋势归入M3-01。 | M1_KEY_TRENDS:7–74；key-trends-m4.md:67–113 |
| 宏观4项 | 全球市场、大宗商品与其他资源、资本市场、经济基础设施均覆盖并联系BMC；GDP/居民消费/联网/社融等选取公报抽核。第三方转载社融来源问题归#9。 | M1_MACRO_ENVIRONMENT:6–72 |

### 通过项（限定范围）

- 九模块整合表及价值流：xiaoyuzhou-bmc-complete.md:11–35保留付款参与者、内容供给、商单服务费UNKNOWN，未把广告主预算等同平台确认收入，监管归约束。
- M1财务评估：xiaoyuzhou-bmc-financial-assessment.md:13、19–22、28–42、50–62、84–88，费率、金额、盈利、转化率与稳定现金流均未冒充事实。
- M2客户侧及SWOT证据：customer-interface-assessment.md:9、17–24、32–40、48–55、67–68，m2-value-proposition-swot-evidence.md:7–14，事实与作用机制分列，保留非会员/单账号/1小时边界和U05反例。
- M1条件式ERRC与新BMC保留假设、待建立合作与金额未知；强制社区问题另归#8，故不是整个新BMC通过。
- M2小宇宙与微信读书旅程、喜马拉雅扫描、content-platform-matrix.md:20–40：区分免费实测与PLUS官方权益，喜马拉雅未测能力UNKNOWN；不把个人私密笔记当成多人私密交流。
- 直接查看E-223、E-224、E-225三个仓库截图：小宇宙15/月与120连续包年及权益；微信读书首月9次月19/特惠年168及版权排除；喜马拉雅年188/前2月16第三月30及套餐差异，与M2矩阵31–32行相符。只核对当日页面报价，没有支付验证。
- flomo 99/299年、Obsidian Sync年付折算4美元与Publish8美元、即刻20/月128/年等官网展示数值抽查一致；不证明各端全部账号报价或实际付费权益。
- A阶段具体通过项见下方用户研究核验索引，不将AI模拟合入8人样本，不将便利访谈推成群体比例。

### 已知重复、已修复与不新增

- #7与A-03/A-08/M4-09：公开讨论空位、单次入口推全产品/全市场；包含四产品比较中“没有回顾/没人同时解决”的全称结论，归原范围问题，不新建。
- #8：P0/P1与强制社区冲突，PR #6未合并，不能称已修复。已有描述足够，不另写重复评论。
- #9：社融35.6万亿元、8.3%本次在国家统计局英文公报核对一致，含可比口径；M2增8.5%也一致。不新增评论。
- M4-01/02/03：费率未核与过期价格/权益。特别校正：E-223截图同时含会员周报、图标/主题与同传/优惠；两份权益清单不全不等于互斥，不将差集直接报“功能不存在”。
- M4-04/05/08：监管证据、课件术语、2024/2025调查不同样本，延续既有记录。没有把两个年度的数据合成趋势。
- M4-06：当前矩阵100–106行已有M3摘要，但与行标题错位（如跨来源行填价格、来源上下文行填回顾），107–113仍待填；属于同一三列合并验收事项，保留给M1，不新建。
- M4-07及Phase1已知缺口：U07编号/体验时间，U03元数据；不重复。
- A-04/A-05/A-06/A-07：RSS低成本、费率、监管伙伴、使用率/态度推论延续。新成本项M3-02只报竞品业务范围错配。
- A-01/A-09/A-11在PR #2已修复；M1整合和基础设施已收敛部分成本/Apple依赖/无跟帖措辞。M4_PHASE2_AUDIT早期“财务趋势未提交”已被其后附交付状态和main文件取代，不再报缺文件。
- 未新增纯风格、表格编号或细小命名问题；SWOT里焦点产品与项目视角混用的个别条目先作整合口径提醒，没有认定新实质错误。

### 外部证据索引与UNKNOWN

核验日期均2026-11-12，Firecrawl抓原站内容。页面描述仅证明页面当时所述，不证明后台经济数据/实际权限。外部页面未写入公共证据登记表。
1. https://help.flomoapp.com/basic/storage.html HTTP200：文字不计配额，图片/附件有存储限制，推翻“仅文字”；不能推成本为0。
2. https://obsidian.md/sync HTTP200：远端存储配额、多格式同步、年付4美元/月起；https://obsidian.md/publish HTTP200：网站托管、年付8美元/站/月。免费本地与付费云服务需分开。
3. https://help.flomoapp.com/membership/pro.html HTTP200：99/299及PRO/MAX。MCP当前PRO起可用与原稿MAX表述有差异，但本轮不确定历史更新时间、也非主比较结论，暂记动态差异不新建Issue。
4. https://apps.apple.com/cn/app/id966129812 HTTP200：会员价目、48小时文案仍在；不等于Android入口/购买原因已核实。
5. https://book.douban.com/subject/1008145/annotation HTTP200：页码笔记及回应链接；https://book.douban.com/annotation/18363273/ HTTP200：319页笔记及回复；另抽https://book.douban.com/annotation/18137290/可见161页及回复。没有登录/购买/发布。详情页抓取metadata混有无关网站SEO字段，只采用与列表互相印证的豆瓣正文结构，不采用这些metadata作来源身份依据。web工具独立获取未成功。
6. https://www.stats.gov.cn/english/PressRelease/202602/t20260228_1962661.html HTTP200：2025统计公报，社融与M2、GDP、联网率、消费等抽核；不推出小宇宙经营增长。
7. https://file.digitaling.com/eImg/uimages/20240724/1721788588565026.pdf Firecrawl与web均403。2024统计只完成仓库证据归属、样本/口径和推论边界检查，未重新逐图验数；不是数字错误发现。
8. 未独立重跑任何产品任务，未接触受访者；M4附件local未入库仍限制复现。不据此断言记录虚构。真实支付转化、收入占比、成本曲线、页码到全文精确跳转、未测版本能力均UNKNOWN。



## 2. 用户研究核验索引



| 编号 | 有实质影响的行为、需求、采用与替代判断 | 原始记录行号 | 综合材料对应与判定 |
|---|---|---|---|
| U01 | 浏览社媒及线下讨论，噪声与信息筛选困难；表达欲低，无明确笔记需求；AI过滤只是提出的替代办法，实际使用UNKNOWN；新社区迁移未验证 | research/user-interviews/U01-interview.md 17–37、47–65 | Phase1 43；M1整合22。归纳一致 |
| U02 | 主动记笔记并理解PID/PLC；平板笔记/WPS方便够用；概念积极反馈不证明迁移与持续采用；跨源关联仍是假设 | research/user-interviews/U02-interview.md 20–37、48–65 | Phase1 44、56、62；M1整合23；收束24。反例完整 |
| U03 | 转发文案后翻聊天记录一次；是否成功找回UNKNOWN；笔记难保留触发背景；现有方案总体够用；QQ讨论是另一事件；功能认可与广告厌恶属于态度 | research/user-interviews/U03-interview.md 19–40、45–64 | Phase1 45；M1整合24。未将态度升级为实际采用 |
| U04 | 点赞、进一步了解人物、抖音分享与简单交流；不等于找回原视频；备忘录够用；期待回应来自概念介绍后表态，具体情境未核；观点关联是新奇兴趣 | research/user-interviews/U04-interview.md 19–42、48–69 | Phase1 46；M1整合25。保留足够性和采用边界 |
| U05 | 发朋友圈与收藏单集，认为回找方便；捕捉灵感及附图链接有摩擦；不太会用新讨论功能；采用条件是足够简单；跨源关联认可尚无真实任务演示 | research/user-interviews/U05-interview.md 20–44、60–74 | Phase1 47、54–62；M1整合26；收束24、32。支持捕捉探索，同时反驳普遍回找困难 |
| U06 | 备忘录写观点及教学理解，回找不便，课堂已有讨论；备忘录/OneNote勉强够用；专装App可能小题大做；OneNote标签是替代设想，非已实行行为 | research/user-interviews/U06-interview.md 20–45、61–75 | Phase1 48、56–64；M1整合27；收束24、32。痛点与拒绝采用均保留 |
| U07 | 小说评论、截图微信分享、书签与记事本保存；偶尔回味，回找摩擦与瞬时共鸣；截图省事，未表达新工具采用；没有跨源关联行为 | research/user-interviews/U07-interview.md 20–41 | Phase1 49；M1整合28；收束24、30–37。案例归纳一致，但元数据问题见A-02 |
| U08 | 公号观点未保存且未回找；另一视频分享后线下讨论；出处不一定有用；实时呼出/微信转发/更简单为概念接受条件；常驻可见是愿望 | research/user-interviews/U08-interview.md 19–46 | Phase1 50、54–62；M1整合29。明确保留预测与行为区别 |

以上 Phase1 指 research/phase1/PHASE1_FINDINGS_2026-11-08.md；M1整合指 research/m1/M1_RESEARCH_INTEGRATION_2026-11-12.md；收束指 research/m1/M1_PHASE_CLOSURE_2026-11-12.md。



### 用户研究通过范围与元数据限制



1. 样本外推与AI隔离通过。Phase1 7、25–37、66–76；M1整合10、33–37、128；收束18、81–83明确便利样本、自述与合成材料边界。指定综合材料中未发现用AI模拟增加真实样本数或推出总体比例。
2. 反例保留通过。U02工具足够、U05回找方便且讨论意愿弱、U06现有工具勉强够用和独立App阻力均进入Phase1 44、47–48、56–62、M1整合23、26–27及收束24、32。
3. P0个人沉淀作为优先验证方向通过。U03 25–34、U05 27–32、U06 20–32、U07 29–34支持部分捕捉/上下文/回找摩擦；M1整合54、136–138和收束24–26、49保留采用未验证。证据不支持声称已完成统一功能排序或证明商业需求。
4. P1轻量讨论作为HYPOTHESIS通过。真实交流与回应期待可追溯八案索引，收束30–37、50明确迁移及持续参与未知；强制社区原型另归Issue #8。
5. 行为、态度与愿望大体区分通过。U03 49、U04 50–52、U05 39–44、U06 40–45标明概念反馈；U08 25、36和综合稿29/Phase1 50保留未实际回找。未把喜欢或觉得有用写成已发生购买、留存或迁移。
6. 替代方案与采用门槛通过。Phase1 43–64、86–100、M1整合22–29、收束24–26对应原始工具路径和拒绝条件。付费未知保留于Phase1 64、M1整合48、收束86。

### 元数据复核边界

U03 10–15日期、时长、筛选及许可未知，已在Phase1 123记录，沿用已有待补项。U04 10–15区分聊天跨度与有效时长，不构成已证实的时长错误。U05/U06 8–10的19:00—20:00窗口与10分钟时长可以并存，现有证据不足以认定冲突。U01/U02 13明确记录许可未单独记录，不能推出未获许可或访谈不真实。
U07的B节体验与A节访谈应分别评价；后补体验日期晚于Phase1不能单独证明A节访谈日期错误。



## 3. 发布前复核与给M1的建议

2026-11-13查询全部Issues（两页，第2页为空）时，普通Issues仅#7、#8、#9，均open且无评论；PR #1/#2/#3/#5已合并，#4被#5替代，#6仍open未合并。未发现本轮四项已有重复或main修复。发布后逐项GET核实#10—#13的真实URL，未追加已有Issue评论。

豆瓣新增主要反证为[官方帮助中心“笔记”](https://help.douban.com/evaluation?app=4#t2-q1)，2026-11-13成功访问。官方说明可从图书条目“写笔记”入口创建笔记；该说明不同于本轮实际登录操作，未测权限继续UNKNOWN。

建议M1先处理#10与#12，收敛收费/需求推论及豆瓣笔记边界，再统一#11与#13的成本、收入比较口径。既有#7—#9和M4问题沿原记录处理。不能把用户需求未验证写成需求不存在，也不能把费用、收入未知反推为亏损、零成本或必然存在广告。

本轮没有独立复现产品体验、认证访谈真实性或计算内部经营数据。没有修改研究正文、证据登记表、SWOT、ERRC、BMC或docs/REVIEW_STATUS.md。临时工作记录不属于提交范围。
