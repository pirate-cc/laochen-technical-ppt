# 老陈技术汇报 PPT

面向中文技术汇报、教学、产品介绍、操作培训、文化叙事等场景的 Codex Skill。依据听众和用途选择讲解、素材与动态；沿用模板或建立一致的视觉方向，交付文案自然、视觉贴合主题、保留原生编辑能力的 PowerPoint。

**当前版本：0.1.18 · 作者：老陈 · [MIT License](LICENSE)**

English: A reusable Chinese presentation skill for Codex, covering scene-based sourcing, natural copy, template preservation or coherent original design, editable objects, and native slide animation.

## 能做什么

- **新建或整体重做：** 从场景和观众目标安排讲解，依据实际素材共同修订文案、视觉与原生动态；讲演稿默认每页都有服务内容的对象动画。
- **局部修改：** 只修改指定页面、对象及必要依赖，保留无关内容、格式与动画。
- **审阅、解释或诊断：** 默认只检查和报告；用户明确授权后才修改文件。
- **文案、提纲或素材：** 只交付所需内容；静态、打印或阅读稿按相应用途处理。

完整规则见 [SKILL.md](skills/laochen-technical-ppt/SKILL.md)，具体写法与协作示例见 [worked-examples.md](skills/laochen-technical-ppt/references/worked-examples.md)。

## 0.1.18 素材网站索引

- 新增 SVG Repo、Storyset、PresentationGO、LottieFiles、NASA SVS、Smithsonian Open Access、Our World in Data 和 Poly Haven 八个入口，按适用场景、素材格式与使用条件整理。
- 从矢量对象、场景插画、PPT 组件、动态参考、科学可视化、馆藏实物、公共数据和三维素材中按需选择；保留已有来源和复用途径，网站名单不限制继续发现合适原件。
- 明确署名、条目许可、公开再分发和账户条件，区分矢量/三维源文件、媒体动画与 PPT 原生对象，不把下载格式视为可编辑性或动画实现的保证。

具体入口见 [素材网站索引](skills/laochen-technical-ppt/references/asset-sources.md#additional-asset-libraries)。本版沿用按场景选材、图文共同修订和无模板时建立一致视觉方向的流程，保留自然中文成稿、讲演版逐页原生动态、原生可编辑要求，以及完成必要制作核对后直接交付用户自行检查的方式。Skill 只提供链接和使用方法，不打包第三方素材。

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
│       ├── asset-sources.md          # 主题视觉与素材来源
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
