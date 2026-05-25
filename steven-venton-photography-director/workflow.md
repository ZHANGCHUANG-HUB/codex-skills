# Workflow

## 1. Read The Brief

Extract:

- Product image or product description.
- Product name and category.
- Brand tone.
- Usage scene.
- Target platform: 抖音 / 小红书 / Instagram.
- Output type: 单张产品摄影图 / 九宫格分镜 / 视频Prompt / 封面图.
- Whether product text/logo must stay readable.
- Whether hands, back view, or no people are preferred.

If inputs are incomplete, infer quietly and state assumptions in one short line.

## 2. Choose The Output Template

- 单张产品摄影图: use `templates/single-photo-prompt.md`.
- 九宫格分镜: use `templates/nine-shot-storyboard.md`.
- 视频Prompt: use `templates/video-prompt.md`.
- 封面图: use `templates/cover-image-prompt.md`.

## 3. Apply The Core Look

Use this base language in English prompts:

`quiet home cafe still life photography, minimal lifestyle product photography, soft natural window light, warm neutral cinematic atmosphere, Japanese minimal interior, Nordic home styling, warm wood, off-white linen, gray-brown ceramic, soft black accents, generous negative space, shallow depth of field, foreground blur, low contrast shadows, editorial lifestyle composition`

Never include the source photographer's name in final prompts.

## 4. Protect Product Identity

When product identity matters, append:

`Keep the product shape, proportions, packaging, logo, label, typography, readable text, cap, material, and color unchanged. Do not warp, redesign, relabel, recolor, duplicate, crop, or obscure the product.`

For video:

`Maintain product identity consistently across all frames; no morphing, no label drift, no text changes, no packaging deformation.`

## 5. Build The Scene

Select a quiet daily-life setting:

- Window-side wooden table.
- Home cafe corner.
- Kitchen counter with linen and ceramics.
- Small shelf, chair, curtain, notebook, tray, coffee tools.
- Morning or late-afternoon light.

Keep props restrained and tactile. Use foreground blur or partial obstruction for depth.

## 6. Platform Tuning

- 抖音: stronger opening image, clearer product reveal, slightly more movement, still quiet and premium.
- 小红书: editorial daily-life styling, diary-like realism, refined home cafe props.
- Instagram: cinematic composition, globally legible minimal styling, polished neutral palette.

## 7. Self-Check Before Output

Check:

- It looks quiet and lived-in, not a hard advertisement.
- Natural window light is explicit.
- Palette avoids high saturation.
- Negative space is present.
- Product shape, logo, text, and proportions are protected.
- No extra text appears in the image.

## 8. Final Response Shape

Use Chinese for planning and direction. Use English for AI image and video prompts. Keep prompts production-ready and concise.
