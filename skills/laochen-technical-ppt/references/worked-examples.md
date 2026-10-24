# Worked examples

These examples show how to introduce a subject from supplied material and retain its concrete explanation in the template. They include teaching calculations and explicitly identified historical material. Select only the example needed for the current task and adapt it to the actual source, visual style, and requested count.

## Task boundary cases

Use these cases to apply the [task scope](../SKILL.md#task-scope), [production confirmation](implementation-and-checks.md#minimum-production-confirmation), and [collaboration choices](collaboration.md#task-selection). The stated outcomes are expected behavior, not claims that these tasks or their playback have been run.

| User request | Scoped work | Observable outcome |
| --- | --- | --- |
| “检查第 3–5 页的讲解逻辑和文案，告诉我哪里可以改。” | Read those pages and the source or neighboring context needed to judge them; report concrete findings and suggestions. | The report locates each finding and explains its basis. The PPTX is unchanged, and no revised deck is created. |
| “检查并修复第 4 页的动画问题，其他页面保持原样。” | Inspect the requested sequence, repair the affected objects/effects, and repeat the affected requested check. | Corrections stay within the page and its necessary dependencies. Report actual configuration/playback evidence separately and retain any limitation. |
| “把第 5 页标题改成‘候选窗口与点标记’，其余不动。” | Read the title and necessary context, replace its text while preserving run formatting and effect targets, then confirm the saved write. | Only the title and any unavoidable formatting dependency change; no deck-wide rewrite, asset search, or animation additions. |
| “第 5 页换成这张新截图，保留文字和动画，我自己检查。” | Inspect the supplied image, use the existing picture object's crop/placement where appropriate, and preserve its animation identity. If replacement changes the ID, remap the affected targets before saving. | The new screenshot and its referenced effects are saved. No new visual direction or finished-deck playback round is introduced. |
| “沿用模板做 12 页技术讲演 PPT，做完交给我自行检查。” | Arrange the explanation, create the full deck, and apply the live-talk default to all 12 slides, including any cover, transition, and closing slides within that total. | Deliver one editable 12-slide deck with actual native effects and minimum production confirmation; do not add outline approval, rendering, or playback. |
| “把这些内容做成 8 页静态阅读版，保留图表数据可编辑。” | Write enough visible explanation to read independently, use coherent static annotated states, and preserve native chart/data relationships. | Deliver the requested 8-slide static deck; do not add a live-talk copy or impose the animation default on this use. |
| “文案和真实数据已定，重做场景素材和复杂原生动态。” | When these two areas have independent workload, delegate B for assets/layers and C for production. The main agent handles the remaining content/source coordination. | B+C is a complete valid combination; C is the sole PPTX/script writer. No A role is created just to fill the team. |
| “只生成一张监测场景背景，给我图片和提示词。” | Generate and save the requested background and prompt under the asset workflow. | Deliver the image and prompt; no presentation is created. |

When workflows are combined, use presentation tooling for the chosen file operations and required format checks while preserving the user's stated scope and review choice. For example, the 12-slide direct-delivery case does not gain a render-every-slide phase from a general workflow. If the tool cannot preserve the required native animation, report that feature limitation and continue independent work; a static export is not an animated delivery.

For a Skill revision, these cases can guide a focused behavioral check with appropriate source files. Judge the actual report, file changes, object preservation, and chosen roles; matching phrases in the Skill is not execution evidence. Do not turn this table into a mandatory test round for every deck.

## Story and pacing

This illustrative planning case uses material already represented in these examples: a waveform with channel/time labels, a linear-detrending description and four-sample calculation, a record-reading → detrending → display diagram, and an interface showing original and processed traces. Work through audience, order, page content, and layout internally, then complete the requested deck.

### Choose the explanation order

First decide what this audience should understand from this material. The same source set can support different starting points and levels of explanation:

| Audience and goal | Chosen explanation order | Reason for the order |
| --- | --- | --- |
| New learners who know arithmetic and need to understand detrending and read its displayed output | 认识波形的坐标 → 理解拟合直线 → 跟随逐点相减 → 阅读界面中的处理结果 | The waveform supplies an object to follow; the fitted line gives subtraction a concrete meaning; the interface then connects the calculated output to its representation. |
| Colleagues familiar with waveform reading who need to understand how processing and display are connected | 软件整体数据流 → 关键去趋势运算 → 处理前后波形的显示关系 | Begin at the system level they need, expand the key operation, then relate its output to the display. Use their existing waveform knowledge to keep the explanation focused. |

These are possible internal choices, not two decks to produce. Use the audience and purpose from the actual request. Keep the diagram's actual processing order while choosing which parts need introduction or expansion.

### Assign content, then lay out

For a new or substantially remade segment in the new-learner case, translate the chosen sequence into the following illustrative pages. Combine or split its content within the requested total count and speaking time; a narrow correction does not reopen an already confirmed sequence.

| Order and page subject | Concrete content | Main material | Connection to the next page |
| --- | --- | --- | --- |
| 1. 波形的时间轴与通道 | Explain how to locate a sample or interval and distinguish the displayed channels. | The supplied waveform with readable labels and a focused cue. | The audience can read the sample positions used in the teaching calculation. |
| 2. 拟合直线描述窗内线性变化 | Explain the input points, fitted line, and fitted values at the sample positions. | The four-sample teaching plot with its formula. | The fitted values become the quantities subtracted on the next page. |
| 3. 逐点相减得到差值序列 | Walk through representative subtractions and explain what the residual sequence represents. | The input, fitted values, subtraction, and output from the teaching calculation. | The audience knows which kind of output the interface presents. |
| 4. 原始波形与处理波形怎样对照 | Explain the source screenshot's original/processed color labels and corresponding time range. | The actual interface screenshot with nearby explanations. | Completes the segment by connecting the operation to its display. |

The four-sample calculation explains the operation; the interface page uses its screenshot's actual record and labels. Once the sequence and these page explanations are established, select the template's appropriate waveform, method, and screenshot layouts. Arrange the needed plots, formula, arithmetic, and adjacent copy using their native objects. Estimate pacing from the explanation: locating an interval, following a calculation, and reading a screenshot take different amounts of time. The page sequence and content guide the composition and native builds; template placeholders do not determine the talk's order. Continue into the complete deck without asking the user to confirm this internal plan.

## Initial literature learning

For a literature-learning meeting, first use the audience's prior knowledge and the supplied paper to choose the starting point. New learners may need the task's object and a key definition before the mechanism; an audience familiar with that task can begin with the method's overall structure and expand its key operation. Determine this explanation order first, then distribute its content into pages. The following table illustrates an object → operation → connected method sequence.

| Page role and possible title | Content and visual | Connection |
| --- | --- | --- |
| Introduce the object: 这篇研究处理什么对象 | Explain the paper's input, task, and relevant setting using its task definition or original figure. | Gives the method a concrete object. |
| Explain the mechanism: 关键步骤怎样完成处理 | Expand one important operation using the source's formula, diagram, or worked example. Explain what changes between input and output. | Makes the method understandable beyond its name. |
| Connect the method: 各步骤通过什么结果衔接 | Show how one step's output becomes the next step's input and how the resulting output is read. Use the paper's quantities and terminology. | Forms a complete account of the method. |

These roles may be combined or expanded. Choose the concepts needed to understand the supplied paper; attribute its figures and findings to the authors. Introduce the presenter's understanding in natural Chinese. A specific discussion question may be added when discussion is part of the task, rather than giving every literature page an unresolved-question ending.

## Semantic build

After choosing the talk's sequence and assigning the linear-detrending content to a page, follow its within-page explanatory order:

| State | Visible content and explanation |
| --- | --- |
| Entry | Original sequence, sample-index axis, and page title. |
| Fit | Fitted line, fitting formula, and the sentence explaining the linear component appear together. |
| Subtract | Subtraction and residual sequence appear with the sentence explaining the output. |

The earlier content stays available so the audience can relate output to input. Implement coordinated native effects for this live-talk page and choose stages by meaning. The [live-talk default](../SKILL.md#core-requirements) also covers simple pages in a new or wholly remade deck; a local text revision preserves the existing sequence. Use the [live and reading versions](#live-and-reading-versions) below for a static reading request.

## Overview with progressive annotations

### Source material

The supplied second-meeting deck “第二次组会_数据整理与信号处理.pptx” contains an overall multi-channel record and a page of local three-channel groups. Their captions describe an enhanced packet near 12 s in the overall view and changing waveform segments around 33.1 s in the local panels. Each figure retains its own record identity and time range.

### Overall multi-channel record

| Stage | Newly visible or emphasized | Retained context |
| --- | --- | --- |
| Entry | The complete overall record with channel identities, time axis, and scale information. | Page title and figure context. |
| Locate the shared change | A narrow outline or light time band around the source-supported region near 12 s, together with the explanation of the enhanced packet. | The overall plot and axes. |
| Explain channel differences | Representative regions with their explanations of packet shape or persistent oscillation. | Channel identities, the shared interval, and the display's scale information. |
| Detail, if useful | A linked enlargement of the selected segment. | Its selection in the overview and matching record/channel/time labels. |

Use a region cue for a shared interval and choose channel examples from the actual source. Interpret amplitude according to the figure's actual scaling.

### Local three-channel groups

| Stage | Newly visible or emphasized | Retained context |
| --- | --- | --- |
| Entry | The complete set of local panels with readable group/channel identities and time axes. | The window and scale information. |
| Locate the change | Bands or outlines on the segments associated with “约 33.1 s 后”, together with their amplitude-change explanation. | All panels and the time context around each segment. |
| Compare packet shapes | A short packet and a sustained oscillation, with each explanation beside its selected region. | Group/channel identities and the earlier interval cues needed for comparison. |
| Detail, if useful | An enlargement of the representative fragments. | Source selection and matching time ranges. |

Set annotation boundaries and phase labels from the original figure or data. Treat an enlargement as a detail of an overview only when their record, channel, and time correspondence establishes that relationship. Keep each cue editable and reveal it with its matching explanation.

## Mechanism motion with editable objects

**Page role:** Explain particle vibration in solid material. Use the P/S relationship from [USGS: P Waves and S Waves in the Crust](https://www.usgs.gov/media/images/p-waves-and-s-waves-crust). This is a schematic teaching example; its particle positions and timing are illustrative, not field measurements.

**Title:** P、S 波的质点振动方向不同

**Visible copy, revealed beside each mechanism:**

> P 波的质点沿传播方向往复振动，形成交替的压缩与伸展。
>
> S 波的质点垂直于传播方向往复振动。

**Composition and asset choice:** Use two aligned bands with the same propagation arrow pointing right. Draw material points as native circles and equilibrium positions as small native marks. Emphasize one tracked particle in each band. Give the diagrams prominence, with the two explanations beside their bands; use the template's existing category colors and line weights. Native geometry supplies the mechanism accurately, so this page needs neither a stock photo nor a generated full-page diagram. Label the visual “振动方向示意”.

| Object role / suggested name | Initial state | Native action and trigger | What remains visible |
| --- | --- | --- | --- |
| P/S material bands, propagation arrows, equilibrium marks | Visible on entry; all particles at rest | Keep fixed reference geometry. | Propagation direction and equilibrium positions. |
| `P_particle_focus` and `P_explanation` | Particle visible at equilibrium; explanation hidden | On click, show the explanation and move the particle right, then left through equilibrium, then return to rest. Use a short coordinated motion-path sequence. | P explanation and the particle at its equilibrium position. |
| `S_particle_focus` and `S_explanation` | Particle visible at equilibrium; explanation hidden | On the next click, show the explanation and move the particle up, then down through equilibrium, then return to rest. | Both bands and both explanations for comparison. |

Plan the displacement around equilibrium; do not move the material particle along the entire propagation arrow. If the diagram includes neighboring moving points to show a traveling wave, derive their positions from a consistent wave model rather than animating all points in phase. A brief motion sequence ends at a readable stable state; the presenter starts the next comparison. Keep all particles, arrows, labels, and effects native. A simple label fade is insufficient to implement this mechanism.

**Source note:** Preserve the USGS mechanism reference in notes. Use no numerical speed ratio unless the current source and page actually require one. Adapt the composition and stages to the requested count; the example is one page, not a reason to add extra slides.

## Matched waveform comparison

**Historical material:** Reuse the [recorded M1-03 comparison](research-explanation.md#result-interpret-a-matched-comparison): channels 1 and 5, the 33.00–33.65 s window, detrended native-rate and 100 Hz sequences, and recorded RMS ratios rounded to 12.8% and 70.4%. This example specifies how to present that documented comparison; it does not report a new processing run. For another record, use its own source data, interval, and computed quantities.

**Title:** 同一窗口，两道降采样后的幅值变化不同

**Visible copy:**

> M1-03 在 33.00–33.65 s 内，道 1 的 RMS 幅值比为 12.8%，道 5 为 70.4%。同样转为 100 Hz，道 1 的均方根幅值减弱更明显。

**Adjacent definition:** RMS 幅值比 = 100 Hz 序列 RMS / 去趋势原生序列 RMS。

**Composition and asset choice:** Give each channel an aligned before/after pair of plots. Keep time alignment and the amplitude scale fixed within each pair, using the actual source's units. Compare each channel to its own source; do not imply cross-channel amplitude comparability if the source does not provide it. Use native charts from the actual arrays when available. If only source figures are available, retain those images with editable cues and state the editing boundary when relevant. A generated waveform or a decorative background does not serve this evidence page.

| Click stage / object roles | Action | Retained context |
| --- | --- | --- |
| Entry: `trace_native_ch1`, `trace_native_ch5`, axes and identifiers | Show original panels with readable record, channel, and time labels; reserve aligned space for processed panels. | Full window and source scale. |
| First click: `trace_100hz_ch1`, `rms_ch1`, `comparison_ch1` | Reveal the actual processed channel 1 plot, its ratio, and its explanation together. Keep the original panel beside it. | Original samples and corresponding processed time positions. |
| Second click: `trace_100hz_ch5`, `rms_ch5`, `comparison_ch5` | Reveal the channel 5 comparison with the same layout and metric definition. | The complete channel 1 comparison. |
| Optional focus: `roi_band` and `detail_panel` | If a particular source-supported region needs explanation, show its cue and a linked enlargement on the same click. | Matching channel/time identity and original amplitude context. |

Use coordinated Appear/Fade or native chart builds for the actual states. Keep both endpoints available. Do not morph one measured waveform into another: interpolated shapes would introduce samples that are not in either dataset, and native charts are not geometric Morph targets. The explanation concerns relative RMS amplitude change; it does not establish phase correctness or picking accuracy.

**Source note:** Keep the original figure/data reference, window, processing stages, scaling, and metric definition in the existing notes. For current production, inspect the actual supplied material before reusing historical numbers. This page requires no stock-photo search or image generation.

## Monitoring scene and acquisition flow

**Page role and available content:** Introduce a proposed monitoring chain whose supplied design connects a sensor, acquisition unit, and waveform display. This is a conceptual scene with editable relationships. Use the supplied design to determine actual components and connections; a scene illustration does not establish field deployment.

**Title:** 监测信号从传感器进入采集与显示环节

**Visible copy:**

> 传感器把地层振动转换为电信号，采集单元将其数字化，软件按时间组织并显示采样序列。

**Visual decision:** Use a large quiet underground scene to make the setting recognizable, with native sensor, acquisition, display, connectors, and labels layered above it. The scene carries environmental context; the editable chain carries the technical explanation. An actual project photograph is preferable when this page documents a real installation. For an authentic reference, search `井下 微地震 传感器 安装 官方` or `official borehole geophone installation photograph`, open the original page/image, and check suitability and rights. For a proposed design needing a controlled composition, generate a scene directly.

### Slide-specific generation example

This illustrative layout assumes a light template with a navy accent, gray supporting colors, and room for the native chain on the right. Change these choices to match the actual template and layout before generation; do not recolor the whole deck to match the example.

```text
Use case: scientific-educational
Asset type: background illustration for an editable technical PowerPoint slide
Primary request: a calm conceptual cutaway of an underground monitoring environment
Scene/backdrop: two simplified solid-rock layers with a clean ground surface, schematic rather than a geological survey
Style/medium: restrained technical illustration, off-white background, muted blue-gray rock tones, a small navy accent, crisp readable silhouettes
Composition/framing: wide landscape crop; ground cutaway concentrated toward the left and lower part; open quiet area on the right for native slide objects and explanations
Text: no text, no numbers, no labels
Constraints: background environment only; no sensors, cables, acquisition electronics, waveforms, logos, or measured geological details; the monitoring chain will be added as editable PowerPoint objects
Avoid: dramatic disaster imagery, neon glow, decorative circuitry, heavy texture, watermark
```

Use the built-in image tool, inspect the result, and copy the selected scene into the project's existing assets folder, for example `assets/monitoring-scene.png`. This prompt is a production example, not a report that an image has been generated. If a separate movable equipment cutout is actually useful, request that asset separately with true transparency; do not attempt to move an object painted into the background. Keep the sensor and chain native when independent editing is required.

### Layers and dynamic sequence

| Layer / suggested object roles | Entry and action | Explanation and retained context |
| --- | --- | --- |
| `scene_background`, title, “监测链路示意” | Visible on entry, with the template's master, title style, and fixed identity elements. | Establish the setting without claiming an actual deployment. |
| `sensor`, `sensor_label` | Visible initially at the design-supported location. | Identify the origin of the chain. |
| `link_sensor_acquisition`, `acquisition`, `acquisition_label` | On click, show the receiving unit and connector together; use a directional Wipe along the connection where supported. | Keep the sensor and source location visible. |
| `link_acquisition_display`, `display`, `display_label` | On the next click, reveal the next connection and display; a small marker may travel along the visible connector to indicate data flow. | Retain the preceding chain. Marker travel time is illustrative, not measured latency. |
| `chain_explanation` | Reveal its sentence with the completed chain or in meaningful phrases beside the corresponding components. | Leave the completed system readable for discussion. |

Do not place an outgoing flow marker before its destination has appeared. Use an actual screenshot or real data for a project-result display. If a tiny waveform only identifies the display function in this concept page, draw and label it as a schematic. Keep the path, component shapes, captions, and animation targets editable; embed only the environmental illustration. The same approach transfers to other engineering systems by replacing the setting and components from their supplied sources.

## Natural Chinese

Develop the available subject description into useful prose. Some drafts lack information; others contain a valid idea in awkward or overly abstract wording. Improve both substance and expression, preserving technical terms that the audience needs.

| Draft wording | Ready-to-use wording | What improves |
| --- | --- | --- |
| “采样率是重要参数。” | “1000 Hz 对应 1 ms 的采样间隔，100 Hz 对应 10 ms；相邻采样点的间隔扩大到原来的十倍。” | The relationship between sampling rate and interval. |
| “去趋势，改善数据质量。” | “在分析窗内拟合直线，再从原波形中逐点减去这条直线，得到去除线性趋势后的序列。” | The transformation performed on the data. |
| “处理后存在差异。” | “M1-03 的同一窗口内，道 1 与道 5 的 RMS 幅值比分别为 12.8% 和 70.4%；道 1 的相对幅值减弱更明显。” | A specific comparison, with its interval and metric definition beside the figure. |
| “软件提供可视化支持。” | “灰线显示原始波形，蓝线显示处理后波形；候选窗口标出时间范围，点标记标出候选位置。” | How the supplied interface represents the data and candidates. |
| Cover title “造园如作画” for a class about Chen Congzhou and the eastern Yuyuan restoration | Main title “陈从周的园林设计”; subtitle “以豫园东部修复为例”. | Names the person, subject, and case immediately. A poetic phrase is no longer carrying the cover's explanatory task. |
| “画理指导空间的经营” | Heading “借鉴山水画的构图方法”; body “通过主次、疏密和远近层次，安排山石、水面与建筑的位置。” | Replaces an abstract phrase with the actual design operation. |
| “动观与静观：让行走与停留相互配合” | Title “动观与静观：游线和观景点的安排”; body “沿廊行走时，转折与遮挡使景物依次出现；在厅堂和水边停留时，可以细看主景与倒影。” | Keeps the professional concepts and explains what the visitor sees in each situation. |
| “以格局统合具体的要素” | “先确定山、水和建筑的整体布局，再安排游路、桥廊和植物的位置。” | Turns an abstract summary into understandable design steps. |

The sampling and detrending sentences are teaching explanations. The M1-03 values and ratio definition are in the [recorded result example](research-explanation.md#result-interpret-a-matched-comparison). The interface wording follows the historical screenshot case below. The garden rows demonstrate editorial choices for that teaching context; they are not quotations by the designer or evidence that every garden has the described features. Match copy to the actual sources and selected views. These examples do not impose a vocabulary ban or a fixed title pattern.

## Title without a presenter cue

A literature slide has the title “围绕这些问题，我梳理了几类方法” and a smaller gray line beneath it: “先看每篇在解决什么，再联系自己的数据。” The second line describes the speaker's sequence.

Name the comparison directly, for example “几类方法的处理对象与关键步骤” when those are the table's actual columns; use more specific method names when the page provides them. Let the substantive table follow the title. Put the speaker's sequence in notes when useful. A caption such as “27.45–29.45 s” remains beside the waveform because it identifies the data being discussed. Existing titles that already identify the subject clearly can stay.

## Auxiliary small text below an example

A teaching slide already shows $skill-creator and the example request “创建中文技术汇报 Skill：沿用模板，分步讲解，交付可编辑 PPTX。” A separate smaller gray line says “先用真实任务试一次，再按输出补充规则。”

Keep the command and worked request. Omit the extra reminder from the slide, using notes if it helps the speaker. Keep useful instructions beside the actual interface, such as “选择‘老陈技术汇报PPT’，再附上模板和材料。” If revising a Skill is itself the topic, explain that operation in the main body.

## Complete one-slide rewrite

This is a self-contained teaching page about linear detrending. Its small numerical sequence is a constructed calculation, represented on the slide as “线性去趋势算例”.

### Material available to the writer

- Sample indices n = 0, 1, 2, 3.
- Input sequence x = [2, 2, 4, 8].
- An ordinary least-squares straight-line fit x̂[n] = 2n+1, giving fitted values [1, 3, 5, 7].
- Sample-by-sample subtraction y[n] = x[n]−x̂[n], giving y = [1, −1, −1, 1].

These quantities are enough to explain the fitting and subtraction. The page introduces that operation directly.

### Internal explanation plan

For an audience that can read the four sample positions and follow arithmetic, the page's goal is to explain how the residual is produced. Choose the order input points → fitted line and fitted values → sample-by-sample subtraction → residual meaning. Assign the two visible paragraphs below to those operations, with the corresponding quantities beside them. Then arrange the plot, formula, and arithmetic in a suitable existing layout. On a live page, use that same order for its native builds. This planning is part of authoring and leads directly to the finished page.

### Before

**Title:** 波形预处理

**Visible copy:**

- 去趋势，改善数据质量。
- 消除背景影响，为后续处理提供支持。

This names an operation and gives broad benefits. The supplied calculation provides a more useful explanation.

### After

**Title:** 线性去趋势：拟合直线，再逐点相减

**Main visual:** Plot the four input points and fitted line on the same sample-index axis, then relate them to the residual sequence through a subtraction. Use editable lines, markers, formula text, and annotations. Label n as “采样点序号” and amplitude as “幅值（任意单位）”. Keep the template's colors and typography, and place each explanation beside its corresponding quantity.

**Complete visible copy:**

> 在 n=0、1、2、3 四个采样点上，原始序列为 [2, 2, 4, 8]。对它作直线拟合，得到 x̂[n]=2n+1，对应的拟合值为 [1, 3, 5, 7]。
>
> 将原始序列与拟合值逐点相减，得到 [1, −1, −1, 1]。这个差值序列表示原始数据相对拟合直线的起伏。

**Adjacent formula:** y[n] = x[n] − (2n+1)

The visible text explains both operations and the meaning of their output. It finishes with the subject itself.

**Speaking notes:**

> 先看原始点和拟合直线。四个采样位置上的拟合值依次是 1、3、5、7。第一个点用 2 减 1 得到 1，第二个点用 2 减 3 得到 −1，其余位置按同样的方法相减。下方差值序列与原始序列保持一一对应，只是减去了拟合直线。

**Source note:** Teaching calculation defined by the four input values, sample indices, and ordinary least-squares fitting rule above.

### Why the rewrite is useful

The page explains what is fitted, how the subtraction is carried out, and what the residual represents. Its formula, input, intermediate values, and output all refer to the same operation. It supplies technical understanding from the available material without requiring an additional project experiment.

Use this reasoning for other methods: select a key operation from the actual source, make its quantities understandable, and connect the output to that operation. Numerical examples are useful when they clarify the subject; they are not a requirement for every page.

## Software presentation from an existing screenshot

**Historical source:** Slide 8 and its notes in the September 2026 deck “地震波检测研究进展.pptx”, read for the writing example on 2026-10-16. The recorded screenshot contains Event3, a 34.154–34.289 s candidate window, a P candidate at 34.243 s with status “建议”, and gray original/blue processed waveforms.

**Title:** 候选窗口与点标记怎样呈现在波形上

**Main visual:** Use the actual screenshot. Keep the relevant time axis, traces, candidate window, and original status labels legible. Place an editable cue on the window and another on the P candidate, with each explanation nearby.

**Complete visible copy:**

> Event3 的候选窗口为 34.154–34.289 s，34.243 s 处的点标记表示 P 候选位置。窗口对应一段时间范围，点标记对应其中一个时刻。
>
> 灰线显示原始波形，蓝线显示处理后波形。对照同一时段的两条曲线，可以阅读处理前后的波形形态。

**Speaking notes:** Move from the window's two boundaries to the point marker, then use the original color labels to explain the two traces. Follow the source's display scaling when discussing amplitude.

**Source note:** Retain the original slide/screenshot reference and its record identity with the page. The example's numbers and colors belong to that historical screenshot; use the actual source for another interface.

This page introduces the interface's objects and their meanings. A detailed review procedure can be explained on a page whose topic is review.

## Garden teaching page

**Audience and task:** Second-year landscape students learning to connect viewing experience to route and viewpoint design. This is an illustrative teaching page, not a historical reconstruction or an attributed quotation. For a named designer or garden, verify the terminology and site relationships against the actual sources before applying the example.

**Available material for this example:** A clearly identified photograph of a turning corridor beside a garden scene, plus a photograph showing a stationary viewing place in a hall or waterside pavilion. Inspect the views to determine which columns, openings, foreground objects, water, and distant subjects are actually visible. Use a reliable plan if the lesson also needs exact locations or routes.

**Title:** 动观与静观：游线和观景点的安排

**Visible copy:**

> 动观是在行走中看景。沿游廊前进时，观看方向和遮挡关系不断变化，景物随路线依次展开。设计游线时，要考虑转弯前后分别能看到什么。
>
> 静观是在固定位置赏景。人在厅堂、廊角或水边停留，可以细看主景与背景的关系。选择观景点时，要考虑视野是否清楚，以及是否便于停留。

**Composition and assets:** Give the two authentic views enough prominence to compare. Place each short paragraph beside the corresponding view, with a small number of native labels tied to visible features. Preserve the template's type and palette. Use a real corridor photo rather than a crude band of rectangles to explain the experience of walking; when explaining the route's location, use a source-supported plan with an editable route instead of inferring a whole route from one photograph. A generated garden illustration may support a design exercise but cannot establish the historical layout.

| Stage / object roles | Native action | Retained context |
| --- | --- | --- |
| Entry: title, both photographs, essential view identities | Show the subject and views together; a short coordinated entrance is optional here because the following content stages supply the page's animation. | Both views remain available throughout the comparison. |
| Explain moving views: `corridor_cue`, `moving_view_copy` | On click, reveal a cue on a visible opening, turn, or foreground obstruction with the matching paragraph. Add directional motion only if the source actually supports the shown direction. | The corridor view and the second view remain fixed. |
| Explain a fixed viewpoint: `viewpoint_cue`, `fixed_view_copy` | On the next click, reveal the visible viewing position or framed subject with its paragraph. | Retain both explanations for comparison. |

**Speaking notes:** “先看游廊这张照片。沿着路线前进，前景的遮挡和观看方向会变化，所以游线设计要考虑景物出现的次序。再看固定观景点：停在这里时，主要看哪处景物，前面是否有遮挡，能否舒适地停留？动观和静观分别帮助我们判断路线与停留位置怎样安排。” Adjust references to the actual photographs; do not describe features absent from them.

**Authoring decision:** The visible paragraphs already explain the two concepts and their design implications. Notes provide a way to guide attention. Cues and copy enter together, while the source views stay available; the deck needs neither a fabricated map nor a mandatory extra slide. Continue this live-talk default on the cover and closing page: introduce the person/work through a restrained title-and-photo entrance, and reveal the closing design points in meaningful groups. These are production instructions, not a claim that a deck or its playback has been tested.

## Live and reading versions

Use the same linear-detrending teaching material to choose how much explanation stays visible.

**Shared title:** 线性去趋势：拟合直线，再逐点相减

| Intended use | Visible explanation | Role of notes |
| --- | --- | --- |
| Live talk | “对 [2, 2, 4, 8] 拟合直线，得到 [1, 3, 5, 7]；逐点相减后为 [1, −1, −1, 1]，表示原序列相对拟合直线的起伏。” Show the formula beside the plotted operation. | Guide attention from input to fitted line to subtraction; walk through representative values. |
| Standalone reading | Use the two complete paragraphs from the worked page, with the sample indices, formula, and sequences readable beside the diagram. | Retain the calculation's source note and additional arithmetic if useful. |

Both versions keep the actual technical explanation visible. The live page uses native builds by default, with speaking notes supporting its pacing. An explicitly requested standalone-reading version carries the fuller explanation on a coherent static page. Produce the requested format in the existing template; do not create an additional reading deck or remove the live version's animation unless requested.

## Accurate delivery wording

Default, with user-led review:

> 已完成11页完整PPT，备注中附有讲述提示和文献来源。已加入原生点击动画。

Match the count and features to the actual file and provide its usable path. Keep production commentary in the delivery message when relevant.

If the user explicitly requested animation review and playback could not be completed:

> 原生动画已写入，配置已核对；本次实际播放检查未完成。

State a concrete production issue when it affects the requested delivery. Keep implementation, configuration checks, playback, and measured rehearsal distinct.
