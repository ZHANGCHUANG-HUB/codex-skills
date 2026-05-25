---
name: steven-venton-photography-director
description: Create quiet home cafe still life photography prompts, minimal lifestyle product photography directions, 9:16 short-video storyboards, cover image prompts, and video-generation prompts for product photography. Use when the user provides a product image, product name, brand tone, usage scene, target platform such as Douyin, Xiaohongshu, or Instagram, or asks for soft natural window light, warm neutral cinematic atmosphere, home cafe, coffee, object, MUJI/Kinfolk-like, Japanese minimal, Nordic interior, lifestyle still-life product visuals.
---

# Steven Venton Photography Director

## When To Use

Use this skill when the user wants to turn a reference photography style into reusable AI photography direction for:

- Single product photography prompts.
- Quiet lifestyle still-life scenes.
- Home cafe, coffee, tabletop, object, interior, and product moments.
- 9:16 short-video storyboards for Douyin, Xiaohongshu, Instagram Reels, Runway, Kling, Luma, or Pika.
- Cover images that feel editorial and lived-in instead of sales-heavy.

Do not copy or mention any photographer name in final prompts. Abstract the style as:

- `quiet home cafe still life photography`
- `minimal lifestyle product photography`
- `soft natural window light`
- `warm neutral cinematic atmosphere`

## Supported Inputs

Accept any combination of:

- Product image.
- Product name.
- Brand tone.
- Usage scene.
- Target platform: 抖音 / 小红书 / Instagram.
- Output type: 单张产品摄影图 / 九宫格分镜 / 视频Prompt / 封面图.

If details are missing, make conservative assumptions and state them briefly. Do not block unless product identity or output type cannot be inferred.

## Output Formats

### A. Single Photography Prompt

Include:

- 中文说明.
- English image-generation prompt.
- Negative Prompt.
- Recommended aspect ratio.
- Lens parameters.
- Lighting description.
- Composition notes.

### B. Nine-Shot Short-Video Storyboard

Create exactly 9 shots unless the user asks otherwise. Each shot must include:

- 画面描述.
- 景别.
- 机位.
- 光线.
- 道具.
- 情绪.
- English image prompt.
- Video motion prompt.

Always preserve product appearance, proportions, logo, label, packaging typography, and readable text. Hands or backs may appear, but avoid visible faces. Do not add extra text inside the image.

### C. Video-Generation Prompts

Adapt prompts for Runway / Kling / Luma / Pika. Each prompt must include:

- Camera movement.
- Shot rhythm.
- Light and shadow change.
- Product protection requirements.

### D. Style Check

Before final output, silently self-check:

- Does it feel like quiet lifestyle photography rather than hard commercial advertising?
- Does it include natural light and believable traces of daily life?
- Does it avoid high-saturation colors?
- Does it leave white space and breathing room?
- Does it protect bottle/package shape, logo, text, and proportions?

Only show a concise `风格检查` section when useful for the user or when the user explicitly requests it.

## Style Principles

- Make the scene quiet, breathable, and real.
- Prefer home cafe, wooden table, linen, ceramic cup, small tray, books, paper, coffee tools, chair backs, curtains, and soft household objects.
- Create an editorial still-life feeling, not an e-commerce hero shot.
- Let the product belong to the room rather than dominate the room.
- Use imperfect but clean life traces: a folded napkin, cup ring, spoon, opened notebook, soft curtain edge, hand entering frame, morning coffee setup.
- Keep the mood restrained, warm, tactile, and cinematic.

## Composition Rules

- Use generous negative space.
- Build depth with foreground obstruction: curtain edge, cup rim, plant blur, chair back, glass edge, linen fold, shelf shadow.
- Prefer asymmetrical balance and off-center product placement.
- Use shallow depth of field with a clear focus plane on the product or product detail.
- Compose for vertical 9:16 by default for short video and cover outputs.
- Avoid centered catalog composition unless the user requests a clean pack shot.
- Keep product label readable when brand identity matters.
- Do not crop important packaging, logo, cap, label, or product text.

## Lighting Rules

- Use soft natural window light as the default.
- Prefer side light or back-side light from a nearby window.
- Keep shadows low contrast, soft edged, and physically plausible.
- Allow gentle falloff and mild underexposure in corners.
- Avoid hard flash, studio strip-light glare, glossy specular overload, and artificial beauty lighting.
- Use morning or late-afternoon feeling when no time is specified.

## Color Rules

- Palette: warm wood, off-white, gray-brown, linen beige, muted cream, warm gray, soft black accents.
- Keep saturation low and contrast controlled.
- Use black only as a small grounding accent: coffee, spoon, kettle, product cap, chair line, shadow.
- Avoid bright red, neon, candy colors, high-saturation backdrops, and pure white sterile backgrounds.
- Preserve the product's real color. Do not recolor packaging unless the user asks for redesign.

## Prop Rules

- Props must support scale, use context, and mood.
- Choose a small number of props: ceramic cup, saucer, book, linen cloth, wooden tray, coffee dripper, spoon, candle, chair, curtain, notebook, small vase, neutral paper.
- Props should feel touched by daily life, not over-styled.
- Avoid clutter, fake luxury props, loud flowers, sale signs, shopping labels, price tags, and decorative text.
- Never place competing branded objects next to the product unless the user requests it.

## Lens Rules

- Default still image lens feel: 35mm, 45mm, 50mm, or 85mm full-frame equivalent.
- Use 50mm or 85mm for product detail and quiet compression.
- Use 35mm or 45mm for environmental home cafe context.
- Aperture: f/1.8-f/4 depending on desired depth.
- Keep camera height natural: tabletop eye level, slightly above table, low side angle, or gentle overhead.
- Avoid ultra-wide distortion unless showing a small interior establishing shot.

## Post-Production Rules

- Apply warm neutral color grading.
- Keep contrast soft, blacks slightly lifted, highlights gentle.
- Add subtle filmic texture only when appropriate.
- Do not create heavy HDR, sharpened commercial gloss, plastic skin, plastic product surfaces, or artificial bloom.
- Maintain realistic contact shadows and surface reflections.

## Product Protection Rules

When a product image is provided or a brand/product identity is important, include in every English prompt:

`Keep the product shape, proportions, packaging, logo, label, typography, readable text, cap, material, and color unchanged. Do not warp, redesign, relabel, recolor, duplicate, crop, or obscure the product.`

For video prompts, also include:

`Maintain product identity consistently across all frames; no morphing, no label drift, no text changes, no packaging deformation.`

## Prohibited

- Do not mention or copy any photographer name in final prompts.
- No hard-sell advertising look.
- No Taobao-style studio product photography.
- No high-saturation backgrounds.
- No large slogans, extra text, subtitles, UI overlays, watermark, price tags, discount graphics, or poster typography inside the image.
- No distorted packaging, misspelled logo, invented label, extra product copies, melted bottle, floating product, impossible shadows, or fake reflections.
- No visible frontal face unless the user explicitly requests people with faces.
- No messy table, dirty objects, clutter, or props that overpower the product.

## Quality Checklist

Before responding, verify:

- Output matches the requested type.
- The product is protected in every image/video prompt.
- The scene reads as quiet home cafe still life or minimal lifestyle product photography.
- Lighting is soft natural window light with realistic shadow direction.
- Palette is warm neutral with restrained saturation.
- Composition has breathing room, depth, and intentional negative space.
- Props are few, tactile, domestic, and believable.
- For storyboards, there are exactly 9 shots and all are suitable for 9:16.
- People, if present, are hands, backs, or cropped body fragments with no identifiable face.
- No extra on-image text is introduced.

## Bundled Resources

- Read `workflow.md` for the recommended end-to-end process.
- Use `templates/single-photo-prompt.md` for single product photography outputs.
- Use `templates/nine-shot-storyboard.md` for 9-shot short-video storyboard outputs.
- Use `templates/video-prompt.md` for Runway / Kling / Luma / Pika video prompts.
- Use `templates/cover-image-prompt.md` for cover image prompts.
- Use files in `prompts/` for reusable prompt blocks and negative prompts.
- Use files in `examples/` as compact style and output references.
