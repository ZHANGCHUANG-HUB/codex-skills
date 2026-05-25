---
name: commercial-food-storyboard-generator
description: Generate premium commercial food photography prompts and 9:16 short-video storyboards for products, food, drinks, restaurants, cafes, desserts, wineries, menu launches, social media ads, Douyin, Xiaohongshu, and Instagram Reels. Use when the user provides a product name, food or beverage concept, restaurant theme, product/reference image, or asks for commercial food photography prompts, short video shot lists, storyboard tables, nine-shot visual plans, AI image prompts, AI video prompts, or negative prompts.
---

# Commercial Food Storyboard Generator

## Purpose

Create a commercial-grade 9:16 food and beverage short-video storyboard that combines advertising photography prompt writing with a nine-shot video structure. Output in Chinese for planning fields and English for AI image/video prompts.

## Workflow

1. Extract or infer the brief:
   - Product name, food, beverage, restaurant, cafe, dessert, winery, or reference image subject.
   - Theme, such as情侣约会品酒, 餐厅新品上市, 咖啡馆探店, 甜品种草, 酒庄溯源.
   - Platform: 抖音, 小红书, Instagram Reels, or a sensible default based on the request.
   - Whether people appear, whether faces appear, and whether product text must be preserved.
2. If required inputs are missing, make conservative assumptions and state them briefly before the table. Do not stall unless the product or theme is impossible to infer.
3. Generate exactly 9 shots by default, all designed for vertical 9:16.
4. Use Markdown tables for the storyboard. Keep each cell concise but production-useful.
5. After the table, output the three required master prompts:
   - 整合版九宫格图片 Prompt
   - 逐镜头生成单图的 Prompt 模板
   - 视频生成总 Prompt

## Default Visual Style

Apply this style unless the user asks for a different style:

`premium commercial food photography, restaurant menu photography, editorial food styling, warm realistic lighting, shallow depth of field, carefully styled props, high-end social media advertising look, appetizing texture, cinematic composition`

Translate the look into concrete staging choices: natural highlights, appetite-driven texture, controlled reflections, styled tabletops, premium props, clean product visibility, and believable restaurant/cafe/bar/winery context.

## Nine-Shot Structure

Use this fixed sequence unless the user asks for a different number of shots:

| Shot | Role |
|---|---|
| 1 | 环境建立，展示氛围 |
| 2 | 产品第一次出现 |
| 3 | 食物/酒水细节特写 |
| 4 | 人物动作，例如倒酒、举杯、夹菜 |
| 5 | 餐桌全景 |
| 6 | 产品与场景融合 |
| 7 | 情绪氛围镜头 |
| 8 | 产品英雄镜头 |
| 9 | 结尾广告主视觉 |

## Storyboard Table Columns

Each shot must include these columns:

| Column | Content |
|---|---|
| 镜头 | Numbered `1` to `9` |
| 中文画面描述 | What appears on screen, with product, food, atmosphere, and action |
| 构图方式 | Vertical 9:16 framing, angle, lens feel, foreground/background layering |
| 光线设计 | Direction, quality, color temperature, highlight/reflection behavior |
| 道具建议 | Props that reinforce the product and theme without clutter |
| 英文 AI 绘图 Prompt | A complete image prompt in English |
| 英文 AI 视频 Prompt | A complete motion prompt in English |
| Negative Prompt | English negative prompt |

## Product Image Rules

When the user uploads or references a product image, include preservation instructions in every relevant English prompt:

- Keep the product shape, proportions, label, logo, cap, bottle/package material, and typography unchanged.
- Preserve all readable product text exactly when the user asks to retain product text.
- Do not warp, melt, crop off, relabel, redesign, recolor, or invent product packaging details.
- Integrate the product naturally into the scene, with contact shadows and matching reflection quality.
- Match the product lighting direction, shadow softness, and color temperature to the surrounding environment.

If no product image is provided, describe a plausible premium product appearance but avoid pretending that exact brand details are known.

## People And Face Rules

If the user requests people:

- Show lifestyle actions that sell the product: pouring wine, lifting a glass, cutting dessert, serving coffee, plating food, sharing at a table.
- Keep gestures natural and commercially polished.

If the user requests no visible face or no face:

- Do not show a complete frontal face.
- Use hands, backs, silhouettes, cropped shoulders, side profiles without identifiable facial detail, or partial body action.
- Express emotion through posture, table interaction, lighting, props, and atmosphere.

If the user requests no people, keep all shots product, food, table, service, or environment focused.

## Platform Tuning

Use `references/platform-style-notes.md` when the platform is important or the user asks for platform-specific tone. Otherwise apply these quick defaults:

- 抖音: faster, more sensory, stronger opening hook, vivid movement.
- 小红书: editorial lifestyle, refined props, aspirational but realistic.
- Instagram Reels: cinematic, polished, globally legible, premium brand feel.

## Negative Prompt Guidance

Include negatives that protect realism and commercial usability:

`low quality, blurry, noisy, distorted product, warped label, incorrect text, misspelled logo, extra fingers, deformed hands, unnatural skin, messy table, dirty food styling, overexposed highlights, harsh flash, plastic texture, fake food, watermark, subtitles, UI overlay, text artifacts, cropped product, duplicate product, distorted packaging`

Add face-specific negatives when no face is requested:

`full frontal face, direct eye contact, identifiable face, close-up face`

## Final Master Prompts

After the table, output:

1. `整合版九宫格图片 Prompt`: English prompt for one 3x3 storyboard grid image. Mention nine panels, vertical video storyboard frames, consistent product identity, commercial food photography, and the fixed shot sequence.
2. `逐镜头生成单图的 Prompt 模板`: English reusable template with placeholders like `[PRODUCT]`, `[THEME]`, `[SHOT_NUMBER]`, `[SHOT_DESCRIPTION]`, `[PLATFORM]`, `[FACE_RULE]`, `[PRODUCT_IMAGE_RULE]`.
3. `视频生成总 Prompt`: English prompt describing the full 9-shot vertical video, pacing, transitions, product continuity, lighting continuity, and social platform polish.

## Output Discipline

- Default to 9 shots and 9:16 vertical composition.
- Keep Chinese planning text actionable for a creative director or photographer.
- Keep English prompts ready to paste into AI image/video tools.
- Do not add unrelated marketing strategy unless the user asks.
- If the user provides a reference image, explicitly reflect its product/category, material, color palette, and mood without claiming unseen details.
