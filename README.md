# InterflowAI Editorial Line Illustrations

> 《互通有无美式线条正文配图》
>
> Turn Chinese articles, essays, event recaps, product notes, course notes, and methodology writing into white-background editorial line illustrations.
>
> 中文正文配图 | 美式线条人物 | 文章认知锚点 | 品牌色块 | Codex Skill

---

## 这个仓库是什么

InterflowAI Editorial Line Illustrations 是一个 Codex Skill，用来为中文文章生成正文配图方案、shot list 和图像提示词。

它不是通用插画 prompt，也不是 PPT 信息图模板。它的核心目标是：先理解文章里的认知锚点，再把一个判断、问题、流程、关系或情绪，变成一张有人物动作、有物件隐喻、有留白的 editorial 插画。

它可以用于 AI 文章，但不只服务 AI 内容。更通用的使用场景包括：

- 公众号长文
- 小红书图文
- 活动复盘报道
- 产品观点文章
- 方法论 / 框架文章
- 课程笔记 / 学习总结
- 工作流说明
- 创业复盘 / 团队复盘
- 品牌内容 / 社群内容

默认视觉预设使用 InterflowAI / 互通有无 的品牌配色，但你可以替换成自己的品牌色、署名和文章主题。

一句话：**让 AI 不只是“配一张好看的图”，而是把文章里真正需要被理解的东西画出来。**

---

## 和小黑 Skill 的关系

这个项目是受 Ian 的 [Ian Xiaohei Illustrations](https://github.com/helloianneo/ian-xiaohei-illustrations) 启发做出的二创。

感谢 Ian 和小黑 Skill 提供的核心方法：

- 先找文章里的认知锚点，而不是平均配图；
- 把抽象概念变成物理动作；
- 让角色参与系统，而不是站在旁边装饰；
- 用怪诞但成立的隐喻，让文章更好理解。

不同的是，本 Skill 默认不使用“小黑”这个角色 IP，也不复制小黑示例图构图。

它保留的是“小黑式解释力”，并把这套方法迁移到更通用的 editorial line-art 视觉系统里：人物、色块、署名、品牌色和文章场景都可以替换。

---

## 适合谁用

特别适合：

- 写中文文章，需要正文配图和文章插图的人
- 做知识型内容、方法论内容、活动复盘的人
- 想把抽象观点画成具体隐喻的人
- 想要一种比 PPT 信息图更轻、更有人味的配图风格的人
- 用 Codex 做内容生产，希望稳定复用一套视觉语言的人

不适合：

- 想要商业 KV 或完整品牌海报的人
- 想要传统 PPT 信息图、复杂架构图或流程图的人
- 想要儿童卡通、可爱 IP、表情包风格的人
- 想把大量正文、长段解释或完整课程页塞进一张图里的人
- 需要严格可编辑矢量源文件的人

---

## 它会产出什么

默认输出：

- 一篇文章的 4-8 张 shot list
- 每张图的放置位置、主题、核心意思、人物动作、物件隐喻和中文标注建议
- 单张图片提示词
- 16:9 横版正文配图
- 可选：InterflowAI 品牌色块和角落小署名

默认不输出：

- PPTX / PDF / Keynote
- SVG / HTML / Canvas 可编辑图
- 商业海报或封面 KV
- 大段文字型信息图
- 一键发布链路

---

## 视觉风格

默认视觉系统：

- 纯白背景
- 黑色 / 深蓝线条人物
- 人物动作夸张、修长、有一点失衡感
- 大量留白
- 一张图只表达一个核心动作、结构、状态或隐喻
- 少量中文旁注
- 可选角落小署名：`互通有无` / `Interflow`

InterflowAI 默认配色：

- Blue `#0070DB`
- Orange `#FF5A00`
- Yellow `#FFD200`
- Mint `#00E9A6`
- Pink `#FF978E`

这些颜色是默认 preset，不是使用限制。你可以在 prompt 里替换成自己的品牌色。

---

## 示例效果

### InterflowAI handoff

![InterflowAI handoff](examples/images/01-interflow-handoff.png)

这张图用于示范默认 InterflowAI 视觉 preset：白底、美式线条人物、品牌色块、问题 / 案例 / 匹配 / 下一次的内容资产隐喻。

更多可复制 prompt 见 [examples/prompts.md](examples/prompts.md)。

---

## 安装

克隆仓库：

```bash
git clone https://github.com/Jeorrysyd/interflowai-editorial-line-illustrations.git
cd interflowai-editorial-line-illustrations
```

复制 skill 到 Codex skills 目录：

```bash
mkdir -p "${CODEX_HOME:-$HOME/.codex}/skills"
cp -R ./interflowai-editorial-line-illustrations "${CODEX_HOME:-$HOME/.codex}/skills/"
```

安装后，在 Codex 里使用：

```text
Use $interflowai-editorial-line-illustrations 给这篇文章做一组白底美式线条正文配图。
```

---

## 怎么用

### 只做配图规划

```text
Use $interflowai-editorial-line-illustrations

先不要生成图片。请分析下面这篇文章哪里值得配图，输出 5 张左右的 shot list。
每张图写清楚：放在哪段后、主题、核心意思、人物动作、物件隐喻、建议中文标注词。

<粘贴文章>
```

### 直接生成正文配图

```text
Use $interflowai-editorial-line-illustrations

把下面这篇文章生成 4 张白底美式线条正文配图。
要求：16:9 横版、黑色线条人物、少量中文旁注、动作可以夸张一点。

<粘贴文章>
```

### 使用 InterflowAI 默认品牌 preset

```text
Use $interflowai-editorial-line-illustrations

按互通有无 IP 配色，给这篇文章做 1 张封面 + 5 张正文插画。
风格：白底、美式线条人物、Interflow Blue 为主，橙 / 黄 / 绿 / 粉做几何点缀。
正文图角落加很小的署名「互通有无」，不要直接贴 logo。

<粘贴文章>
```

### 替换成自己的品牌色

```text
Use $interflowai-editorial-line-illustrations

给下面这篇产品文章做正文配图，但不要使用 InterflowAI 配色。
改用我的品牌色：主色 #2F6BFF，辅助色 #F7B500、#26C281。

<粘贴文章>
```

---

## 工作流程

这个 skill 的流程是：

1. 读取文章、Markdown、截图、会议纪要或用户给的主题。
2. 提炼核心观点、认知转折、流程结构和适合视觉化的段落。
3. 先输出 shot list：每张图只选一个认知锚点。
4. 把抽象概念换成一个物理动作：抱、递、接、筛、折叠、匹配、搬运、连接。
5. 用普通物件承载复杂关系：卡片、文件夹、电脑、门、日历、箱子、线团、便签。
6. 让线条人物承担核心动作。
7. 按风格规则生成或改写单张图提示词。
8. 用 QA checklist 检查：白底、留白、非 PPT 感、文字不密、品牌色不乱用、不复刻参考图。

---

## 目录结构

```text
.
├── README.md
├── LICENSE
├── NOTICE.md
├── examples/
│   ├── prompts.md
│   ├── images/
│   │   └── 01-interflow-handoff.png
│   └── outputs/
│       └── generic-shot-list.md
└── interflowai-editorial-line-illustrations/
    ├── SKILL.md
    ├── agents/
    │   └── openai.yaml
    └── references/
        ├── article-analysis.md
        ├── style-dna.md
        ├── interflow-brand.md
        ├── prompt-template.md
        └── qa-checklist.md
```

真正需要安装到 Codex 的是子目录：

```text
interflowai-editorial-line-illustrations/
```

根目录的 README、LICENSE、NOTICE 和 examples 是 GitHub 分享文档。

---

## 测试记录

这个 skill 已通过：

- `quick_validate.py` 基础校验。
- 本地 Codex 生成测试。
- InterflowAI 默认品牌 preset 样图测试。

它不依赖特定平台。只要模型能读取 `SKILL.md` 和 `references/`，就可以复刻“先找认知锚点，再生成正文配图”的流程。

---

## 注意事项

- 图片里的中文文字越短越稳定。
- 每张图只讲一个核心结构，不要把文章做成说明书。
- 示例图只用于风格校准，不是构图模板。
- 不要上传真实会议纪要、内部链接、未脱敏客户信息或未授权参考图。
- 如果使用 InterflowAI preset，可以放小署名，但不要直接贴 logo 或做大水印。
- AI 图像模型可能出现错字、幻觉标签、风格漂移或多余标题，生成后需要检查。

---

## 关于作者

**Joyce / InterflowAI / 互通有无**

Joyce 正在把 InterflowAI / 互通有无做成一个 founder-led AI implementation brand：通过内容、直播、demo、工作坊和 AI 诊断，把真实业务现场转化成可复用的案例、内容资产和商业解决方案。

- GitHub: [Jeorrysyd](https://github.com/Jeorrysyd)
- 小红书 / 视频号: `J在后台`
- 微信: `joycedann`

---

## 继续探索

这套正文配图 Skill，是 InterflowAI 内容生产系统里的一个小工具。

如果你也在尝试把真实经验、活动现场、产品判断或方法论内容，变成更好读、更有记忆点的图文资产，可以关注 InterflowAI / 互通有无。

我们会持续公开构建：内容工作流、AI 辅助写作、活动复盘、品牌内容资产和可复用的 Codex Skills。

想交流可以加微信：`joycedann`，备注「配图」。

---

## License

MIT License. See [LICENSE](LICENSE).
