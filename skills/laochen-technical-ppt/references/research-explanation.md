# Research explanation examples

Read the relevant section when introducing a technical subject, explaining figures or methods, replacing empty copy, or planning cumulative builds. Follow the [task scope](../SKILL.md#task-scope): a local wording edit uses the affected passage and enough neighboring context to preserve meaning; a review reports findings instead of rewriting the deck. For authorized writing, start from the supplied description and explain the relevant object, operation, or relationship. Source notes distinguish teaching material from recorded project comparisons.

按任务选读：[讲解顺序](#from-observation-to-method)、[材料范围](#let-the-materials-set-the-scope)、[页面角色](#substance-by-page-role)、[文案与来源](#writing-from-sources)、[辅助文字与备注](#audience-facing-qualifications-and-small-text)、[自然中文](#natural-chinese-technical-copy)。

## From observation to method

Before dividing a waveform-based report into pages, identify the audience's existing knowledge and what this report should help them understand. Read the available records, method descriptions, and outputs, then choose which concepts or objects must be explained before the next part can be followed. The roles below can guide that sequence. After choosing it, assign the concrete explanation and main material to each page, then select layouts. See the [audience-to-sequence example](worked-examples.md#story-and-pacing) for a worked internal plan.

| Explanatory role | What the audience needs | Suitable content |
| --- | --- | --- |
| 原始记录 | What is being analyzed, and how is the record read? | A representative record with channel/component identity, axes, and units. |
| 观察现象 | Which feature or relationship does the record show? | Locate a visible packet, changing segment, channel difference, or another source-supported feature and explain its shape or relationship. |
| 处理需求 | Which part of the record is the processing step concerned with? | Connect the observed feature to the actual detection, candidate selection, baseline handling, or display task. |
| 方法选择 | How does the operation work on that object? | Explain the key transformation and its input/output relationship in the actual or proposed processing order. |
| 输出解释 | How should the output be read? | Explain the output's curves, labels, values, or relationship to the original record using their actual meanings. |
| 总结 | What understanding or work does this segment deliver? | State the concept explained, operation implemented, observed comparison, or actual output. |

These are explanatory dependencies, not six required pages. Add a short prerequisite definition before a record when the audience needs it, and use familiar concepts directly when they are already shared knowledge. A literature-learning talk can introduce the paper's mechanism and figures with attribution; a system introduction can follow components and data flow. Select and combine the roles within the requested count after determining the explanation order. Complete that planning internally and proceed to content and layout.

## Let the materials set the scope

Select the aspect that the supplied material can explain directly. Develop that description into useful content, then finish at its natural scope. Do not turn material that was never part of the introduction into a report about missing conditions, data, or validation.

| Supplied material | Explanatory focus | What to write or show |
| --- | --- | --- |
| A diagram of record reading, detrending, and waveform display | Roles and data flow | Explain what reading supplies, what detrending changes, and how the display presents its output; place the explanation beside the corresponding nodes. |
| The formula for linear detrending | The operation itself | Explain fitting a straight line and subtracting it sample by sample, with the input, fitted line, and residual sequence. |
| A screenshot containing a waveform, candidate window, and P candidate | The interface's representation | Explain the window's time range, the point mark's position, and how the original and processed traces are distinguished. |
| A paper's description of one key step | The step's mechanism | Explain the quantity it uses, the transformation or rule, and its role in the paper's method. |
| Matched before/after waveforms with a defined ratio | The observed comparison | Identify the shared interval, explain the ratio, and describe the difference it shows. |

These are scope choices, not a required set of pages. Read the relevant code, formula, data definition, or original source when it helps explain the chosen subject. A mechanism introduction stays focused on the mechanism; an interface introduction stays focused on the interface. Evaluation questions are developed on pages whose task is evaluation. Speaker notes guide the explanation and retain sources rather than accumulating unrequested deficiency statements.

## Substance by page role

Start with the subject and write what the audience should understand about it. Select the relevant aspects; a complete introduction does not need a result claim, a judgment, or a next-step paragraph.

### Concept: explain a relationship

**Title:** 采样率与采样间隔

**Visible copy:**

> 1000 Hz 表示每秒采样 1000 次，相邻采样点间隔为 1 ms；100 Hz 对应 10 ms。采样率降为原来的十分之一，采样点之间的时间间隔就扩大到原来的十倍。

**Visual:** An editable teaching time axis with two sampling grids and labeled intervals. The relationship is Δt = 1/fs. Let the explanation finish with this relationship.

### Method: show the operation

**Title:** 线性去趋势如何处理缓变分量

**Visible copy:**

> 对分析窗内的波形 x(t) 拟合直线 at+b，再逐点相减：y(t)=x(t)−(at+b)。拟合直线描述窗内的线性变化部分，差值 y(t) 表示原波形相对这条直线的起伏。

**Visual:** Show the input waveform and fitted line on a shared time axis, then show the subtraction and output. Place the formula beside the transformation. A teaching diagram can explain the operation directly; an implemented workflow can use its actual intermediate arrays. See the [complete worked page](worked-examples.md#complete-one-slide-rewrite) for a numerical teaching example.

### System: explain components and their cooperation

**Teaching source:** A block diagram with three nodes: 记录读入 → 线性去趋势 → 波形显示.

**Title:** 波形从记录读入到处理显示

**Visible copy:**

> 读入模块将记录组织成带有时间坐标的波形序列。去趋势模块拟合窗内直线，并从序列中逐点减去拟合值。显示模块绘制处理后的波形，使处理步骤与对应的波形变化能够沿同一数据流阅读。

**Visual:** Keep the three supplied nodes and label the quantities passed between them: 波形序列 → 去趋势序列. The explanation gives each node a concrete role and connects the nodes through their data.

### Result: interpret a matched comparison

**Recorded source:** The supplied 28-slide deck “第二次组会_数据整理与信号处理.pptx”, slide positions 22–23, and existing M1-03 rows in “R12/input-chain-diagnostic/metrics.csv”. The interval is 33.00–33.65 s; the displayed ratios are rounded from 0.1282768633 and 0.7037612501.

**Title:** 同一窗口，两道降采样后的幅值变化不同

**Visible copy:**

> M1-03 在 33.00–33.65 s 内，道 1 的 RMS 幅值比为 12.8%，道 5 为 70.4%。同样转为 100 Hz，道 1 的均方根幅值减弱更明显。

**Adjacent definition:** RMS 幅值比 = 100 Hz 序列 RMS / 去趋势原生序列 RMS，描述同一原道处理前后的幅值变化。

**Visual:** Align the actual before/after waveforms to the stated interval. Retain each channel's identity and scale and place its ratio beside it. Keep the metric's meaning as relative RMS amplitude change. Detailed source records belong in notes; the visible copy finishes with the comparison.

### Plan: define an intended comparison

Use this page when the task includes planning the comparison. The following is an illustrative design continuing the recorded case.

**Title:** 重采样与标准化的分阶段对比方案

**Visible copy:**

> 固定 M1-03 的道 1、道 5 和 33.00–33.65 s 窗口，分别导出去趋势、100 Hz 重采样和标准化三个阶段的序列。用前两阶段计算 RMS 幅值比，再核对标准化阶段使用的分量标准差，定位各阶段对应的幅值变化。

**Visual:** Show the three sequences and the quantity compared at each stage, with shared record/window identifiers. The title identifies the page as a plan and the body specifies its operation.

### When a draft has no substance

Return to the subject. Expand a process name into its transformation, a module label into its function and connection, or a chart label into its observed relationship. For a method, inspect the operation in its code or source description. For a concept, explain the relevant definition, formula, or distinction. Retain short content when it already teaches a complete point. Removing an empty or defensive passage should leave room for a better subject explanation, rather than another passage about what is unavailable.

## Figure and adjacent explanation

Choose the composition from the subject being explained. Keep one dominant visual and enough adjacent text to relate its features to the technical point.

| Subject | Useful explanation | Visual connection |
| --- | --- | --- |
| A waveform comparison | Locate the shared interval and explain the shape or amplitude relationship actually shown. | Put the relevant channel names, interval, and ratio beside the corresponding traces. |
| Time-varying P/S probability outputs | Explain which curve represents each output and how the curve's time coordinate relates to the input record. When the page covers candidate selection, explain the selection rule from the actual implementation. | Use the supplied curves, their labels, and the relevant operation. |
| A processing method | Explain the transformation between the input and output with a formula or intermediate sequence. | Put the explanation beside the corresponding step. |
| A software screenshot | Explain what the window, point mark, control, or output represents. | Use a focused crop or editable cue on that visible object. |
| A system diagram | Explain each relevant component's role and what passes along its connections. | Keep the flow and explanation adjacent rather than splitting them into detached cards. |

A question can open a discussion, but the page still supplies its technical explanation. See the [software screenshot example](worked-examples.md#software-presentation-from-an-existing-screenshot) for a complete introduction to an existing interface.

## Locating evidence during explanation

For an overall figure or dense display, connect each explanation to a specific visible target before choosing its cue. A direct label and adjacent sentence may already make the target clear.

| Target | Suitable cue | Preserve |
| --- | --- | --- |
| A point, component, interface control, or isolated feature | A short leader/arrow or direct label | The target and nearby labels; route the leader through free space. |
| A time interval or spatial region | An outline box or light interval band | The underlying detail, axes, and the source's approximate or exact extent. |
| A channel group or related panels | A bracket, side marker, or restrained linked outlines | Channel/panel identities and the comparison relationship. |
| A detail too small to explain at presentation size | An enlargement linked to its region in the overview | Record identity, location, units, and any scale change. |

When authoring a live explanation, establish the overview first. Reveal or emphasize each cue with its matching explanation on the same click. Keep the overview stable, retain earlier marks needed for comparisons, and fade obsolete cues when they compete with the current explanation. A reading page may show a coherent static annotated state. Editing a caption alone preserves the existing sequence unless its changed meaning requires an adjustment within the requested scope.

Set the cue's position and extent from the source figure or data. Link overview and detail through their actual record, channel/panel, and time or spatial correspondence. Use the source's own meaning for labels and scales. Record “讲解点 → 图中对象或范围 → 标注方式 → 点击阶段 → 保留内容” compactly in the existing plan or notes when needed. The [waveform examples](worked-examples.md#overview-with-progressive-annotations) show possible builds.

## Explain the method in the project

Use the relevant parts of the supplied description to explain the method:

| Piece | What to explain | Useful placement |
| --- | --- | --- |
| Input | The data or previous output entering the operation. | Beside the incoming arrow or input object. |
| Operation | The quantity calculated, transformation performed, or selection rule applied. | Beside the formula, structure, or worked intermediate result. |
| Output | The sequence, curve, window, value, or label produced and what it means. | Beside its example or outgoing arrow. |
| Role | How this operation fits the supplied paper, design, or actual processing flow. | Along the connection it helps explain. |

These are aspects of one explanation, not four boxes to fill. “拟合直线并逐点相减” explains an operation; “处理：预处理” simply repeats a category. A method introduction can finish after explaining its transformation and function. A local performance assessment is a different page task.

Connect methods through the actual quantities they pass. For a waveform → probability curve → candidate position chain, explain each quantity and the operation that produces the next one from the supplied implementation. Use a paper's flow for literature learning and the code's actual flow for implemented project work.

## Concept comparisons

Select distinctions because they help the audience understand the subject or read its figures. In a P/S introduction, the relevant material may connect particle motion, propagation properties, and visible arrival features. Explain the chosen relationships using the scientific source. Let the material and audience determine the dimensions, rather than filling a universal comparison table.

## Cumulative method chain

For a documented chain “input → method A → intermediate output → method B → final output”, a possible build is:

| State | Newly visible | Retained context |
| --- | --- | --- |
| Entry | Input object, identity, and necessary axes/units. | Title and input context. |
| First click | Method A, its incoming arrow, and its operation explanation. | Input and essential context. |
| Next click, if useful | Intermediate output and its meaning. | Input, Method A, and the preceding arrow. |
| Following click | Method B, its incoming arrow, and its explanation. | Upstream chain and intermediate output. |
| Output stage | Final output and its concrete interpretation. | Earlier steps needed to relate output to input. |

Combine an intermediate output with its method when a separate click adds little. Within a semantic stage, use one click and coordinated effects for the part, connector, and explanation. Decide grouping before assigning effects and retain stable targets. Use [native implementation guidance](implementation-and-checks.md#native-animation) for mechanics and fallback constraints.

## Feedback cases and acceptance criteria

Apply these writing choices while authoring the requested deck.

| Feedback case | Expected authoring result |
| --- | --- |
| The talk follows source-file order or fills template pages before its explanation order is chosen. | Use the audience's prior knowledge, goal, and supplied subject matter to determine the explanation order first; distribute page content next and lay it out afterward. |
| A page uses concepts or outputs before the audience has the context to understand them. | Introduce the needed concept, input, or overall relationship earlier and connect the dependent page to it. |
| Copy contains attitudes, repeated titles, process names, or generic promises. | Explain the subject's actual operation, role, feature, or relationship. |
| Copy has professional meaning but reads like an abstract slogan or an awkward translation. | Name the concrete subject and use familiar verbs; explain the term through the visible example. Read the title and its paragraph together and rewrite the wording before layout. |
| An introduction is interrupted by project deficiencies or validation commentary. | Develop the available structural, conceptual, or operational description and finish at that scope. |
| A method page is treated as a performance-evaluation page. | Explain its transformation and function; use evaluation content when evaluation is the page's task. |
| Figure-side copy asks a question without explaining the figure. | Locate the relevant feature and state the relationship it shows. |
| The audience cannot locate the referenced figure region. | Establish the overview, then present each cue with its matching explanation. |
| The page lists component names without showing cooperation. | Explain their roles and what passes along the connections. |
| Every page ends with a plan or validation sentence. | End a completed introduction with its technical explanation; write a plan when the task calls for one. |
| Methods and arrows all appear at entry during a requested step-by-step explanation. | Reveal each downstream method with its incoming arrow and explanation, retaining preceding context. |
| A concept comparison gives only a surface feature. | Explain the source-supported relationships that matter to the audience. |
| Fonts vary or labels compete with the waveform. | Use a coherent Chinese hierarchy and allocated label space, keeping necessary context legible. |

Keep the user's completion mode and requested count. For review-only work, report the relevant writing findings and evidence; revise only when modification is authorized. Use [task-boundary cases](worked-examples.md#task-boundary-cases) for local and mixed requests. One-off slide numbers and placements remain instructions for that presentation.

## Writing from sources

- 新建或整体重做时，先根据听众已有知识和目的选择讲解顺序，再分配页内容。需要的定义、输入或整体关系先于依赖它的细节与输出；文献、设计与实际实现各沿其真实方法和数据关系解释。局部修订沿用已确认的整体顺序，只处理受影响的含义与衔接。文件顺序、模板占位顺序和某个通用大纲不能替代这一判断。
- 把名称展开为具体知识：概念解释含义和关系，方法写关键运算和输入输出，组件写作用与连接，图旁文字写实际特征或差异。必要时用公式、算例或中间输出，先写清完整解释再安排布局；不固定字数、句数、四框结构或每页结尾。
- 结果和决策可使用有依据的结论标题；背景、定义和过程可直接命名对象或操作，如“观察波形”“候选事件识别流程”。封面先交代人物、作品或主题，内容页标题准确概括该页；按 [标题与封面](#titles-and-cover-copy) 选择自然写法。冗余“文献学习”等装饰标签可去掉，确实标识章节或任务时保留。
- 项目进展依据记录说明做了什么与得到什么；概念或文献页直接介绍来源主体和理解。对用户有记录的工作可用第一人称，文献内容归于原作者；一个案例可以反复使用，只要各页增加不同的具体解释。
- 相邻页通过概念、数据交接、观察或实际结果衔接。图旁文案应指出所解释的区域、曲线或关系，讨论问题可伴随解释而不替代它；按任务提出具体组会讨论，不为每页附泛化计划或验证句。
- 一次删除某页、调整页序或固定标题只作用于当前演示，不升级为永久页号、禁用标题或统一顺序。材料未涉及的条件按现有范围处理；实际比较的不确定性、样本和事实状态仍完整保留。

## Audience-facing qualifications and small text

Use on-slide text to explain the subject. Preserve the information needed to read an object or figure, and choose its placement by that explanatory role.

- Default to a title followed directly by substantive content. Do not routinely fill a smaller gray subtitle or a detached bottom takeaway with presenter cues such as “本页主要介绍…” or “接下来我们来看…”. Put useful spoken transitions in notes; a template's subtitle box need not be filled.
- Retain a subtitle or short explanation when it supplies a concrete scope, condition, definition, or finding needed on screen, or when the user requests it. Integrate technical explanation into readable body text or beside its evidence; preserve necessary labels, units, captions, and qualifications. See the [subtitle example](worked-examples.md#title-without-a-presenter-cue).
- Keep necessary explanations beside images, screenshots, charts, and diagrams. Otherwise, minimize unrequested reminder lines, generic advice, repeated summaries, and supplementary workflow tips. A line such as "先用真实任务试一次，再按输出补充规则" below a complete example normally belongs in speaker notes if useful to the presenter, or can be omitted. Do not add a small sentence just to fill remaining space or close each page.
- Remove extra lines rather than enlarging, recoloring, moving, or relabeling them as captions. Integrate information needed for the technical explanation into the readable body. Preserve figure labels, units, relevant domains, required credits, and explicitly requested text. See the [example below a task prompt](worked-examples.md#auxiliary-small-text-below-an-example).

| Information | Placement |
| --- | --- |
| Object names, labels, units, variable meanings, and technical conditions that define the subject | Readable title, figure caption, or adjacent explanation; reveal them with the object they explain. |
| An actual comparison's sampling basis, error bars, uncertainty, or result status | Beside that comparison on an evaluation or result page, preserving the source's meaning. |
| Asset source, generation method, or detailed provenance that does not change interpretation | Speaker notes by default; preserve visible credit or disclosure when the license, venue, or user requires it. |
| Render checks, editability claims, tool limitations, or other production commentary | Internal QA or the delivery message when relevant; keep it out of the audience's slides and talk track. |

- Use accurate subject names such as "井下观测场景示意", "线性去趋势算例", "仿真结果", or "采集模块设计". Identify realistic illustrations as illustrations and simulation plots as simulation results; keep generation details and source records in notes unless visible credit is required.
- An introduction does not automatically need a deficiency or validation statement. Do not append "当前没有……", "暂时不能判断", "尚未验证" or equivalent passages to its body, footer, or speaking notes. When material covers only the structure or mechanism, finish that explanation at its natural scope instead of discussing absent experiments or conditions.
- Explain a technical condition as part of the subject when it matters: "线性去趋势通过减去拟合直线处理窗内线性漂移" identifies the operation's scope. Preserve an actual result's uncertainty, status labels, and comparison basis where those define its meaning. This does not require a separate paragraph about what the project cannot establish.

Speaker notes may hold explanation cues, necessary detail, source attribution, and a transition to the next slide. Live slides still need useful labels, units, and conditions; reading decks need enough visible explanation to stand alone. See [live and reading versions](worked-examples.md#live-and-reading-versions) for the same evidence in each use. Do not impose a word quota or a verbatim script on every page. For note mechanics when needed, see [Duarte's guide](https://www.duarte.com/blog/everything-need-know-using-speaker-notes-in-powerpoint/).

## Natural Chinese technical copy

- 交付可直接上屏和讲解的文字。围绕具体对象写清所需的含义、做法、关系或现象；正文是完整解释，不能只给概念标签或等用户扩写的提纲。备注可补充例子与讲述节奏，可见文案本身应当清楚。
- 使用自然、准确的专业中文。检查主语指向、动宾搭配和因果关系；连续使用“经营、统合、赋能、贯通、体验”等抽象词时，回到它们实际指代的对象和操作。保留确有含义的用词，不建立机械禁词表。例如将“以格局统合具体的要素”改成“先确定山、水和建筑的整体布局”，再解释各自的位置和联系。
- 专业术语有教学价值时保留，并用听众能理解的例子解释。园林课可以保留“动观、静观、对景”，同时说明人在什么位置、看见什么，以及路径或景物怎样安排；不把术语换成同样抽象的口号。技术含义、机制和结论仍以实际来源为准。
- 不为对仗、四字短语、字数、行数或卡片数量增删含义，不补造第三项来凑齐列表。保留真实的并列关系和正常对齐，“检测与拾取”或“动观与静观”可以直接作为主题。布局适应合理的长短差异，不把全部标题改成同一种“概念：让……”或“以……实现……”句式。
- 在授权写作范围内连同页标题、小标题、正文和图注通读所需相邻上下文：一句话是否能顺口讲出，听众能否确定它在说哪个对象，标题是否得到正文和图片的解释。发现生硬搭配、抽象堆叠、指代不明或重复句框时改写受影响文案；范围外问题只在影响当前任务时指出。只读审阅交付这些发现与建议。
- 内容有实质与表达自然需要同时满足。去掉空话或防御性文字后，补足相关知识；有知识但不好读时，改写表达而保留含义。不要把必要解释全部挪进备注，也不要把冗余句换成更大的强调文字。参见 [自然中文改写](worked-examples.md#natural-chinese) 和 [完整园林教学页](worked-examples.md#garden-teaching-page)。
- 文字排得下与文字写得好分别处理。用实际中文、可用字体和文本框尺寸安排标点、混排、单位、符号与换行；不靠空格或随意断句凑齐行长，不把英文词数估算当成中文适配证明。保存与检查按 [制作核对](implementation-and-checks.md#minimum-production-confirmation) 执行。

### Titles and cover copy

- 封面主标题优先标明人物、作品、项目或课程主题，副标题按需补充案例、范围或角度。例如主标题“陈从周的园林设计”，副标题“以豫园东部修复为例”。不默认用文艺口号占据主标题；用户指定风格或有必要引用时，保留准确出处并让主题清楚可见。
- 页标题采用该页最自然的表达：对象名称、具体操作、比较问题或有依据的结论均可，不强制冒号、对仗或结论句。小标题应帮助辨认内容，正文能直接说明时无需再加抽象概括。
- 概念含义需要展开时放入正文。例如标题可写“动观与静观”，正文说明沿游路移动与驻足观看的差别；若该页讨论设计操作，可写“动观与静观：游线和观景点的安排”。标题长度由信息决定，不能靠省略关键对象制造简洁。
