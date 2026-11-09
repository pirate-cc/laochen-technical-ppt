---
name: laochen-technical-ppt
description: "Create, revise, or review Chinese PowerPoint decks for technical reports, teaching, product introductions, training, cultural topics, and other presentation scenes. Choose sources and visuals for the actual audience and purpose; preserve natural copy, editable objects, and native animation on every slide of a new or wholly remade live-talk deck."
---

# 老陈技术汇报 PPT

根据题材、听众和用途选择讲解、素材与动态，把主体讲清楚。沿用已有模板；没有模板时按场景建立一致的视觉语言。交付文字可直接使用的可编辑 PPT，讲演稿默认逐页有原生动态，完成与本次用途和修改范围相称的检查后直接交付。

## Task scope

按完整请求判断本次动作，混合请求分别处理：

- **新建或整体重做：** 执行完整制作流程，讲演稿落实逐页动态。
- **局部修改：** 只处理指定页面、对象及其必要依赖，沿用已确认的内容、素材与版式；不因全稿默认要求而重写其他页、补齐全稿动画或重启素材选型。新增页面按其用途制作，已有无关效果保留。
- **审阅、解释或诊断：** 只检查和报告发现、依据与建议。完整上下文中已授权修复时，才执行相应修改；制作过程中纠正本次造成的问题属于已授权制作。
- **仅文案、提纲或素材：** 交付请求的内容或资产，不顺带制作 PPTX。静态、打印或纯阅读请求按该用途处理。

参考 [任务边界示例](references/worked-examples.md#task-boundary-cases) 判断局部与混合请求。

## Core requirements

- **按场景讲清内容。** 从请求和资料判断题材、听众、希望观众理解或完成什么，以及讲演或阅读用途；这些信息用于内部决策，不形成固定问卷。每页传达一个完整意思，按本次需要解释对象、操作、关系、变化、叙事或选择依据。先确定讲解目标和依赖，再分配内容；素材与文案可相互修订，不按文件、模板占位或某个行业案例机械展开。见 [讲解选择](references/research-explanation.md#choose-the-explanation-from-the-scene)。
- **介绍与评价分开。** 结构、机制、界面或文献介绍讲清现有材料即可结束；材料未涉及的实验、数据或验证，不自动变成正文、页脚或备注中的缺陷声明。实际结果的状态、不确定性和比较条件仍须保留。
- **证据状态准确。** 候选、示意、教学算例、设计、仿真和实测分别命名；项目截图、波形、数字与结论来自可定位的真实来源。历史例子不代表新运行，生图不补实验依据。必要标签、单位、变量与条件随解释对象可见。
- **文案自然、可直接使用。** 封面先交代人物、作品或主题，页标题直接命名对象、操作或有依据的结论。正文用适合听众的专业中文说明具体对象、做法和关系，保留必要术语并解释其含义；避免抽象名词堆叠、生硬搭配和刻意文艺化的概括。写作时连同相邻页通读并改稿，不让用户再把提纲加工成正文，也不依靠备注补救含糊的可见文字。详细标准见 [中文成稿](references/research-explanation.md#natural-chinese-technical-copy)。
- **视觉统一、布局服从内容。** 有模板时保留字体、配色、母版、固定元素与标注风格；无模板时按 [视觉方向](references/implementation-and-checks.md#working-without-a-template) 建立一致规范。构图随内容变化，关键类别用颜色之外的线索辅助区分，文字、线条与标注在背景上可辨。不为凑字数、对仗或卡片数量删改含义。泛化提醒、重复总结和讲述顺序移入备注或删除，必要图旁说明和署名保留。
- **保留所需可编辑性。** 文字、表格、图表数据和技术图的组件、标签、连接保持约定的原生编辑粒度；背景照片或插画可以是图像。局部修改保留无关内容、格式和动画，不用整页图片、视频或重建近似稿静默替代要求的原生对象。
- **根据场景寻找和复用素材。** 先明确本页对象或关系、真实性、编辑粒度与动态所需图层。用户提供或项目已有的合适材料直接复用；需要新增素材时，以网站检索为主，按当前题材寻找原作者、资料持有者和适当素材网站，不局限于示例名单。已连接素材库按需补充；需要原生关系图或真实数据图时直接绘制，生图用于适合的定制插画。素材的内容、构图和质量须支持本页解释，替换时保留必要关系。按 [场景选材](references/asset-sources.md#scene-to-material)、[已有材料复用](references/asset-sources.md#reuse-local-and-connected-material) 与 [来源发现](references/asset-sources.md#choose-sources-by-purpose) 执行，记录来源或生成提示词，选够即停。
- **讲演版默认逐页有原生动态。** 在上述制作范围内，封面、过渡页、简单结论和结束页同样安排适度的对象入场或强调；内容页围绕实际讲解对象展开，复杂图让标识、连接和说明同步出现，需要时表现路径、运动、局部放大或真实状态切换。简单页可用一次协调入场，点击次数由内容决定；普通整页转场不替代页内动态，标签淡入不替代机制运动。
- **完成必要检查后交付。** 完成文案、图文对应、实际对象与动画写入及 [最小制作核对](references/implementation-and-checks.md#minimum-production-confirmation)。新增或修改版式后查看受影响页面的实际渲染；新增或修改动画、交互或播放顺序后，在支持相应效果的实际环境中核对受影响内容。局部修改不扩大为全稿重做或无关回归。完整排练、无障碍专项审计等额外检查按任务需要执行。不增加默认大纲、样稿或分批审批；用户明确保留的审批或检查安排照常执行。必要效果核验受阻时，说明具体受影响内容和实际检查层级，交付可用部分，不把结构正确表述为效果已验证。

## Working with other skills

本 Skill 负责场景判断、讲解、文案、主题视觉、动态及用户约定的交付方式。先按 [工作界面与工具选择](references/implementation-and-checks.md#choose-the-working-surface) 确定输出目标、模板状态和所需能力，再把这些已确定的约束传给 Presentations 或相应服务 Skill。基础 Skill 提供所选工具的接口、格式处理和必需导出检查；其未指定目标时的默认分支不重新决定已经明确的交付形式。联用按受影响范围完成必要文件、渲染和动态效果检查，不重复已完成的检查或增加无关审阅轮次。用户明确要求优先；本 Skill 不覆盖更高层指令或工具权限。

选工具时确认原模板导入、原对象编辑、所需图表与动画的实际支持，按 [工作界面与工具选择](references/implementation-and-checks.md#choose-the-working-surface) 继续；不能靠更换工具或重建近似稿静默降低约定的可编辑性。

## Choose task complexity

常规任务由主代理完成；有独立工作量时，从 A 内容与证据、B 视觉与素材、C 制作与动态中选择必要的一个、两个或三个专项。按真实工作量选择，不以固定页数或“完整制作”字样触发全部代理。

启用协作时读取 [协作与交接](references/collaboration.md)，明确角色、输入、输出及写入范围。启用 C 时由 C 独占权威 PPTX 及制作脚本，否则由主代理写；A/B 不另做分支 PPTX。使用子代理工具而非新建用户聊天；并发不足时顺序执行或由主代理接回职责。各角色只读所需参考，沿用本次任务与检查边界。

## Complete the requested deck

仅制作或修改任务执行相应步骤；局部修改从已有成果和受影响对象进入，不重跑全套规划。

1. **读取需求、已有成果与模板。** 判断本次场景与范围，确定页数或时长、来源、保留项、输出目的地和权威路径，尽早确认模板、图表与动画能力。能从现有材料判断的直接判断；仅澄清无法解决且影响目标的缺口。用户要求模板保真但无可用模板时，先取得模板再制作最终稿。
2. **安排讲解并形成初稿。** 从观众目标和内容依赖决定顺序，写出本页要解释的具体对象或关系、文案初稿和来源；按需选择解释、操作、比较、叙事或决策方式，不套固定行业大纲。同步判断主视觉、需要独立编辑或运动的对象，以及素材缺口。
3. **取得素材并共同定稿。** 复用合适现有材料，需要新增素材时主要从适合当前场景的网站寻找并查看原件，按需补充其他途径。依据实际可见内容与来源修订文案、构图和逐页分镜；必要时换素材或调整受影响的解释，见 [图文往返调整](references/research-explanation.md#copy-and-asset-iteration)。讲演版逐页说明入场、对象动作与保留上下文，优先按 [信息关系选择效果](references/implementation-and-checks.md#choose-the-effect-from-the-explanation)；简单页一句话即可。按依赖推进已明确的页面，不为一页缺图暂停其他页。
4. **在原工具中制作。** 复用合适模板页及原生对象，按真实字体和尺寸安排正文、坐标与标注，解决拥挤后再考虑缩字号。按 [原生动态规则](references/implementation-and-checks.md#progressive-explanation-and-animation) 和 [效果选择](references/implementation-and-checks.md#choose-the-effect-from-the-explanation) 实现分镜，保留约定页数。工具限制只暂停受影响部分；保留可用成果并说明具体限制，不静默更换交付形式。
5. **保存并交付。** 按本次范围完成最小制作核对及必要效果检查，提供一个权威最新版及直接可用路径，简述实际改动、已完成的验证与影响使用的问题。审阅请求另按 [检查边界](references/implementation-and-checks.md#when-to-use-checks) 报告，区分结构核对、实际播放和排练。

素材网站可按 [适用场景、格式与使用条件](references/asset-sources.md#additional-asset-libraries) 选读，仅调用本页需要的入口。

仅在需要具体示范时读取 [产品与结构动作](references/worked-examples.md#product-introduction-with-editable-motion)、[操作培训](references/worked-examples.md#procedure-training-with-native-interface-states)、[数据比较](references/worked-examples.md#comparison-with-supplied-data) 或 [方法讲解](references/worked-examples.md#complete-one-slide-rewrite)。示例均标明教学设定，按关系迁移其做法，使用本次来源重新确定事实、视觉与分镜。Skill 自身有实质修订时可按 [跨场景验证](references/worked-examples.md#skill-revision-checks) 检验行为；这不增加每份 PPT 的审阅步骤。
