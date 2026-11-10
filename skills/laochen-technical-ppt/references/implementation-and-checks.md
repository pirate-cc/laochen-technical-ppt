# Implementation and scoped checks

Read only the needed sections. Reuse project tooling; configure necessary dependencies under existing authorization. Mentioned libraries are examples, not required installations or permission to change the agreed application/format.

## When to use checks

Follow [task scope](../SKILL.md#task-scope): review reports without editing; authorized repair, including current-authoring errors, fixes the issue and repeats affected checks. Cover changed content and necessary dependencies, including shared resources rewritten by the tool; do not repeat completed checks or expand local work into full-deck regression. Rehearsal, specialist accessibility audits, cross-application checks, and edit trials apply only when requested or required by the agreed use. Honor explicit user checkpoints without adding gates.

## Minimum production confirmation

Inspect the saved authoritative output, using saved-object/package inspection plus the relevant renderer/runtime. Apply only the affected rows:

| Affected part | Confirm during production |
| --- | --- |
| Saved output and page structure | Save succeeded without exporter/package errors. Resolve the presentation page list and relationships for count, order and referenced parts; counting `slide*.xml` files does not establish order. |
| Substantive explanation | The visible page explains its operation, relationship, difference or result basis. Necessary definitions, formulas, parameters, conditions and evidence survive layout and remain readable. Trace result claims to their source object, conditions and metric across pages; intermediate improvement is not the task outcome. If only names, vague evaluations or unexplained images remain, develop/reorganize within scope using [content depth](research-explanation.md#choose-content-depth) and [revision diagnosis](research-explanation.md#diagnose-the-explanation-gap), not word/formula quotas. |
| Native content and chart data | Text, tables, labels, units and objects retain promised editing granularity. Changed charts keep series/categories, data references, cached values and embedded workbooks consistent with supplied data, required formulas and source lineage. |
| Consumed assets and fonts | Images/media and required sources are embedded or resolve from saved locations. Confirm actual fonts and delivery dependencies; no silent substitution or temporary-URL-only asset. |
| Layout and visible content | Render changed pages from the saved deck at the intended viewing size; inspect font/fit, clipping, overlap, labels and figure legibility. |
| Titles and auxiliary text | Read each affected title and its next visible line, including covers/closing pages. The title names the topic, operation, answered question or supported finding; learning advice/presenter sequencing belongs in notes. The next line must add necessary information: place inputs, conditions, units and example identity by their objects; remove routine audience/process labels and repetition. Preserve meaningful user copy and necessary page-wide conditions. Apply [information-placement rules](research-explanation.md#audience-facing-qualifications-and-small-text), not punctuation/word blacklists. |
| Animation and interaction | Reconcile planned stages with saved target identities, triggers/order, coverage and intentional duplicates. Play affected sequences in the intended application or compatible runtime; inspect entry, intermediate legibility/order and stable final state. New/remade live decks cover every slide; local work covers affected objects/effect dependencies. `p:timing` or effect counts prove neither coverage nor playback quality. |

### Check status and exceptions

Record one status per applicable check in existing notes; no separate QA report is required:

- **Completed:** state the inspection actually performed. Script success, package structure, an in-memory canvas or effect XML does not establish saved rendering, playback, editing behavior or cross-application compatibility.
- **Explicitly delegated to the user:** identify their stated check scope; ordinary delivery for viewing is not delegation.
- **Unavailable:** name the affected feature, missing capability/runtime and completed verification level. Retain usable work, continue independent steps and deliver with the limitation where possible; do not claim the check passed. Changing required animation/editability, format or count still requires authorization covering that change.

## Choose the working surface

- Choose the destination from the current request, confirmed agreement and applicable user/higher-priority defaults: explicit local PPTX/offline/path requests use a local route; cloud/service requests use that service. Edits stay in the existing document/destination unless conversion or separate output is requested; live PowerPoint work uses the open presentation.
- With no such destination agreement/default, new decks use editable local `.pptx`. Resolve conflicting general-Skill routes (including PPTX-to-Spaces) by instruction priority and user agreements before authoring; apply only the selected route's implementation/checks. Obey its API contract and permissions.
- Before committing, verify template import, original-object editing, chart data and native animation from current interfaces/docs or relevant project evidence. A new master is not imported-template preservation; rebuilding is not original-object editing; a local template does not prove cloud fidelity. Handle unsupported operations through [check status](#check-status-and-exceptions).
- Use Template Creator only when a reusable template is requested.

Use supplied template proportions or venue/display requirements; otherwise choose an appropriate format. Estimate timing from explanation complexity, builds, pauses and transitions, not equal time per slide. Rehearsal and manual advance follow [animation review](#requested-animation-review).

## Working without a template

| Situation | Action |
| --- | --- |
| Required template fidelity but no actual file | Obtain the file before final production; continue independent source/content work. Verbal descriptions cannot establish fidelity. |
| Local revision or reusable confirmed complete visual design | Keep that visual language; no new style/template search. |
| New/remade deck without template or complete design | Follow [template selection](template-selection.md) using representative content pages and the user's direction. Prefer a suitable editable template. |
| Explicit original design or no suitable accessible candidate | Establish font family/hierarchy, palette/semantic colors, spacing, title/body relationships, image treatment and annotations from topic, audience, format and use. Existing notes or the first page suffice; adapt compositions within this coherent language. |

For a remaining design gap use [reference selection](asset-sources.md#content-methods-and-complete-talk-examples) and [adaptation](asset-sources.md#adapt-design-references). Apply the chosen tool's relevant template flow after resolving user instructions: direct-design instructions may select a different branch, but do not bypass an actual API requirement or change destination to obtain a picker. If the tool supports continuing after unavailable/cancelled selection, proceed as a new design, not preservation of an unseen template. Do not add outline/sample approval gates.

## Template and object editing

- Preserve master/layout relationships and original objects in scope. Identify targets by stable name, role or identity. Retain paragraph/run properties, indentation, bullets, links, emphasis and theme inheritance; if replacement rebuilds the text body, explicitly restore formatting and confirm the saved result.
- Editability means the promised operation: text changes, table-cell edits, label/connector adjustment or chart-data edits. Photos need not be vectors; screenshots cannot substitute for required editable diagrams. For supplied scientific figures retain agreed data/plot sources and state the editing boundary; do not rasterize required native objects without agreement.
- Chart/data consistency is defined in the production table. A visible chart or embedded workbook alone does not prove agreement; application inspection/edit trials apply when in scope.

Source examples inspected on 2026-10-15, not runtime certification: [PptxGenJS README](https://github.com/gitbrent/PptxGenJS/blob/3c9ec1b687c174952166f6a34b5e87ebf69fa469/README.md) documents generation and custom masters; [python-pptx TextFrame.text](https://github.com/scanny/python-pptx/blob/278b47b1dedd5b46ee84c286e77cdfb0bf4594be/src/pptx/text/text.py#L172-L178) clears and rebuilds paragraphs; [Chart.replace_data](https://github.com/scanny/python-pptx/blob/278b47b1dedd5b46ee84c286e77cdfb0bf4594be/src/pptx/chart/chart.py) updates both chart XML and the embedded workbook. These examples illustrate what to check, not a requirement to use those libraries.

Duplicate suitable template pages while retaining background, master, typography, footer, logo and proportions. Fit content through composition before shrinking type. For code explanations show relevant lines with their explanation nearby.

## Chinese text fitting and fonts

Reuse [deck parameters](layout-and-style.md#establish-reusable-deck-parameters) for matching roles; consistency is not proof of fit.

| Concern | Implementation/check |
| --- | --- |
| Actual text metrics | Use the actual Chinese, Latin and mathematical fonts, box dimensions, margins and spacing. Check missing glyphs/fallback, line-boundary punctuation, subscripts/superscripts, symbols and number/unit pairs. English word estimators are provisional for Chinese. |
| Meaning and notation | Keep meaningful title phrases together across line breaks. Follow source/field conventions for variables, descriptive subscripts, units and vectors/matrices; symbols must denote the same quantities in prose, figures and formulas. Required editable formulas need a supported representation and rendered check, not an image. |
| Overflow | Preserve readable hierarchy; edit meaningfully or recompose within agreed count before shrinking. Judge actual projection/reading use, not universal point sizes, lines or character quotas. |
| Changed layout | Recheck affected saved rendering after grouping, font replacement or conversion; text-fit properties do not establish final fit. |
| Portable fonts | Confirm target availability. Embed only if application and license permit; balance file size and later edits. Character subsets can prevent added text, while full-character embedding may support it. Do not conceal missing fonts by outlining/rasterizing; propose material style-changing substitutions. |
| Agreed PDF output | Create and inspect it within scope; it neither replaces the editable deck nor certifies animation. |

Version-specific examples: [PptxGenJS fit notes](https://github.com/gitbrent/PptxGenJS/blob/3c9ec1b687c174952166f6a34b5e87ebf69fa469/src/core-interfaces.ts#L1007-L1010) explain that shrink/resize behavior is triggered by editing text or resizing shapes; [python-pptx _LineSource](https://github.com/scanny/python-pptx/blob/278b47b1dedd5b46ee84c286e77cdfb0bf4594be/src/pptx/text/layout.py#L237-L248) splits candidate lines by whitespace-delimited words. Verify the selected tool/version rather than generalizing these limitations. [Microsoft font embedding guidance](https://support.microsoft.com/en-us/office/fonts/benefits-of-embedding-custom-fonts) covers character subsets, licensing, and editing implications.

## Scientific charts

- Choose comparison, trend, distribution or relationship from the question. Preserve values, baselines, units, transformations and time/event order; avoid misleading axes, unsupported continuity and meaning-changing decoration.
- Encode categories, ordered magnitude, reference-centered deviations or emphasis appropriately. Keep identities consistent across slides and respect field conventions; retain needed colorbars/references. Use direct labels for a few series, legends for dense/shared encodings, and place conditions near evidence without masking it.
- Define uncertainty marks (SD, SE, specified confidence/credible interval or source-defined measure), sample size and repetition unit where relevant; do not invent intervals or exchange definitions.
- Inspect paper-figure labels at intended size. If unreadable, enlarge relevant panels, pair overview/detail or redraw from available source data; retain controls, axes, units, color scales and qualifications. Do not infer numbers from a picture merely to produce an editable chart.
- For simulation views, adjust background, view, legend and unnecessary UI while preserving variable, units, scale/colors, case identity and relevant geometry. Mesh visibility follows its evidential role, including discretization/contact/reliability. Align comparative views/scales/crops without changing results.

References: [Wilke on color scales](https://clauswilke.com/dataviz/color-basics.html), [time-series labels](https://clauswilke.com/dataviz/time-series.html), and [uncertainty](https://clauswilke.com/dataviz/visualizing-uncertainty.html). [Nature figure guidance](https://research-figure-guide.nature.com/figures/building-and-exporting-figure-panels/) concerns publication figures; do not import its print-size typography as a slide font prescription.

## Accessibility

- For distributed/teaching/reading decks, retain meaningful titles, argument-based reading order, concise informative alt text and decorative-object marking. Avoid duplicating nearby text or narrating decorative arrows. Follow [grouping rules](#progressive-explanation-and-animation), not unnecessary regrouping to clear checker warnings.
- During a requested accessibility review, inspect body text, informative lines/markers, selections and callouts, including text over images. Use text/shape/pattern/position as well as color for categories; numerical contrast alone does not make thin projected lines legible. Run the available application checker, inspect its gaps and record the version/features; coverage varies.
- WCAG informs, but does not certify, PPT: 4.5:1 ordinary text, 3:1 large text under the standard's definition, and 3:1 necessary non-text graphics with its exceptions. Also assess actual Chinese glyph size and viewing conditions.

References: [Microsoft accessible presentations](https://support.microsoft.com/en-us/accessibility/powerpoint/make-your-powerpoint-presentations-accessible-to-people-with-disabilities), [reading order and grouping warning](https://support.microsoft.com/en-us/powerpoint/make-slides-easier-to-read-by-using-the-reading-order-pane), [W3C text contrast](https://www.w3.org/WAI/WCAG22/Understanding/contrast-minimum), and [non-text contrast](https://www.w3.org/WAI/WCAG22/Understanding/non-text-contrast). Microsoft's [2026-04-02 update](https://techcommunity.microsoft.com/blog/microsoft365insiderblog/better-contrast-checking-for-slides-in-powerpoint/4504713) describes a staged rollout of transparency-aware text checking and remaining table/native-chart limitations. Check the target version and actual feature availability instead of treating that announcement as proof of local capability.

## Progressive explanation and animation

- **Scope:** new/remade live-talk decks need meaningful native animation on every slide, including covers, section transitions, simple conclusions and closing slides. Simple pages may use one coordinated entrance/emphasis; complexity determines stages, not a click quota or a requirement to move every object. Static/print/standalone-reading pages follow their use. Local edits preserve unrelated effects; added pages follow their own use.
- **Semantic stages:** establish complete content first, then coordinate each explanation/visual target with its cue, connector and text. Title/decoration-only movement does not build a content page; generic slide transitions are not within-slide actions. Do not split by picture/text, left/right position or individual text boxes. Keep related evidence visible for comparison; separate entrances need not become separate pages. See [multi-model comparison](worked-examples.md#comparing-related-models-on-one-slide).
- **Method chains:** normally reveal a downstream step, incoming arrow and explanation on the same click; keep prior steps visible and reveal the source before its dependency. No arrow into an unexplained empty area or full-chain entrance when sequential build is requested. See [method-chain example](research-explanation.md#cumulative-method-chain).
- **Dense evidence:** begin with a stable overview retaining identity, axes, units and labels. Reveal/emphasize each region cue and explanation together. Choose arrows, boxes, interval bands, brackets, direct labels or linked enlargements by geometry; preserve panel/record identity and time/spatial correspondence. Retain comparison context but remove obsolete cues that obscure evidence. See [evidence location](research-explanation.md#locating-evidence-during-explanation) and [data comparison](worked-examples.md#comparison-with-supplied-data).
- **Before asset production:** use the [effect table](#choose-the-effect-from-the-explanation) to identify moving/changing objects, fixed references, separate layers, pivots/anchors and source-supported states; feed these into [sourcing](asset-sources.md#scene-to-material). Appear/Fade suffices for labels/builds; taught motion or state change must occur in the actual subject.
- **Plan and group:** in existing notes keep each created/remade page's action; one sentence suffices for a simple entrance. For complex pages associate observations, evidence targets, cues, clicks and retained context. Set necessary groups/reading order before animation: regrouping may discard effects and reordering may alter overlap. Confirm affected targets/sequencing afterward; coordinated effects can replace a native group. Local changes update only affected entries.
- **Write the effects:** notes are not native animation. Write effects into the delivered PPTX through the supported API below; do not assume export preserves them. Keep clicks under presenter control with stable reading states. About 0.3–0.5 s is only a simple-fade starting point; avoid gratuitous motion, letter/word fragmentation and unrequested automatic slide advance.
- **Fallback:** use [check status](#check-status-and-exceptions) for unavailable implementation/playback or explicit user review. Only if the request permits static fallback and its page count, use clearly identified cumulative step pages retaining prior content. Otherwise keep the agreed count and identify the unsupported feature; no silent static-as-animated delivery, video-for-editable substitution or duplicate pages to change count.

## Native animation

Use stable object identities/semantic roles. For complex builds record in existing notes:
`role/name -> effect/path/start-end geometry -> trigger -> order -> duration/delay/repeat -> entry/final visibility`.
Simple stages need no separate schema. Set these actual properties through the supported animation API. In authorized Windows PowerPoint automation, `TimeLine.MainSequence.AddEffect` is one route; inspect main and interactive sequences where relevant. Deliberately set click/with-previous/after-previous: one click can run coordinated effects, but the next substantive stage remains presenter-controlled. Derive duration from the action.

### Choose the effect from the explanation

| Meaning | Native construction and invariant |
| --- | --- |
| Cover, section transition, conclusion/closing | Restrained coordinated title/main-visual entrance or concluding emphasis; leave the complete subject readable. |
| Photo, concept or short explanation | Reveal/emphasize the actual subject's cue and matching sentence together, as one semantic group when further splitting adds nothing. |
| Component, dependency or observation | Appear/Fade with its incoming arrow, cue and text; keep prior dependencies visible. |
| Interface/process state change | Reveal, emphasize or replace affected native controls/state, or align authentic screenshots with native cues. Preserve unchanged context and supported trigger/result; do not invent later success, approval or operation. |
| Flow along a path | Directional Wipe on a connector, optionally followed by native marker motion. Match path/direction and show destination before arrival; movement does not imply measured transit time without a source. |
| Vibration/recurring mechanism | Native motion path or rotation about a fixed reference such as equilibrium; use a short coordinated sequence ending stably. Label fades cannot replace the taught movement. |
| Overall object and detail | Native enlargement plus source-region emphasis, or Morph across already planned adjacent pages. Preserve overview/detail identity and readable context. |
| Two measured/before-after states | Aligned source charts/panels with reveal/state switching; fix comparative axes/units and use actual endpoints, not invented interpolated observations. |
| Designed spatial/structural change | Native position/size/rotation or Morph across planned pages; consistent object identity and explainable start/end geometry within agreed count. |

Optional [product](worked-examples.md#product-introduction-with-editable-motion), [procedure](worked-examples.md#procedure-training-with-native-interface-states) and [scene](worked-examples.md#conceptual-scene-with-separate-layers) examples illustrate roles; transfer relationships, not their subjects or numbers.

**Morph:** match corresponding objects across planned adjacent pages; explicit matches use the same unique `!!`-prefixed name. Set differing position/size/rotation and the native transition, not just a note. Charts do not geometrically morph; use actual chart states/panels. See [Microsoft Morph guidance](https://support.microsoft.com/en-us/powerpoint/morph-transition-tips-and-tricks).

**Optional media:** [Manim](https://github.com/ManimCommunity/manim) or another deterministic renderer may explain a dense continuous mechanism when media fits the agreed output. Define equations/parameters, retain source, embed the clip and keep required text/annotations/relationships native. Internal particles/curves remain noneditable in PowerPoint. Prefer native effects when sufficient; no routine-animation framework installation or clip substitution for required editable motion.

### Requested animation review

Apply the production table's animation check to requested reviews and affected new/changed sequences, including duration/delay and entry/exit behavior. Repairs or re-export repeat affected checks under the same [status rules](#check-status-and-exceptions).

Rehearse only when requested; preserve speaker control unless automatic advance is requested. [Rehearse Timings](https://support.microsoft.com/en-us/powerpoint/training/rehearse-and-time-the-delivery-of-a-presentation) can record timing; afterward confirm manual advance where needed. Planned duration, automated playback checking and actual spoken rehearsal are distinct.

References: [Microsoft AddEffect](https://learn.microsoft.com/en-us/office/vba/api/powerpoint.sequence.addeffect), [BrightCarbon on pacing](https://www.brightcarbon.com/blog/how-to-be-a-powerpoint-animation-ninja-in-7-easy-steps/), and [PowerPointLabs AnimateInSlide](https://github.com/PowerPointLabs/PowerPointLabs/blob/79e6be4882b736a0cb4828e06a96286de9b3aed6/PowerPointLabs/PowerPointLabs/AnimationLab/AnimateInSlide.cs). The latter includes deletion of existing effects on selected objects; do not copy that behavior into a preservation-focused local edit. Its [test comparison helper](https://github.com/PowerPointLabs/PowerPointLabs/blob/79e6be4882b736a0cb4828e06a96286de9b3aed6/PowerPointLabs/Test/Util/SlideUtil.cs) illustrates separate content/image/animation checks, but does not compare every animation property. These source examples do not replace the playback evidence required by the production table.

## Portable delivery and scoped regression

For requested edit/portability trials, use a temporary copy of the saved deck and test embedded chart data, image/media links and offline dependencies in only the agreed applications/environments. Preserve the authoritative file unless repairing within scope, then remove the disposable copy.

For regression, compare changed content and dependencies with the pre-edit baseline; inspect untouched pages/effects proportionately when tools rewrite shared resources or whole packages. Changed hashes do not establish slide regressions; identical images do not establish unchanged animation. Keep findings/repair evidence in existing QA notes.

## Delivery and optional review

Deliver one authoritative result and agreed sources with actual changes, location, verification and material font/media dependencies. Report missing checks by [status](#check-status-and-exceptions); do not add unrelated checklists, approval gates or unrequested alternate decks/PDFs/reports.

A review delivers located findings and suggestions; authorized repair also identifies actual corrections and remaining issues. Distinguish content/source inspection, static rendering, native-object/data inspection, playback, and rehearsal, then stop at the agreed scope. See the [task-boundary cases](worked-examples.md#task-boundary-cases) for scoped review, local edits, and direct delivery.
