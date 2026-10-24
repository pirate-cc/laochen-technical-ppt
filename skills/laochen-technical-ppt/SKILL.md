---
name: laochen-technical-ppt
description: "Create, revise, or review Chinese technical, teaching, research, or project-report PowerPoint decks. Use natural ready-to-use copy and subject-matched visuals, preserve template style and editable objects, and implement native animation on every slide of a new or substantially remade live-talk deck."
---

# 老陈技术汇报 PPT

依据已有材料把主体讲清楚，沿用用户模板，交付文字可直接使用、视觉贴合主题的可编辑 PPT。讲演稿默认逐页有原生动态，完成制作后直接交给用户自行检查。

## Task scope

按完整请求判断本次动作，混合请求分别处理：

- **新建或整体重做：** 执行完整制作流程，讲演稿落实逐页动态。
- **局部修改：** 只处理指定页面、对象及其必要依赖，沿用已确认的内容、素材与版式；不因全稿默认要求而重写其他页、补齐全稿动画或重启素材选型。新增页面按其用途制作，已有无关效果保留。
- **审阅、解释或诊断：** 只检查和报告发现、依据与建议。完整上下文中已授权修复时，才执行相应修改；制作过程中纠正本次造成的问题属于已授权制作。
- **仅文案、提纲或素材：** 交付请求的内容或资产，不顺带制作 PPTX。静态、打印或纯阅读请求按该用途处理。

参考 [任务边界示例](references/worked-examples.md#task-boundary-cases) 判断局部与混合请求。

## Core requirements

- **内容有实质。** 每页解释一个完整意思：概念的关系、方法的关键操作、系统的组成与协作，或图中可见的特征和变化。先确定听众与讲解顺序，再分配各页内容、选择主视觉和动态、最后排版实现；不按文件或模板占位顺序机械展开。
- **介绍与评价分开。** 结构、机制、界面或文献介绍讲清现有材料即可结束；材料未涉及的实验、数据或验证，不自动变成正文、页脚或备注中的缺陷声明。实际结果的状态、不确定性和比较条件仍须保留。
- **证据状态准确。** 候选、示意、教学算例、设计、仿真和实测分别命名；项目截图、波形、数字与结论来自可定位的真实来源。历史例子不代表新运行，生图不补实验依据。必要标签、单位、变量与条件随解释对象可见。
- **文案自然、可直接使用。** 封面先交代人物、作品或主题，页标题直接命名对象、操作或有依据的结论。正文用适合听众的专业中文说明具体对象、做法和关系，保留必要术语并解释其含义；避免抽象名词堆叠、生硬搭配和刻意文艺化的概括。写作时连同相邻页通读并改稿，不让用户再把提纲加工成正文，也不依靠备注补救含糊的可见文字。详细标准见 [中文成稿](references/research-explanation.md#natural-chinese-technical-copy)。
- **模板统一、布局服从内容。** 保留模板字体、配色、母版、固定元素与标注风格，构图随内容变化；关键类别用颜色之外的线索辅助区分，文字、线条与标注在背景上可辨。不为凑字数、对仗或卡片数量删改含义。泛化提醒、重复总结和讲述顺序移入备注或删除，必要图旁说明和署名保留。
- **保留所需可编辑性。** 文字、表格、图表数据和技术图的组件、标签、连接保持约定的原生编辑粒度；背景照片或插画可以是图像。局部修改保留无关内容、格式和动画，不用整页图片、视频或重建近似稿静默替代要求的原生对象。
- **主动选择主题素材。** 先读模板、本地资料与既有示例，再按用途复用、搜索、原生绘制或直接生图。素材同时满足解释任务与主题所需的视觉质量；替换粗糙示意图时保留原有的空间、流程或证据关系，按需用实景、可靠底图或精细插画配原生标注。检索查看原页面/原图和许可；栅格创作使用可用的 imagegen Skill 与内置工具。素材及所需图层保存在项目内，保留来源、署名或生成提示词；选够即停。
- **讲演版默认逐页有原生动态。** 在上述制作范围内，封面、过渡页、简单结论和结束页同样安排适度的对象入场或强调；内容页围绕实际讲解对象展开，复杂图让标识、连接和说明同步出现，需要时表现路径、运动、局部放大或真实状态切换。简单页可用一次协调入场，点击次数由内容决定；普通整页转场不替代页内动态，标签淡入不替代机制运动。
- **做完直接交付用户自行检查。** 完成文案、图文对应、实际动画写入和 [最小制作核对](references/implementation-and-checks.md#minimum-production-confirmation)，处理本次制作与导出错误后交付。不增加大纲、样稿或分批审批；成稿渲染、截图、重开编辑试验、播放、无障碍审计、排练与回归仅在用户明确要求对应检查时执行。不声称未执行的检查通过，不例行列出省略项。

## Working with other skills

本 Skill 负责讲解、文案、主题视觉、动态及用户约定的交付方式；通用 Presentations 等基础 Skill 提供所选工具的接口、格式处理和必需导出检查。联用时按本次用户要求确定范围，不把其他流程的默认成稿渲染或审阅轮次自动加入任务，也不把这里的直接交付理解为跳过必要文件检查。用户明确要求优先；本 Skill 不覆盖更高层指令或工具权限。

选工具时确认原模板导入、原对象编辑、所需图表与动画的实际支持，按 [工作界面与工具选择](references/implementation-and-checks.md#choose-the-working-surface) 继续；不能靠更换工具或重建近似稿静默降低约定的可编辑性。

## Choose task complexity

常规任务由主代理完成；有独立工作量时，从 A 内容与证据、B 视觉与素材、C 制作与动态中选择必要的一个、两个或三个专项。按真实工作量选择，不以固定页数或“完整制作”字样触发全部代理。

启用协作时读取 [协作与交接](references/collaboration.md)，明确角色、输入、输出及写入范围。启用 C 时由 C 独占权威 PPTX 及制作脚本，否则由主代理写；A/B 不另做分支 PPTX。使用子代理工具而非新建用户聊天；并发不足时顺序执行或由主代理接回职责。各角色只读所需参考，沿用本次任务与检查边界。

## Complete the requested deck

仅制作或修改任务执行相应步骤；局部修改从已有成果和受影响对象进入，不重跑全套规划。

1. **读取需求、已有成果与模板。** 确定本次范围、听众、用途、页数或时长、来源、保留项、目标应用与权威输出路径。能从现有材料判断的直接判断；仅澄清无法解决且影响目标的缺口。用户要求模板保真但无可用模板时，先取得模板再制作最终稿。
2. **安排讲解并写成稿。** 让定义、整体或输入先于依赖它的细节与输出，按实际方法顺序解释；把自然、具体的可见文案、来源和主图目标对应到页面，并连贯通读修改。科研链可参考“原始记录 → 观察现象 → 处理需求 → 方法选择 → 输出解释 → 总结”，这是依赖关系，不是固定六页；单页介绍也不必附结果或计划。
3. **选择视觉与逐页分镜。** 按 [主题构图](references/asset-sources.md#subject-led-visual-design)、[图像替换标准](references/asset-sources.md#visual-quality-and-image-replacement) 与 [素材路线](references/asset-sources.md#choose-reuse-search-drawing-or-generation) 确定主视觉。讲演版逐页说明入场、对象动作与保留上下文；简单页一句话即可，静态用途在全局要求中注明。A/B 可准备独立材料，依赖已明确的页即可交 C 制作。
4. **在原工具中制作。** 复用合适模板页及原生对象，按真实字体和尺寸安排正文、坐标与标注，解决拥挤后再考虑缩字号。按 [原生动态规则](references/implementation-and-checks.md#progressive-explanation-and-animation) 和 [效果选择](references/implementation-and-checks.md#choose-the-effect-from-the-explanation) 实现分镜，保留约定页数。工具限制只暂停受影响部分；保留可用成果并说明具体限制，不静默更换交付形式。
5. **保存并交付。** 按本次范围完成最小制作核对，提供一个权威最新版及直接可用路径，简述实际完成内容与影响使用的问题。审阅请求另按 [检查边界](references/implementation-and-checks.md#when-to-use-checks) 报告，区分结构核对、实际播放和排练。

按本页任务选用 [机制运动](references/worked-examples.md#mechanism-motion-with-editable-objects)、[真实波形对比](references/worked-examples.md#matched-waveform-comparison)、[场景与采集链路](references/worked-examples.md#monitoring-scene-and-acquisition-flow)、[完整单页改写](references/worked-examples.md#complete-one-slide-rewrite) 或 [园林教学页](references/worked-examples.md#garden-teaching-page) 等相关示例。示例中的历史数字、配色、页数和点击数只属于其语境；不默认通读全部参考，也不把示例升级为通用模板。
