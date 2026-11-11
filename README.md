# 老陈技术汇报 PPT

面向中文技术汇报、教学、产品介绍、操作培训、文化叙事等场景的 Codex Skill。以完整正文为主体，先讲清事实、做法、关系与判断，再用图支撑说明；沿用指定模板，新稿按场景选型或自主设计，交付文案自然、讲解充分、保留原生编辑能力与逐页原生动态的 PowerPoint。

**当前版本：0.1.27 · 作者：老陈 · [MIT License](LICENSE)**

English: A reusable Chinese presentation skill for Codex, with complete body copy supported by figures, scene-based template selection and sourcing, natural copy, template preservation or coherent original design, editable objects, and native slide animation.

## 能做什么

- **新建或整体重做：** 从场景和观众目标安排讲解，读透原材料后先写完整正文，再配图支持并安排原生动态；讲演稿默认每页都有服务内容的对象动画。
- **局部修改：** 只修改指定页面、对象及必要依赖，保留无关内容、格式与动画。
- **审阅、解释或诊断：** 默认只检查和报告；用户明确授权后才修改文件。
- **文案、提纲或素材：** 只交付所需内容；静态、打印或阅读稿按相应用途处理。

完整规则见 [SKILL.md](skills/laochen-technical-ppt/SKILL.md)，具体写法与协作示例见 [worked-examples.md](skills/laochen-technical-ppt/references/worked-examples.md)。

## 0.1.27 正文为主体，图辅佐文字

- 核心规则和制作顺序明确先定演示内容、形成完整上屏正文，再按正文需要配图；图片识别、图例和部件标签不能替代正文。
- 区分正文与图注：实验页讲实际做法及条件，结果页讲观察、比较依据与判断；材料支持的计算和解释可充分展开，保留事实与推断的边界。
- 版式支持连贯段落、完整步骤、结果分析配证据图表及纯文字页；模板选型检查必要正文是否有可读空间，不用图文面积配额决定质量。
- 完整制作默认由专门 A 内容子代理决定整稿主线、每页要演示什么并写出完整正文，C 制作子代理据此制作；B 提供支持材料、D 选模板，按实际需要加入。A 回看成稿，主代理统一整合；局部修改不自动扩成全流程，不新增用户审批。
- 正文优先讲实际做法、原理、观察与判断；计划写具体行动，结果直接说明指标和差距，减少反复“尚未”“不代表”等防御性清单，必要条件仍就近说明。
- 制作检查先读保存后的正文，再核对配图如何支持；同步修订 [连续研究示例](skills/laochen-technical-ppt/references/research-and-revision-examples.md#research-argument-across-four-slides) 及 [修订验证](skills/laochen-technical-ppt/references/paired-evaluation.md)。
- 增加 [正文先行的四页完整案例](skills/laochen-technical-ppt/references/visual-cases.md#body-copy-and-production-handoff)，保留原始材料、A 的内容稿、C 制作的可编辑 PPTX 和检查记录，供核对正文如何进入最终页面。
- 原生可编辑、讲演版逐页原生动画、自然标题、局部修改边界和按影响范围复验的要求继续保留。

## 0.1.26 规则精简与案例修正

- 主文件集中任务范围、有效底线和按需入口；合并内容深度、素材选择、检查例外与协作重复，保留原生编辑和讲演版逐页原生动态。
- 介绍与方法比较默认具体主题标题；必要身份、输入、单位和条件就近表达，避免例行灰色副标题，同时保留有依据的发现标题。
- 将网站条目集中到 [来源目录](skills/laochen-technical-ppt/references/source-catalog.md)，仅在素材缺口需要时读取；保留所有原有入口与特有许可说明。
- 保留历史对比稿，新增 [修正版可编辑案例](skills/laochen-technical-ppt/references/visual-cases.md#current-corrected-examples)，修正文案与小字并检查实际渲染和 PowerPoint 动画视频；准确记录检查范围。
- 修订验证按行为与实际成果判断，不要求旧段落逐字不变；区分首次完成稿问题和修复后质量，避免只追加规则。

## 0.1.25 内容驱动版式与同输入出片比较

- 增加 [版式选择与稿内参数](skills/laochen-technical-ppt/references/layout-and-style.md)：从比较、路径、整体局部、公式和数据关系选构图，按实际拥挤原因调整，复用本稿字体层级、间距、颜色含义和标注样式。
- 增加 [可视改稿案例](skills/laochen-technical-ppt/references/visual-cases.md)，保留合成教学材料、可编辑 PPTX 和真实渲染；案例说明取舍，不能当作普遍改善证明或固定模板。
- 增加 [同输入出片验证](skills/laochen-technical-ppt/references/paired-evaluation.md)：冻结旧版和输入，独立制作、实际渲染与相关播放检查，记录改善、退步及适用范围；公开案例后续作为教学/回归材料。
- 原有内容深度、中文表达、模板保留、可编辑性、局部修改边界和逐页原生动态要求保持不变；不新增默认审批或普通制作任务的跨场景测试。

## 0.1.24 自然具体的页面标题

- 按页面实际内容选择主题短语、操作、问题或有据发现，技术介绍可直接命名具体对象与方面；避免将讲者提醒、口号和整段解释压成标题。
- 增加 [标题判断](skills/laochen-technical-ppt/references/research-explanation.md#titles-and-cover-copy) 与 [改写案例](skills/laochen-technical-ppt/references/worked-examples.md#titles-from-page-content)，区分真实操作顺序与空泛句框，不机械禁词或统一全部句式。
- 整理章节标签、页标题和图题的作用；在授权范围内减少重复，用户指定标题和局部修改范围继续保留。
- 同步修订较长的内置示例标题，将具体步骤、数据解释和条件保留在正文；内容深度、模板选型、可编辑性与逐页原生动态要求不变。

## 0.1.23 比较论证、具体改稿与模板选型

- 比较模型时辨明输出对象、输入与适用条件，区分可比较的结构与有数据支持的性能；贡献表达区分新增能力与实际收益。
- 将结果型结论追到对应对象、工况、指标和证据，区分方法表现与研究问题的回答，保留部分达成和不确定性的实际含义。
- 改稿先判断知识缺口、关系混杂或显示问题；用具体例子说明如何删重复、补必要条件，以及整理平台、流程、配置和日志。
- 新增 [研究论证与改稿案例](skills/laochen-technical-ppt/references/research-and-revision-examples.md)：不同输出模型的一页比较、四页连续教学研究、复杂结果页分镜及按用途改写技术页。案例设定完整，原生对象与动态按讲解安排。
- 新增 [模板选型参考](skills/laochen-technical-ppt/references/template-selection.md)，纳入 Slidesgo、SlidesCarnival、iSlide、优品 PPT、SlideModel 和 PresentationGO，区分成套模板与组件，检查代表内容页、可用格式和实际使用条件。新稿按场景选择，已有模板和局部修改沿用确认方向。
- 增加可选 D 模板选型专项，主代理统一选型与交接；D 可与 A 并行，完成后释放名额再推进 B/C，四种角色不要求同时运行。C 或主代理保持唯一权威 PPTX 写入权。
- 沿用可编辑性、逐页原生动态、局部修改及必要效果核验；问答准备按场景需要执行，不新增默认审批、页数或固定检查表。

## 0.1.22 内容充分性与深入讲解

- 将单页任务明确为一个需要完成的解释或论述，允许相关模型、公式、图表和证据同页组织；按实际做法、差异或判断依据检查内容，不以少字、卡片数或留白比例判断质量。
- 修正介绍任务中过度限制已有结果与验证的表述，补入研究问题、方法、证据和结论的对应，以及研究现状归纳、实验/理论/仿真细节选择。
- 明确多面板也可以构成一个主要结构，保留有用的技术解释、变量和文献归属；增加独立教学设定的多模型比较与实验平台页改写案例。
- 将内容充分性并入原有制作核对和协作交接，检查必要知识在最终页面中仍然可见；补充数学符号语义、仿真结果图和问答材料的条件处理。
- 保留可编辑性、讲演版逐页原生动态、模板与局部修改边界，以及必要渲染和播放检查；不新增固定字数、公式数量或审批步骤。

本版的行为验证可分别检查文案、图文安排和分镜；这些检查不替代实际 PPT 的渲染、原生对象编辑和播放验证。

## 0.1.21 按设计问题选择参考

- 在 [参考选择表](skills/laochen-technical-ppt/references/asset-sources.md#content-methods-and-complete-talk-examples) 中补入 Deck.gallery、Data Viz Project、Information is Beautiful Awards 和 Motionimo，分别用于整套版式、图形选型、信息叙事与动态分镜；Curated.design 和 Page Flows 作为视觉与软件培训的按需补充。
- 扩充现有参考转化方法：查看相关页及相邻页面、区分讲演与阅读用途、按本次信息关系选图、把长网页或交互作品转成页面，并明确运动对象的起止状态和固定参照。
- 保留主规则和已有来源，复用现有可编辑性、原生动态与效果检查要求；材料足够即停止检索，访问受限时使用合适的可访问来源，不新增默认审批、付费或安装要求。

## 0.1.20 设计参考与转化

- 加入 [Recent](https://recent.design/) 作为构图、配色、图片处理与动态的参考入口，按当前视觉问题选读作品。
- 补充 [参考转化方法](skills/laochen-technical-ppt/references/asset-sources.md#adapt-design-references)：提取视觉规律，适配中文与演示场景，制作所需原生对象，并入现有渲染和动态效果检查。
- 保留模板、局部修改、内容证据、可编辑性与动态规则；不新增默认选型或审批环节，不打包第三方作品。

## 0.1.19 按修改范围核验效果

- 新增或修改版式后查看受影响页面的实际渲染；新增或修改动画、交互或播放顺序后核对实际效果。
- 局部修改不扩大为全稿回归，完整排练与无障碍专项按任务需要执行，不增加默认审批节点。
- 必要效果检查受阻时报告具体限制与实际检查层级，保留可用成果，不以对象写入代替效果验证。

## 0.1.18 素材网站索引

- 新增 SVG Repo、Storyset、PresentationGO、LottieFiles、NASA SVS、Smithsonian Open Access、Our World in Data 和 Poly Haven 八个入口，按适用场景、素材格式与使用条件整理。
- 从矢量对象、场景插画、PPT 组件、动态参考、科学可视化、馆藏实物、公共数据和三维素材中按需选择；保留已有来源和复用途径，网站名单不限制继续发现合适原件。
- 明确署名、条目许可、公开再分发和账户条件，区分矢量/三维源文件、媒体动画与 PPT 原生对象，不把下载格式视为可编辑性或动画实现的保证。

具体入口见 [素材网站索引](skills/laochen-technical-ppt/references/asset-sources.md#additional-asset-libraries)。本版沿用按场景选材、图文共同修订和无模板时建立一致视觉方向的流程，保留自然中文成稿、讲演版逐页原生动态、原生可编辑要求，以及按本次用途和修改范围完成必要制作核对后直接交付的方式。Skill 只提供链接和使用方法，不打包第三方素材。

## 安装到 Codex

### 方式一：让 Skill Installer 安装

在支持 `$skill-installer` 的 Codex 中发送下面这段话：

```text
使用 $skill-installer 安装这个 GitHub Skill：
https://github.com/pirate-cc/laochen-technical-ppt/tree/main/skills/laochen-technical-ppt
请保留整个 Skill 目录，包括 agents 和 references。
```

安装后，在下一轮对话选择或调用 `$laochen-technical-ppt`；如果列表没有更新，重启 Codex 再试。

### 方式二：手动安装

下载本仓库 ZIP，或克隆仓库：

```bash
git clone https://github.com/pirate-cc/laochen-technical-ppt.git
```

将 `skills/laochen-technical-ppt` **整个文件夹**复制到以下任一位置：

| 使用范围 | 目标目录 |
| --- | --- |
| 当前用户 | `~/.agents/skills/laochen-technical-ppt/` |
| 当前项目 | `<项目根目录>/.agents/skills/laochen-technical-ppt/` |

Windows 上 `~` 指你的用户目录。复制后，目标目录应直接包含 `SKILL.md`、`agents/` 和 `references/`，不要只复制 `SKILL.md`，也不要多套一层仓库目录。如果已有同名版本，先比较并保留自己的修改。

安装位置和 Skill Installer 的官方说明：[OpenAI：Build skills](https://learn.chatgpt.com/docs/build-skills)。

## 使用示例

提供源材料、用途和输出位置；有模板或视觉参考时一并提供，也可允许自主设计。例如：

**科研组会讲演稿**

```text
使用 $laochen-technical-ppt，依据项目中的论文、实验记录和现有模板，
制作面向课题组的 15 分钟汇报。讲清问题、实际做法和结果，
保留原生文字、图表和逐页动态，输出到项目的 output/组会汇报.pptx。
完成制作核对后直接交给我自行检查。
```

**保留已有动画的局部修订**

```text
使用 $laochen-technical-ppt，把现有 PPT 第 5 页替换为提供的新截图，
只调整必要的图旁说明，保留其他页面、格式与动画，保存到原文件。
```

**无模板的操作培训**

```text
使用 $laochen-technical-ppt，根据所附操作记录和界面截图，
制作面向新同事的 6 页培训讲演 PPT。没有模板，视觉由你设计，
讲清操作和对应状态，保留原生文字、标注与逐页动态，
输出到 output/操作培训.pptx，完成后直接交给我。
```

**只审阅，不改文件**

```text
使用 $laochen-technical-ppt，检查这份 PPT 的讲解顺序、文案和图文对应关系。
只报告问题、位置和修改建议，不保存或修改 PPT 文件。
```

## 运行条件与能力边界

本仓库提供工作流指令、参考规则和示例，不捆绑 PowerPoint 应用、PPT 生成引擎、模型服务、字体或第三方付费素材。

执行制作任务的 Codex 环境需要具备合适的演示文稿工具。现有模板编辑、原生图表和原生动画是否能够完成，取决于所用工具的实际能力；Windows PowerPoint 自动化是其中一种实现方式，并非所有环境都具备。本 Skill 不会自动安装 Office，也不会把静态导出视为动画已实现。需要生图或联网素材时，使用所在环境可用的相应工具；其账号、权限、费用与素材许可由实际服务决定。

示例属于教学或行为示范，不能作为新项目的实测数据、运行结果或播放验证。请提供本次任务的真实材料；要求模板保真时须有可使用的实际模板。

## 仓库结构

```text
laochen-technical-ppt/
├── .codex-plugin/plugin.json          # 保留的 Codex 本地插件兼容清单
├── skills/laochen-technical-ppt/
│   ├── SKILL.md                      # Skill 主规则
│   ├── agents/openai.yaml            # 界面元数据
│   └── references/
│       ├── asset-sources.md          # 素材获取与复用规则
│       ├── source-catalog.md         # 按需读取的来源目录
│       ├── layout-and-style.md       # 内容关系与稿内视觉参数
│       ├── visual-cases.md           # 内容交接、历史对比与修正版案例
│       ├── paired-evaluation.md      # Skill 修订验证
│       ├── collaboration.md          # 按需协作与单稿写入
│       ├── implementation-and-checks.md
│       ├── research-explanation.md   # 讲解逻辑与中文成稿
│       └── worked-examples.md        # 任务边界与制作示例
├── LICENSE
└── README.md
```

这是通过 GitHub 分发的 Skill 源码；安装请使用上面的 Skill Installer 或手动方式。仓库中的插件兼容清单保留原包信息，不表示已经上架官方插件目录。

## 修改与分享

欢迎 Fork、修改、商用和再分发本仓库原创内容，请按 [MIT 许可证](LICENSE) 保留版权与许可声明。参考资料中链接的第三方网页、图片、字体、工具及代码仍适用各自许可证；本仓库许可证不替代其授权。

反馈问题请使用 [GitHub Issues](https://github.com/pirate-cc/laochen-technical-ppt/issues)，说明期望行为、实际行为和相关工具环境。分享示例前请去除个人信息及未获授权的项目数据。
