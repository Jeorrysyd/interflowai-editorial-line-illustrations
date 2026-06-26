---
name: interflowai-editorial-line-illustrations
description: Generate Chinese article illustrations in a white-background American editorial line-art style. Use when users ask for WeChat/Xiaohongshu/article spot illustrations, essay visuals, event recap illustrations, product note visuals, methodology diagrams, image shot lists, prompt writing, "小黑配图二创", "互通有无配色", InterflowAI branded visuals, or image QA that should preserve Xiaohei-style conceptual explanation while replacing the mascot with simple human line figures, sparse text, brand color blocks, corner bylines, and abstract geometric identity elements.
---

# InterflowAI Editorial Line Illustrations

## Core Positioning

Create article illustrations that explain Chinese writing through simple human figures, object metaphors, color blocks, and sparse annotations.

This is a general article-illustration skill. It can be used for WeChat articles, Xiaohongshu notes, event recaps, product opinions, course notes, methodology writing, workflow documents, and founder essays. It is not limited to AI topics or InterflowAI projects.

The default visual preset uses InterflowAI / 互通有无 colors and a small optional byline, but users may replace the palette, signature, and theme with their own brand.

This skill is a second-creation inspired by the "小黑配图" method: keep the analysis habit of finding the article's cognitive anchors and turning abstract ideas into physical actions. Do not keep the 小黑 IP by default. The default character is a simple hand-drawn human in an American editorial/productivity spot-illustration language.

## Read References As Needed

- `references/article-analysis.md`: how to turn an article into illustration anchors and shot lists.
- `references/style-dna.md`: visual rules for white background, black line, brand color blocks, text use, and prohibitions.
- `references/interflow-brand.md`: InterflowAI default palette, recurring IP-feeling visual devices, and signature/byline rules.
- `references/prompt-template.md`: prompt templates for one image, cover image, and text-on-image versions.
- `references/qa-checklist.md`: checks and iteration rules after generation.

## Workflow

### 1. Digest The Article

Read the user-provided article, outline, Feishu/Notion content, Markdown, screenshots, or notes. Extract:

- the central claim
- where the reader needs help understanding
- the real tension, not just the positive point
- the best paragraph anchors for images
- whether the platform is WeChat, Xiaohongshu, Feishu, slide, or long article

Do not average one image per section. Pick cognitive anchors where an image can make the article clearer or warmer.

### 2. Produce A Shot List First When Needed

If the user asks "怎么配图", "分析一下", or has not explicitly asked to generate, produce a short shot list. Each item should include:

- placement after which paragraph or section
- image theme
- core idea
- human action
- key object metaphor
- suggested short labels, if any
- format: 16:9, 3:4, 1:1, or grid

Default to 4-8 images for a long article, 1-3 for a short post. Use fewer images when each one carries a clear role.

### 3. Generate One Image At A Time

If the user explicitly asks to "生成", "做图", "输出图片", or "直接做", use `image_gen` for each image separately. Do not combine all images into one sheet unless the user asks for a grid.

Each image should explain one idea through one human-object relationship:

- a person holding, sorting, repairing, carrying, feeding, folding, pulling, or matching objects
- object metaphors such as forms, cards, folders, clocks, phones, boxes, doors, cables, tiny machines, stamps, envelopes, calendar pages, and messy note piles
- sparse labels only when labels make the article easier to understand

### 4. Save And Handoff

When working in a local workspace, save final images under:

```text
assets/<article-slug>-illustrations/
```

Use ordered names:

```text
01-cover.png
02-why-they-came.png
03-useful-thread.png
```

Also save final prompts in the same folder when the user is building a reusable article package.

### 5. QA And Iterate

After generation, inspect every image against `references/qa-checklist.md`. Regenerate or edit when:

- the background is not pure white
- there are too many characters for the intended single-person scene
- it looks like a PPT infographic, corporate vector illustration, or cute mascot poster
- the text is wrong, too long, or used as a headline in a正文 image
- it copies the supplied reference image's exact layout, marks, brand, or composition

## Output Style

Keep the user-facing explanation short. For final handoff include:

- what was created
- where the files are saved
- which visual direction was used
- any remaining risk, such as text legibility or images needing manual review before publishing

Do not write a long style essay unless the user asks for one.
