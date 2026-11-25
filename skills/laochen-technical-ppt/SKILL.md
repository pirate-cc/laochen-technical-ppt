---
name: laochen-technical-ppt
description: "为中文学术报告、教学、产品、培训或文化演示梳理知识树、撰写上屏文案、制作或审阅 PowerPoint。自拟页题不超过七字，正文讲清图中现象、证据支持的判断及其实际作用。围绕听众的问题串起各章，制作可编辑 PPT 和逐页原生讲演动画。"
---

# 老陈技术汇报 PPT

按听众、用途和本次材料把主题讲清楚，交付文案可直接使用的可编辑 PPT。主文件用于执行决策，参考只读当前任务需要的部分。

## Task scope

| 请求 | 范围 |
| --- | --- |
| 新建或整体重做 | 完整制作；讲演稿每页原生动画，包括封面、过渡和结束页 |
| 局部修改 | 只改指定对象与必要依赖，保留无关内容、格式和动画；新增页按用途制作，不补做全稿动画或重选风格 |
| 审阅、解释、诊断 | 报告位置、依据和建议；完整上下文已授权修复时执行修改 |
| 仅知识树、文案或素材 | 知识树用分支或嵌套列表展示主题、知识点与逐页任务。文案和素材按所求形式交付。用户只要提纲、样段或样页时止于该成果。静态、打印、纯阅读按其用途处理 |

混合请求分别处理。用户要求、已确认安排和保留项优先；不增加默认大纲、样稿或分批审批。制作中修正本次造成的问题属于制作范围。需要辨别边界时看 [示例](references/worked-examples.md#task-boundary-cases)。

## Core requirements

1. **先把整场讲顺，再逐页写。** 决策或验收汇报有了证据，就在第一张能讲实质内容的页面交代各选项怎么处理、适用于什么范围。存在未决项时点明待定之处。原理课或探索性报告可从真正的问题起讲。长稿先把各章连成一段话，听众应能从上一章得到的结果，听出下一章为何值得讲。详页再接住具体疑问或继续用前页的结果，结尾回到开场的任务。
2. **图文要讲到实际作用。** 有图的内容页沿着“图中看见什么、据此明白什么、这对当前问题有什么用”把意思讲透。选一处关键差异、部件关系或运算，带上必要参照，解释它为何支持这项判断，再说清哪个方案可选、哪段该查，或后一步拿这个结果做什么。方法图讲明操作改变了谁、解决了哪一步困难。三层意思写成自然的一段。用本次读数、条件或处置限定结论，删掉例行的“仍需验证”和泛谈价值的结尾。[图文改写示例](references/worked-examples.md#explain-what-a-figure-changes)
3. **页标题不超过七个字。** 自拟的上屏主标题和章名用简短、自然的词概括本页要点，如“分组验收结果”。完整结论写进可见正文首句，用具体对象、动作和证据把判断讲透。较长的正式题名如经用户指定须原样保留，依其原文。按[标题写法与计数](references/research-explanation.md#titles-and-cover-copy)逐题检查。讲者提醒和详细来源按[信息用途](references/research-explanation.md#audience-facing-qualifications-and-small-text)放置。
4. **沿用方向，按内容构图。** 保留既有模板或完整视觉方案；仅有风格方向且仍需模板时在该方向内选型，无指定时查看少量适配候选。明确原创或无合适模板时自主设计。保持稿内字体、配色和标注一致，关键类别不只靠颜色区分；不为版式删改必要含义。
5. **让听众在图中找到依据。** 先复用合适原件。按本页任务选数据图、机制图、设备图或概念插画，明确支持哪句话、读者应看哪一处。密集图按需采用直接标名、范围强调、同号说明或局部放大。提前确定来源真实性、许可、编辑粒度与运动图层，保留来源或生成提示词。
6. **保留原生编辑与逐页动画。** 文字、表格、图表数据、技术图组件及连接按约定粒度编辑；照片和背景可为图像。新建/重做讲演稿每页都有原生对象入场、强调或动作，简单页可一次协调入场。复杂图按解释表现路径、运动、放大或真实状态切换，标识与说明同步并保留上下文。整页转场不替代页内动画，标签淡入不替代机制运动；不以整页图片、视频或近似重建稿静默替代原生对象。
7. **看保存后的实际结果。** 连读开场、换章处与末页，回到关键判断指认图中依据。末页若交给别人排查，照它走一遍，核对记录能否区分仍然说得通的解释、不同结果分别该查哪里。[排查与复测](references/research-explanation.md#diagnostic-follow-up)给出写法。按[制作核对](references/implementation-and-checks.md#minimum-production-confirmation)核实文字与对象，改版式看渲染，改动画或交互看入场、中间和终态。区分实际查验、用户接管和能力受限，只复验受影响范围。

## Working with other skills

先按 [目的地与工具能力](references/implementation-and-checks.md#choose-the-working-surface) 确定路线：本次要求、用户默认和更高层约定优先，保留已有稿及目标应用；无这些约定时默认本地 PPTX。通用演示或服务 Skill 只执行所选路线适用环节，并遵守其 API、权限和必需导出检查。不能通过换工具静默降低模板保真、编辑性或动画要求。

## Choose task complexity

完整 PPT 制作（新建或整体重做）默认启用专门的 **A 内容子代理**：先确定整稿主线、每页要演示什么，再交完整上屏正文。主代理统筹，**C 制作子代理**依据 A 的内容稿完成 PPT；B 素材与 D 模板按实际需要加入，见 [协作与交接](references/collaboration.md)。局部修改、仅审阅或仅文案按本次范围处理，不自动补齐全套角色；子代理不可用时由主代理依次承担并说明。正式 PPTX 和脚本只有一个写入者，不新建用户聊天代替子代理。

## Complete the requested deck

局部修改从已有成果进入，其他制作按依赖推进：

1. **确定约束。** 区分指定模板、待改原稿与仅供取材的旧稿，沿用最新确认的范围、页数或时长、保留项及输出路径。要求模板保真时取得原件，及早核实导入、编辑和动态能力。
2. **组织章节和逐页正文。** 完整制作由 A 读原材料和图表，在现有页计划里先串起各页的意思，再把关键观察、推理及用途写成上屏正文；图表明细按需取用。已认可的样段用来校准讲解深度和语气。学术原理讲解或跨页导读见[方法专题](references/method-talks.md)，读数、判断与中文段落见[讲解与文案](references/research-explanation.md#figure-and-adjacent-explanation)。改稿先诊断[知识、关系或显示问题](references/research-explanation.md#diagnose-the-explanation-gap)，再选[版式](references/layout-and-style.md#choose-a-layout-from-the-relationship)。
3. **配图并制作。** 按正文需要取得原件，素材揭示新事实或限制时据此修订正文；先为必要解释安排空间，再确定配图、分层和讲述顺序中的动态，简单分镜一句话即可。复用合适模板页、原生对象和现有实现，按真实字体与尺寸制作，先调组织和空间再考虑缩字号。
4. **保存、检查、交付。** 执行第 7 条，提供一个权威最新版、直接可用入口、实际验证和影响使用的限制。某页受阻时继续其他独立工作，不静默改变交付要求。

## Read references as needed

| 当前需要 | 入口 |
| --- | --- |
| 逐页知识树、学术原理专题、导读与详页 | [按场景安排知识树](references/research-explanation.md#choose-the-explanation-from-the-scene)／[方法专题与示例](references/method-talks.md) |
| 内容深度、研究论证、标题与标签位置 | [讲解与文案](references/research-explanation.md) |
| 模板选型／构图与稿内一致性 | [模板](references/template-selection.md)／[版式与参数](references/layout-and-style.md) |
| 素材复用、检索、绘制或生成 | [素材路径](references/asset-sources.md#choose-reuse-search-drawing-or-generation)；有来源缺口再查 [目录](references/source-catalog.md) |
| 对象、字体、图表、动画与验证 | [制作与核对](references/implementation-and-checks.md)，复杂效果查 [效果选择](references/implementation-and-checks.md#choose-the-effect-from-the-explanation) |
| 需要具体示范 | [制作案例](references/worked-examples.md)／[研究改稿](references/research-and-revision-examples.md)／[可视案例](references/visual-cases.md)；事实用本次来源，不照搬数字与布局 |
| 修改 Skill 或明确要求前后比较 | [修订验证](references/paired-evaluation.md)，不加入普通 PPT 制作流程 |
