# Prompt Templates

## Standalone Article Illustration

```text
Generate one standalone {aspect_ratio} Chinese body spot illustration for an article.

Visual style:
Pure white background. Clean black/deep navy hand-drawn editorial line art, slightly imperfect ink lines, lots of blank space, simple elongated human figure with long legs, small head, minimal face, and oversized expressive hands. Contemporary American editorial / SaaS blog spot illustration feeling: witty, mature, energetic, concise, not cute, not corporate vector, not PPT infographic. Use Interflow brand color blocks with restraint: primary blue #0070DB, orange #FF5A00, yellow #FFD200, mint #00E9A6, pink #FF978E. Use blue on one key object or clothing area; use orange/yellow/mint/pink as a few peripheral rhythm marks. Color should create hierarchy and IP recognition while preserving a clean white background.

Theme:
{theme}

Core idea:
{core_idea}

Composition:
{one main human figure}. The person is {physical_action} with {object_metaphor}. Make the action exaggerated but readable: leaning, reaching, floating, balancing, stretching, handing, sorting, or carrying something oversized. The object relationship should explain the idea without needing a diagram. Keep the scene airy and readable.

Suggested objects:
{object_1} / {object_2} / {object_3}

Interflow brand layer:
Add 2-4 abstract geometric accents in the Interflow palette: orange partial blob, yellow circle, mint dot, pink rounded block, blue card. They should support movement and identity, not become random confetti.

Signature:
When a byline/signature is requested, add one tiny corner signature: "互通有无" or "Interflow". Place it bottom-right or bottom-left, in simple black/deep navy text. It must be much smaller than labels and must not look like a logo, watermark, or title.

Optional Chinese labels:
{label_1} / {label_2} / {label_3}

Constraints:
Use pure white background. Keep one main human figure unless the idea requires a handoff or matching scene; then use at most two figures. Use 3-5 core objects maximum. Use at most four short Chinese labels, and no label should be longer than six Chinese characters. Do not add a title, headline, top banner, slogan, or large text. Do not draw 小黑. Do not recreate or distort the Interflow logo unless explicitly requested. Do not copy any reference image composition, brand logo, watermark, or exact character. A tiny corner signature is allowed only when requested. Do not make a flowchart, slide, dashboard, course graphic, dense explainer, complex workflow mega-diagram, messy childlike doodle, or polished corporate vector illustration. Avoid paragraphs of text. Preserve at least 45% blank white space. Use Interflow color blocks visibly but only on subject/object/accent areas, never as full background. Make the metaphor clear, a little absurd, and suitable as a WeChat/Xiaohongshu article body illustration.
```

## Cover With Title

Use only when the user explicitly asks for a cover, title image, poster, or opening image.

```text
Generate one {aspect_ratio} Chinese article cover illustration.

Visual style:
Pure white background, clean black/deep navy editorial line art, simple elongated human figure with long legs, minimal face, and expressive oversized hands, contemporary American editorial magazine spot illustration, Interflow brand color blocks: primary blue #0070DB plus orange #FF5A00, yellow #FFD200, mint #00E9A6, pink #FF978E, large whitespace.

Title:
{title_lines}

Typography:
Use large clean Chinese title text, readable, elegant, not commercial-poster-like. Keep the title separate from the illustration.

Composition:
{cover_scene}

Constraints:
One main human figure. White background. No watermark, no copied reference layout. Use Interflow palette for IP feeling, but do not recreate the logo unless explicitly requested. Do not make it a generic marketing poster. Keep it editorial, energetic, and intelligent.
```

## Text-On-Image Explainer

Use only when the user explicitly wants more text directly on the image.

```text
Generate one standalone {aspect_ratio} Chinese article explainer illustration.

Visual style:
Pure white background, clean black/deep navy American editorial line art, simple elongated human figure with long legs, small head, minimal face, oversized expressive hands, generous whitespace, medium Interflow brand color blocks on key objects, clothing, and abstract accents: blue #0070DB, orange #FF5A00, yellow #FFD200, mint #00E9A6, pink #FF978E.

Core idea:
{core_idea}

Scene:
{one main human figure} is {physical_action} with {object_metaphor}.

On-image Chinese text:
Use one short headline: "{short_headline}"
Use 3-5 small handwritten labels: {labels}

Constraints:
The text must be short, readable, and secondary to the visual action. Do not create a PPT slide or dense infographic. No paragraphs. No copied logos or reference marks. No 小黑 unless explicitly requested. White background only. Do not use this mode for normal body illustrations unless the user explicitly asks for more on-image text.
```

## Iteration Prompts

### Make It Less PPT

```text
Regenerate the same core idea as a sparse editorial hand-drawn body illustration. Remove slide-like layout, boxes, formal arrows, diagram labels, and any large title. Keep one human figure interacting with one object metaphor on a pure white background with restrained Interflow color accents.
```

### Return To Canonical Body Illustration

```text
Regenerate as the canonical body spot illustration: no title, no headline, one main elongated line-art person, 3-5 core objects maximum, at most four short Chinese labels, at least 45% blank white space, pure white background, restrained Interflow blue/orange/yellow/mint/pink accents.
```

### Increase Explanation Clarity

```text
Keep the same white-background American editorial line-art style, but make the human-object relationship explain the idea more clearly. Add up to three short Chinese labels. Do not add a title or dense text.
```

### Fix Text

```text
Edit only the Chinese text in the image. Replace the incorrect text with: {correct_text}. Keep the same drawing, white background, line style, composition, and blue accents.
```
