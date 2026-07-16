# Image Prompt Rules

## Required prompt anatomy

Write each prompt as a coherent English paragraph containing:

1. Main subject and its action or state
2. Physical setting and relevant props
3. Instagram-inspired realistic lifestyle photography style
4. Light source, direction, softness, and shadow character
5. Framing, shot scale, camera angle, negative space, and focal priority
6. Emotional atmosphere and palette
7. Lens or photographic feel, depth of field, and realistic texture
8. Explicit `3:4 aspect ratio`

Use practical photographic language. Prefer phrases such as `documentary lifestyle photography`, `subtle editorial feel`, `natural window light`, `soft shadows`, `clean composition`, `realistic materials`, and `gentle film-like color rendering` when appropriate.

## Product reference control

Whenever the product is visible, naturally include this control logic:

`Use the supplied product reference image as the identity source. Keep the product shape, proportions, packaging, logo, label layout, typography, cap, material, and colors consistent. Keep the product clear and recognizable. Do not warp, redesign, relabel, recolor, duplicate, crop, or obscure the product.`

Adapt the wording to the product. Do not mention a cap for a product that has none. If exact logo or typography fidelity is essential, recommend reference-image conditioning, inpainting, or a final compositing pass because generative models may alter fine text.

## Reference-image priority

When both product and visual references are provided:

1. Use the product reference to preserve appearance and identity.
2. Use the visual reference for composition, scene, lighting, palette, and mood.
3. Keep the final result within a relaxed INS-style PLOG aesthetic.

Do not copy protected visual details literally when a high-level aesthetic description is sufficient. Describe transferable traits such as lighting, framing, palette, texture, and mood.

## Product negative constraints

End product prompts with a concise selection of relevant constraints:

`No poster design look, no heavy text overlay, no cheap e-commerce styling, no oversaturated colors, no harsh HDR, no cluttered background, no awkward hands, no distorted objects, no unrealistic reflections, no excessive props, no fake luxury styling, no plastic skin, no overly staged commercial poster look.`

Do not bloat prompts with irrelevant negatives. Add `no duplicate product` whenever duplication is a plausible failure.

## Lifestyle negative constraints

Use only the relevant subset:

- no stiff posing
- no artificial studio look
- no oversaturated colors
- no harsh HDR
- no clutter
- no plastic skin
- no distorted hands
- no excessive props
- no text overlay

## Prompt quality check

- Make the prompt self-contained.
- Keep the main subject and focal priority unambiguous.
- Use one plausible light setup rather than conflicting light sources.
- Avoid conflicting composition commands.
- Avoid empty quality incantations that do not change the image.
- Keep the scene achievable and grounded in physical reality.
