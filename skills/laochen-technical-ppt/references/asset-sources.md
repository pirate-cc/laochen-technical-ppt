# Asset sources and lookup

按 [任务范围](../SKILL.md#task-scope) 处理本次素材缺口。先复用提供的文件与项目材料；仅审阅不下载替代素材，局部替换保留原图承担的解释任务。

执行顺序：[选择途径](#choose-reuse-search-drawing-or-generation) → [复用](#reuse-local-and-connected-material)、[检索](#search-and-inspect) 或 [生图](#generate-assets-for-the-slide) → [保存记录](#keep-selected-assets-reusable)。出现具体缺口才打开 [来源目录](source-catalog.md)，成套模板另按 [模板选型](template-selection.md)。

## Scene to material

从现有正文与原材料确定每张图支持的说明、关系或判断，以及真实证据/示意用途、需同时看到的内容与独立编辑/运动对象；不另设问卷或素材数量指标。没有配图需求时不为占位取材。下载或生图前按 [效果关系](implementation-and-checks.md#choose-the-effect-from-the-explanation) 确认图层，素材到位后 [共同修订正文与构图](research-explanation.md#copy-and-asset-iteration)。

以下边界适用于所有途径：

- 真实截图、观测、项目设备与结果必须有对应源材料；保留身份、版本/日期、单位和时空对应。参考照片、旧项目截图和概念插画不转为本次实测证据，示意/现代重构不证明真实部署或历史状态，缺失状态不为动画流畅而编造。
- 约定独立编辑/运动的组件、标签、连接与数据保持 [原生编辑粒度](implementation-and-checks.md#template-and-object-editing)。照片、位图、矢量导出和媒体预览本身不证明组件可编辑，也不能替代所需 PPT 原生动作。

## Choose reuse, search, drawing, or generation

| 需要表达的内容 | 选用途径与区别 |
| --- | --- |
| 项目证据、实际操作状态 | 复用实际记录、截图、设备图或数据；操作图保留控件、反馈与未变上下文。 |
| 真实对象、作品、历史场景 | 查原作者、厂商、持有机构或适合图库的原件，核对具体对象和时间/地点；保留总览与细节的对应。 |
| 连接、过程、空间关系、数量 | 直接用原生图形/图表，或适配可编辑源文件；可靠平面图/照片可辅以原生标注。箭头、比例与连接由本次材料决定，无须另找装饰图。 |
| 概念场景、氛围、前景插画 | 通常检索现有素材；用户指定生图，或定制构图、视角、统一外观有明确收益时使用 ImageGen，不必先穷尽网站。明确要求位图插画时使用图像工具。 |
| 版式与成组视觉设计 | 沿用模板或适合的设计参考；用本次内容转译关系，工具与导出能力按下文核实。 |

## Subject-led visual design

构图、主次、卡片取舍和字体/间距统一按 [版式规则](layout-and-style.md)。素材匹配既定色温、对比、视角与密度，图标使用一致系列，重复对象保持外观身份。按分镜准备分离的背景、前景与原生标注/连接；截图可聚焦裁切或总览加放大，但保留影响解释的警告、控件、标签和上下文。

### Visual quality and image replacement

先诊断替换要改善外观、细节、位置、路线、结构、比较还是氛围，再换素材或图形表达。换色不能解决图形选择错误；标签正确不代表粗糙图形已合用，漂亮照片也不能补出隐藏连接。必要关系未显示时补可靠来源或配套结构图，完成后用下文统一的候选检查。

按需参照 [产品](worked-examples.md#product-introduction-with-editable-motion)、[操作](worked-examples.md#procedure-training-with-native-interface-states)、[比较](worked-examples.md#comparison-with-supplied-data)、[多模型](worked-examples.md#comparing-related-models-on-one-slide) 或 [混合页](research-and-revision-examples.md#revising-a-mixed-technical-page)；只迁移方法。

## Reuse local and connected material

按对象名、别名、图注与现有索引查找用户提供文件及相关项目目录，不遍历无关个人目录。已有合适原件不重复下载/生成；提取前核对版本与用途，按下表保留各格式特有关系，来源身份统一记入 [素材记录](#keep-selected-assets-reusable)。

| 来源格式 | 提取与保留要点 |
| --- | --- |
| PPT | 查看相关页及邻页；需要原生结构时复制原页/对象。图片按 slide/object 的关系定位 `ppt/media/`，不能按媒体文件名推断页序或裁切。保留裁切、标签、分组、图表数据与动画依赖，不把原生对象截图替代。 |
| DOCX / PDF | 先定位图注及页/图号；DOCX 按文档关系取 `word/media/`。PDF 优先提取原图/矢量，提取会丢组合含义时用页面裁切；保留图注、单位与必要上下文。 |
| 表格、绘图、SVG、Visio、设计源文件 | 优先复用数据、图表或原生对象，检查字体、链接资源与数据依赖。`xl/media/` 内图片不是完整图表，图表还需数据和关系。用现有格式工具提取并核对实际编辑粒度。 |
| 图片/素材目录 | 从现有索引或来源笔记取选定原件与实际使用图层，保留透明度，保护源文件。 |

本地不足且已连接服务直接适用时再查素材库，按当前工具契约及对应 Skill 使用；“能搜索/看到设计”不等于已授权素材、可导出或可访问整个库。

## Choose sources by purpose

从对象、作品、过程、场所或数据的创作者、持有者、发布机构定位原件；不因题材未在示例中出现就限于熟悉但无关的网站。按需查看 [来源类型](source-catalog.md#choose-sources-by-purpose)。

### Example starting points

按缺口选读 [常用入口](source-catalog.md#example-starting-points)。

### Additional asset libraries

补充素材库的用途、格式与特有许可见 [来源目录](source-catalog.md#additional-asset-libraries)。

## Content methods and complete-talk examples

具体设计/讲解问题需要参考时选读 [方法与完整案例](source-catalog.md#content-methods-and-complete-talk-examples)，已有合适参考不另搜。

### Adapt design references

查看少量相关作品的实际画面与必要邻页，借鉴动作先看实际运动；在现有笔记记链接、借鉴点与适用页。把有用的层级、比例、配色、裁切或注意力转移转为本次内容，按中文密度、演示比例和观看距离调整，保留关键子组差异与比较条件。不照搬原案例事实、网页/海报小字或固定叙事，不重选已确认方向。

执行 [版式](layout-and-style.md)、[图表](implementation-and-checks.md#scientific-charts) 和 [制作核对](implementation-and-checks.md#minimum-production-confirmation) 的相应规则，不增一轮审批/检查；仅借鉴规律不下载整套作品，直接复用图片、字体、代码则检查许可。

## Search and inspect

1. **定向找原件。** 用本次对象/型号/作品标识 + 解释用途 + 必要视角/格式形成查询；只在有用时增加别名、中英文或 `site:` 等限定，不机械跑同义词。用可用检索/浏览器（含 Edge，尊重用户选择）找原始页面；需要比较视角时用图像搜索。未知截图按标题、图注、署名或独特主体追溯，反向搜图仅在工具支持时使用。
2. **取得对应文件。** 打开原始页面和实际图/可用预览，缩略图与搜索摘要不能作为最终素材、事实或许可依据。论文跟到补充材料/原图/仓库，馆藏跟到条目及下载，仓库只查看所需文件、README 和许可，不默认整库克隆。不能为看图运行仓库脚本；确需执行已授权绘图代码时按项目实现与验证要求处理。
3. **统一验收候选。** 检查主体与技术含义、适用版本、计划裁切/尺寸下的细节和标签、比例、分辨率、透明背景、所需图层及真实编辑能力；保留轴、单位、条件与必需署名。按用途选原分辨率、透明图、矢量/图层或绘图源文件，不凭后缀和文件大小判断。满足解释用途且来源、许可明确就取原件并停止，只为具体未解决缺口继续搜索。
4. **调整失败路径。** 连续不匹配时换标识、来源类型或图形表达，访问受限时换可用路线；允许的概念可生图，确认的关系可绘制，缺少真实证据则说明具体缺口并继续独立工作。检索停止条件不缩减事实核验或已约定文献研究范围。

## Keep selected assets reusable

更新现有素材索引/笔记，不新建并行台账或登记所有淘汰候选。对选定素材紧凑记录：主体/有用别名、项目内路径、原 URL 或源文件及页/对象/图号、创作者与许可/署名、证据或示意身份、编辑粒度、必要图层/数据依赖、用于哪页；生图另记最终提示词、工具及参考图身份。替换时更新同一条记录。

保存原件及实际使用/后续编辑所需衍生文件，更新 PPT 引用并在格式支持时嵌入使用的媒体；不依赖生成工具临时目录或临时 URL。选材时的图像检查不扩大成稿审阅范围。

## Generate assets for the slide

按 imagegen Skill 使用内置图像工具，并遵循输入参考、透明背景及图片交付规则；普通插画不默认切换 CLI/API、付费服务或模型。工具不可用时换已授权途径或说明缺口，不把占位图说成已生成作品。

从计划页面写提示词：主体与解释用途、既定风格/色彩、视角/比例、文字留白、必须保留的关系及独立图层。原生标签由 PPT 添加时要求图中无文字；不增无关道具、虚构细节或装饰数字。背景留出叠加空间，移动前景单独生成并保留真实 alpha；需要独立连接/运动的组件不能合成一张平图。

系列图使用已确认图作外观/身份参考，仅生成实际需要的变体与图层。按 [候选检查](#search-and-inspect) 验收，并额外检查科学合理性、透明度和意外文字，针对问题修正后统一 [保存记录](#keep-selected-assets-reusable)。示例见 [独立图层场景](worked-examples.md#conceptual-scene-with-separate-layers)，不将其风格套为默认。

## Tools and delivery surface

工具选择及导入、原生编辑、动画能力统一按 [工作界面](implementation-and-checks.md#choose-the-working-surface) 核实，遵守用户指定工具与交付形式。Figma、网页和视频导出不自动保留所需 PPT 对象/效果；Figma 路线参照 [官方导出说明](https://help.figma.com/hc/en-us/articles/24848334599447-Export-from-Figma-Slides) 与实际文件。图表、截图或结构图足够时不补装饰图片。

## License and provenance check

直接复用前核对原条目/文件的现行许可、授权与修改要求，记录在现有素材笔记。需要可见署名时保留在页面，只有符合实际要求时才能放备注；免费可下载、搜索过滤条件或公开仓库不等于已获使用许可。各来源特殊条件见目录，仓库内图片/字体仍按各文件条款核实。

仅在选用对应来源时查：[Commons](https://commons.wikimedia.org/wiki/Commons:Reusing_content_outside_Wikimedia)、[Openverse](https://openverse.org/about)、[Unsplash](https://unsplash.com/license)、[Pexels](https://www.pexels.com/license/)、[Lucide](https://lucide.dev/license)、[Servier](https://smart.servier.com/terms-of-use/)。

检索不自动授权订阅、付费、新建连接或上传私人源文件；受限时换可用来源或在授权范围内绘制/生成。不增加审批节点，也不改变已确认的内容、风格和页数。
