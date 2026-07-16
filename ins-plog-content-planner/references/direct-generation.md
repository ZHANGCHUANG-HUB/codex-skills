# Direct Image Generation

## Execution sequence

1. Complete the theme, visual baseline, image sequence, and per-image prompts before rendering.
2. Inspect each supplied image. Assign product images to identity control and reference images to composition, palette, lighting, and mood control.
3. Pass the relevant source images to the image-generation tool using its supported local-path or recent-image reference mechanism.
4. Generate the complete requested set, preserving the same palette, location family, light character, material treatment, and product identity.
5. Review outputs when inspection is available. Regenerate obvious failures such as distorted packaging, duplicated products, illegible hero composition, inconsistent color, deformed hands, or an incorrect aspect ratio.

## Product consistency

- Use the original uploaded product image for every frame in which the product appears; do not rely only on a previously generated frame when an original reference is available.
- Keep the product's silhouette, proportions, package structure, closure, materials, colors, logo placement, and label layout stable.
- Avoid angles or hand placements that conceal identity-critical areas in hero and detail images.
- For tiny typography and logos, generation may not be exact. If brand fidelity is critical, explain that a later inpainting or compositing pass may be required.

## Set consistency

- Reuse one concise shared art-direction block across all generation prompts.
- Vary shot scale, crop, and action according to the plan without changing the campaign's world.
- Use wide, medium, and close shots to create rhythm.
- Do not generate poster text inside the image unless explicitly requested.

## Failure handling

- Regenerate only failed frames when possible; preserve successful frames.
- If the tool cannot produce the full set in one call, continue frame by frame.
- If the tool or environment imposes an output limit, generate as many as possible and state exactly which planned frames remain.
