# QA Checklist

## Pass Criteria

- White background, not beige or textured.
- Black/charcoal line art dominates.
- Blue accent is sparse and meaningful.
- When Interflow IP feeling is requested, Interflow Blue is the dominant color and orange/yellow/mint/pink appear as controlled recurring geometric accents.
- Human figure is simple, elongated, and editorial.
- The character performs the core explanatory action.
- One image explains one idea.
- Composition has enough whitespace.
- Labels, if any, are short and readable.
- The image feels like article illustration, not social media poster, PPT, course slide, or corporate vector art.
- It does not copy the supplied reference image's exact composition, character, text, logo, or signature.
- It does not use 小黑 unless the user explicitly requested 小黑.
- If a signature is requested, it uses only one tiny corner byline such as `互通有无` or `Interflow`, not a logo or large watermark.

## Failure Signals

- More characters than requested.
- Too many objects, arrows, boxes, or labels.
- A large title appears in a正文 image.
- It looks like a business PowerPoint page.
- It looks like a polished SaaS marketing illustration.
- It uses fake app UI or complex dashboards.
- The blue accent becomes a large decorative block without meaning.
- Interflow colors appear as random confetti and do not support movement, hierarchy, or brand recognition.
- The illustration recreates or distorts the official Interflow logo in a正文 image.
- The signature is too large, appears as a headline, or competes with the illustration.
- The text is misspelled, fake-looking, or too dense.
- The image is attractive but does not explain the paragraph.

## Iteration Rules

- If it is too decorative: make the object metaphor carry the article's core tension.
- If it is too abstract: add one concrete object from the article.
- If it is too busy: delete half the objects and labels.
- If it is too cute: simplify the face, reduce expression, and make the pose more deadpan.
- If it is too much like Xiaohei: remove mascot features and use a human figure.
- If the user wants clearer images: switch to Text-On-Image Mode with one headline and 3-5 labels.

## Handoff Note

Before publishing, inspect mobile readability. Chinese text in generated images often needs manual review or a second edit pass.
