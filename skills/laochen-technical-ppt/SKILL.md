---
name: laochen-technical-ppt
description: "Create, revise, or review Chinese PowerPoint decks for technical reports, teaching, product introductions, training, cultural topics, and other presentation scenes. Develop substantive explanations with natural copy, scene-appropriate visuals, editable objects, and native animation on every slide of a new or wholly remade live-talk deck."
---

# 老陈技术汇报 PPT

按听众、用途和本次材料把主题讲清楚，交付文案可直接使用的可编辑 PPT。主文件用于执行决策，参考只读当前任务需要的部分。

## Task scope

| 请求 | 范围 |
| --- | --- |
| 新建或整体重做 | 完整制作；讲演稿每页原生动画，包括封面、过渡和结束页 |
| 局部修改 | 只改指定对象与必要依赖，保留无关内容、格式和动画；新增页按用途制作，不补做全稿动画或重选风格 |
| 审阅、解释、诊断 | 报告位置、依据和建议；完整上下文已授权修复时执行修改 |
| 仅文案、提纲或素材 | 只交付所求内容，不顺带做 PPTX；静态、打印、纯阅读按其用途处理 |

混合请求分别处理。用户要求、已确认安排和保留项优先；不增加默认大纲、样稿或分批审批。制作中修正本次造成的问题属于制作范围。需要辨别边界时看 [示例](references/worked-examples.md#task-boundary-cases)。

## Core requirements

1. **内容充分。** 按观众目标和理解依赖组织，每页完成明确任务；相关模型、步骤和证据可以同页。保留必要定义、关系、操作、公式、条件和判断依据，不用标签、留白或动画代替知识，不以字数或卡片数判定完成。
2. **事实准确。** 来源可定位，区分示例、设计、仿真与实测，不拿历史案例或生图冒充新运行。变量、单位和必要条件随对象可见。介绍材料未涉及的验证不自动变成缺陷声明；实际影响结果判断的状态和不确定性照实交代。
3. **文字自然。** 介绍、解释、方法比较及归纳页默认具体主题；操作页写实际动作，结果页可写有据发现。标题不写口号、讲者提醒或正文摘要，正文不是待用户扩写的提纲。听众定位和制作背景留在内部，不加“教学构造数据”等防御性小字或例行灰色副标题；删掉后不移位、放大或改名保留。输入、单位和示例身份就近自然表达，只有必要的整页限定才用可读副标题。通读相邻页，核对表达和证据，见 [文案规则](references/research-explanation.md#writing-from-sources)。
4. **沿用方向，按内容构图。** 保留既有模板或完整视觉方案；仅有风格方向且仍需模板时在该方向内选型，无指定时查看少量适配候选。明确原创或无合适模板时自主设计。保持稿内字体、配色和标注一致，关键类别不只靠颜色区分；不为版式删改必要含义。
5. **按需取材。** 先复用合适已有材料；关系图、真实数据图可直接原生绘制；真实照片和原图查来源；概念插画按需生成。提前确定真实性、编辑粒度和运动图层，查看原件、核对许可、保留来源或提示词；图文相互修订，够用即停。
6. **保留原生编辑与逐页动画。** 文字、表格、图表数据、技术图组件及连接按约定粒度编辑；照片和背景可为图像。新建/重做讲演稿每页都有原生对象入场、强调或动作，简单页可一次协调入场。复杂图按解释表现路径、运动、放大或真实状态切换，标识与说明同步并保留上下文。整页转场不替代页内动画，标签淡入不替代机制运动；不以整页图片、视频或近似重建稿静默替代原生对象。
7. **看保存后的实际结果。** 按 [制作核对](references/implementation-and-checks.md#minimum-production-confirmation) 检查内容、标题及下一行、对象和图文对应；改版式看实际渲染，改动画/交互检查相关入场、中间和终态。明确区分已检查、用户明确接管、能力受限；XML 或脚本成功不能称为效果通过。只复验受影响范围。

## Working with other skills

先按 [目的地与工具能力](references/implementation-and-checks.md#choose-the-working-surface) 确定路线：本次要求、用户默认和更高层约定优先，保留已有稿及目标应用；无这些约定时默认本地 PPTX。通用演示或服务 Skill 只执行所选路线适用环节，并遵守其 API、权限和必需导出检查。不能通过换工具静默降低模板保真、编辑性或动画要求。

## Choose task complexity

常规任务直接做；有独立工作量才分工并读 [协作与交接](references/collaboration.md)。正式 PPTX 和脚本只有一个写入者，交接前保存并停止写入；不按固定页数启动全部角色，不新建用户聊天代替子代理。

## Complete the requested deck

局部修改从已有成果进入，其他制作按依赖推进：

1. **确定约束。** 读请求、原材料和已有稿，确定用途、页数/时长、保留项、模板与输出路径；尽早核实导入、编辑和动态能力。要求模板保真时先取得原件，仅澄清无法自行解决的关键缺口。
2. **写清内容。** 安排讲解顺序，形成可上屏文案与来源定位；改稿先辨别 [知识、关系或显示问题](references/research-explanation.md#diagnose-the-explanation-gap)，再选 [版式](references/layout-and-style.md#choose-a-layout-from-the-relationship)。
3. **图文定稿并制作。** 按素材路径取得原件，结合实际内容调整构图、分层及动态；简单分镜一句话即可。复用合适模板页、原生对象和现有实现，按真实字体与尺寸制作，先调组织和空间再考虑缩字号。
4. **保存、检查、交付。** 执行第 7 条，提供一个权威最新版、直接可用入口、实际验证和影响使用的限制。某页受阻时继续其他独立工作，不静默改变交付要求。

## Read references as needed

| 当前需要 | 入口 |
| --- | --- |
| 内容深度、研究论证、标题与标签位置 | [讲解与文案](references/research-explanation.md) |
| 模板选型／构图与稿内一致性 | [模板](references/template-selection.md)／[版式与参数](references/layout-and-style.md) |
| 素材复用、检索、绘制或生成 | [素材路径](references/asset-sources.md#choose-reuse-search-drawing-or-generation)；有来源缺口再查 [目录](references/source-catalog.md) |
| 对象、字体、图表、动画与验证 | [制作与核对](references/implementation-and-checks.md)，复杂效果查 [效果选择](references/implementation-and-checks.md#choose-the-effect-from-the-explanation) |
| 需要具体示范 | [制作案例](references/worked-examples.md)／[研究改稿](references/research-and-revision-examples.md)／[可视案例](references/visual-cases.md)；事实用本次来源，不照搬数字与布局 |
| 修改 Skill 或明确要求前后比较 | [修订验证](references/paired-evaluation.md)，不加入普通 PPT 制作流程 |
