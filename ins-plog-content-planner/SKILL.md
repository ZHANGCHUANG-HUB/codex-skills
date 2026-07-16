---
name: ins-plog-content-planner
description: Create and optionally generate complete Instagram-inspired PLOG photo sets for Xiaohongshu, Instagram, and Douyin from a product image, reference image, brand, product, scene, theme, or mood keyword. Use when Codex needs to plan or directly render a cohesive 6- or 9-image lifestyle carousel, write and execute English AI image prompts, preserve an uploaded product's visual identity, establish shared visual controls, or produce matching social captions, titles, cover text, and hashtags. When the user asks to generate, render, make, or directly produce the images, use an available image-generation tool after planning. Focus on still-image PLOG content rather than video storyboards unless the user explicitly requests video.
---

# INS PLOG Content Planner

Turn a vague product or lifestyle idea into a cohesive, publication-ready still-image PLOG plan and, when requested, generate the planned images. Explain the plan in Chinese and write every image-generation prompt in English.

## Choose the Delivery Mode

- **Planning mode:** Use when the user asks for a plan, prompts, copy, ideas, or a PLOG proposal. Return the complete written package only.
- **Direct-generation mode:** Use when the user asks to generate images, make the PLOG images, produce final visuals, directly render, or uses equivalent wording. Create the written plan, then invoke an available image-generation tool to render the images.
- Do not treat “生成 Prompt” or “生图提示词” as a request to render images; those phrases request planning mode.
- If the user explicitly asks for both a plan and images, provide both.

## Workflow

1. Inspect all supplied product and reference images before planning. Treat the product image as the source of truth for product appearance. Treat reference images as guidance for scene, composition, palette, and mood.
2. Classify the request:
   - Product: balance recognizable product exposure with natural lifestyle context.
   - Lifestyle: prioritize atmosphere, authentic fragments, emotion, and visual rhythm.
   - Mixed: combine product visibility with a believable scene narrative.
3. Infer missing settings without stopping for clarification when the defaults below are safe. Ask only when a missing choice would materially change the result.
4. Establish one theme and a visual story arc before writing individual images.
5. Produce the required sections in the exact order under **Required Output**.
6. In direct-generation mode, generate the images by following **Direct Image Generation**.
7. Check continuity, prompt completeness, platform fit, product consistency, and absence of unwanted video material.

## Defaults

- Produce 6 images unless the user requests another count or asks for a fuller set; use 9 images for a fuller set.
- Use a 3:4 aspect ratio for every image.
- Adapt to Xiaohongshu, Instagram, and Douyin photo posts unless a platform is specified.
- Use Instagram-inspired lifestyle photography: natural, relaxed, clean, atmospheric, realistic, softly editorial, low-saturation, neutral-warm, and spacious.
- Prefer window light, daylight, or soft evening light with soft shadows.
- Avoid cheap e-commerce styling, hard-sell poster aesthetics, oversaturation, harsh HDR, excessive retouching, and contrived posing.
- Do not output video storyboards, camera movement, voice-over scripts, or short-video scripts unless explicitly requested.

## Direct Image Generation

Read [references/direct-generation.md](references/direct-generation.md) before invoking an image-generation tool.

- Use the image-generation capability available in the current environment. Do not merely tell the user to copy the prompts into another tool when direct generation is available.
- Inspect uploaded product and reference images before generation. Include every required source image through the tool's supported reference-image mechanism.
- Generate all requested images. When the tool supports only one generation at a time or cross-image consistency is fragile, render sequentially and carry forward the same art direction and product reference.
- Keep every output at 3:4 unless the user requests another ratio.
- Treat generated images as outputs in addition to, not replacements for, the written PLOG package unless the user asks for images only.
- If no image-generation tool is available, state that limitation clearly and still deliver the complete executable plan and prompts.

## Planning Rules

Read [references/plog-structure.md](references/plog-structure.md) before planning the image sequence.

- Give every image a distinct narrative job while maintaining a coherent setting, palette, lighting family, prop language, and photographic treatment.
- For product work, include a useful mix of hero, environment, interaction or use, detail, and closing atmosphere images.
- Make product placement feel incidental to real life rather than pasted into an advertisement.
- Keep hands plausible and actions simple. Avoid unnecessary faces when identity is not relevant.
- Vary shot scale and composition enough to create rhythm, but do not make the set look like unrelated campaigns.

## Prompt Rules

Read [references/image-prompt-rules.md](references/image-prompt-rules.md) before writing prompts.

- Write one self-contained English prompt per image that can be sent directly to an image model.
- State the subject, setting, visual style, lighting, composition, mood, lens or photographic feel, and `3:4 aspect ratio`.
- Do not use placeholders such as “same as above”; repeat the essential shared controls in each prompt.
- When images are supplied, refer to them by role, such as “the supplied product reference image” and “the supplied visual reference image.” Do not claim pixel-perfect text or logo reproduction; instruct the model to preserve visible product identity and recommend reference-image conditioning where supported.

## Copy Rules

Read [references/social-copy-rules.md](references/social-copy-rules.md) before writing social copy.

- Sound like a real personal share: relaxed, observant, aesthetically aware, and lightly recommendatory.
- Avoid official brand copy, exaggerated claims, fake testimonials, and aggressive calls to action.
- When the platform is unspecified, write one caption that reads naturally on all three default platforms.

## Required Output

Use these exact Chinese H1 headings and keep this order:

1. `# 主题定位`
2. `# 整组内容思路`
3. `# 图片规划表`
4. `# 统一风格控制`
5. `# 图文文案`
6. `# 标题建议`
7. `# 封面短句`
8. `# 标签建议`

Under `# 主题定位`, include the PLOG theme name, suitable platforms, core mood keywords, audience, and overall visual direction.

Under `# 整组内容思路`, summarize the story progression from opening atmosphere through closing frame.

Under `# 图片规划表`, create one row per image with:

- 图片序号
- 画面内容
- 构图建议
- 光线建议
- 产品角色（主角 / 配角 / 点缀；无产品时写“无”）
- 情绪关键词
- 英文生图 Prompt

Under `# 统一风格控制`, state the shared style, ratio, photographic realism, light, palette, composition, texture, and negative constraints.

Under `# 图文文案`, write one finished caption. Under `# 标题建议`, provide exactly 3 titles. Under `# 封面短句`, provide exactly 1 short cover line. Under `# 标签建议`, provide exactly 5 relevant hashtags unless the user requests otherwise.

## Final Check

- Confirm the requested or default image count is present.
- Confirm every row contains a complete English prompt and a 3:4 ratio instruction.
- Confirm uploaded product identity constraints appear in every product-visible prompt.
- Confirm the sequence contains both visual consistency and shot-to-shot variation.
- Confirm no poster text is requested inside generated images unless explicitly asked.
- Confirm the answer remains focused on still images and social copy.
- In direct-generation mode, confirm the requested number of images was actually generated or clearly report any tool limitation that prevented completion.
