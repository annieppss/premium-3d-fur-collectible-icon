---
name: premium-3d-fur-collectible-icon
description: Create or restyle a living animal or character as a premium 3D collectible icon with short, dense, carefully groomed fur and stylized toy proportions. Use for furry designer-toy renders, squirrel-like short fur, velvety flocked figures, or reference-image edits where fur is required; do not use for smooth PVC, resin, glass, or non-living object icons.
---

# Premium 3D Fur Collectible Icon

Generate one square ImageGen image per requested character. Keep the character as a compact, high-end collectible figure rather than turning it into a photoreal animal, plush doll, or flat illustration.

## Workflow

1. Identify the character and whether the request includes a character reference, fur reference, or both.
2. Lock the character's identity before describing its fur: silhouette, head-to-body ratio, facial geometry, colors, markings, limb count, tail, and signature details.
3. Derive only material evidence from fur references: pile length, density, direction, softness, guard hairs, sheen, and color variation. Do not import the reference animal's anatomy or markings unless requested.
4. Select the fur treatment that fits the species and request. When no fur reference is supplied, use short, dense, directionally groomed fur appropriate to the character's species.
5. Call `image_gen.imagegen` directly. For an edit, include every required character reference and make identity preservation explicit. Ask a question only when the character itself is ambiguous or required references are missing.
6. Return the generated image. For a set, reuse the same identity lock, fur treatment, lighting, camera language, and background.

## Identity Lock

Treat an attached character image as the authority for design. Preserve its recognizable silhouette and signature features even when natural animal references differ.

- Keep the original head-to-body ratio, face placement, eye spacing, ear shape, muzzle shape, colors, markings, tail design, and number of limbs.
- Express existing markings through fur color rather than attached plastic pieces.
- Keep eyes, nose, mouth, claws, glasses, and other non-fur details in their appropriate smooth material.
- Do not add realistic species anatomy, back stripes, whiskers, claws, or tail details merely because they appear in a fur reference.
- When changing pose or view, change only what the user requests; keep all identity-defining features stable.

## Short-Fur Material

Use a premium velvety flocked collectible finish combined with stylized short animal fur.

- Cover fur-bearing areas with dense, short, fine fibers. Keep them straight or gently directional, never curly unless requested.
- Follow the anatomy with a clean directional flow. Use the shortest pile around the eyes, nose, mouth, muzzle, fingers, and toes so facial and anatomical shapes remain legible.
- Allow slightly softer volume on the cheeks, torso, outer limbs, and tail. Add sparse, delicate guard hairs only where they help the silhouette, such as ear edges, cheeks, back, and tail.
- Use a tidy semi-matte surface with soft diffuse highlights. Individual hairs may be visible at close range, but the figure must still read as a clean designer toy.
- Keep colored regions controlled and recognizable. Natural color variation should be subtle and must not muddy the character's palette.
- Make the eyes and nose smoother and glossier than the fur to create a restrained material contrast.

## Prompt Template

Adapt this template to the user's character and references:

```text
Create a premium 3D collectible toy-style icon of [CHARACTER].

IDENTITY LOCK:
[List the character's fixed silhouette, proportions, facial geometry, colors, markings, tail, limbs, and signature details. State that the provided character reference is authoritative.]

FUR MATERIAL:
Cover the fur-bearing areas with dense, short, finely groomed [SPECIES]-appropriate fur rendered as a premium velvety flocked collectible finish. The short pile follows the anatomy in a clean directional flow. Keep it extremely short around the eyes, nose, mouth, muzzle, fingers, and toes; allow slightly softer volume on the cheeks, torso, and tail. Add only sparse, delicate guard hairs along selected silhouette edges. Use a soft semi-matte response with diffuse highlights. Keep eyes and nose smooth and subtly glossy. Preserve the character's original color blocks and markings through controlled fur color.

STYLE AND COMPOSITION:
Keep a simple, bold, rounded designer-toy silhouette with visible volume and softly rounded edges. Center one complete character on a square canvas with generous breathing room. Use soft, even studio lighting and a warm ivory seamless background with a faint contact shadow. No scenery unless requested.

REFERENCE BOUNDARY:
Use animal photographs only as evidence for fur length, density, direction, softness, sheen, and natural color variation. Do not copy their anatomy, pose, markings, or proportions unless explicitly requested.

No text, logo, watermark, UI elements, duplicate character, extra or missing limbs, changed identity, photoreal animal anatomy, glossy PVC skin on fur-bearing areas, ceramic, clay, hard plastic body, long shaggy fur, wool clumps, poodle-like curls, messy flyaways, wet or matted fur, bald patches, coarse bristles, excessive individual hair detail, low-poly geometry, harsh shadows, grain, or noise. Ultra-high-quality 3D render, premium furry collectible designer toy, clean studio lighting.
```

## Output Rules

- Default to a single square image with the entire character visible.
- Prefer a neutral front-facing pose for a master reference; preserve a requested pose when editing an existing scene.
- Keep backgrounds quiet so the fur edge and character silhouette remain easy to evaluate.
- Do not apply the pearly water-ripple background or inflated PVC finish from smooth collectible styles unless the user explicitly requests them.
