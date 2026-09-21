---
name: civilization-vi-character-skill
description: Generate historically grounded Civilization VI-style 3D character portrait prompts from a character name. Automatically adapt historical era, civilization, identity, clothing, headwear, hairstyle, weapons, accessories, cultural symbols, pose, materials, lighting, composition, white background, and negative prompts while maintaining a consistent AAA strategy-game character-art language.
---

# Civilization VI Historical Character Portrait Prompt Skill

## Purpose

When the user provides only a historical character name, generate a production-ready image-generation prompt for a unified Civilization VI-inspired historical character portrait.

The goal is visual consistency across a large cast: different civilizations and eras should remain historically distinct while sharing one coherent AAA strategy-game 3D character-art treatment.

## Input

The user may provide only a character name, for example:

- 秦始皇
- 阿育王
- 成吉思汗
- 亚历山大大帝
- 苏莱曼大帝
- 伊丽莎白一世

Do not require the user to repeat the style requirements.

## Workflow

1. Identify the historical figure and disambiguate similarly named figures.
2. Determine the most representative historical period and context.
3. Determine civilization/region, cultural background, approximate age, social status, and role.
4. Select historically appropriate:
   - clothing
   - hairstyle and facial hair
   - headwear/crown/helmet
   - weapons
   - jewelry and accessories
   - textiles, patterns, insignia, and cultural symbols
5. Prefer the figure's most recognizable period representation when multiple periods are possible.
6. Do not mix clothing, equipment, architecture, or symbols from unrelated periods or civilizations.
7. Convert the historical research into the fixed visual language below.
8. Output a complete image-generation prompt plus negative prompt.

## Fixed Visual Language

Use a high-quality AAA strategy-game character aesthetic inspired by the visual language of Civilization VI:

- polished 3D character modeling
- physically based materials (PBR)
- realistic skin, hair, beard, metal, leather, wood, and textile textures
- subtly stylized facial proportions with strong character identity
- cinematic but controlled soft directional lighting
- ambient occlusion and refined global illumination
- painterly game-concept-art finish integrated with high-end 3D rendering
- rich but restrained color design
- believable anatomy and historical costume construction
- strong cultural and historical readability

Do not copy an exact existing character model or reproduce proprietary assets. Treat Civilization VI as a high-level stylistic reference.

## Composition

- one person only
- standing pose
- full body or approximately knee/thigh-up, depending on the image model's framing
- centered composition
- front-facing to three-quarter view
- natural heroic presentation pose
- relaxed but confident posture
- hands may interact naturally with a weapon, belt, garment, or accessory
- keep head, arms, major costume elements, and important weapons inside the frame
- clear silhouette
- character occupies the primary visual area

## Background

- pure white background
- no environment or scenery
- no buildings
- no secondary characters
- no decorative graphics
- no text
- no logo
- no UI
- no frame
- subtle natural contact shadow only
- clean separation from the background
- suitable for later background removal and graphic layout

## Historical Accuracy Module

Automatically adapt the following to the named figure:

1. historical era
2. civilization/region
3. ethnicity/cultural context when historically relevant
4. approximate age
5. political/social/military/religious role where documented
6. representative clothing
7. headwear
8. hairstyle and facial hair
9. weapons
10. jewelry and accessories
11. characteristic colors and materials
12. recognizable cultural symbols

Historical details must be internally consistent. If evidence is uncertain or surviving depictions are later artistic reconstructions, prefer cautious wording such as "historically plausible" rather than inventing certainty.

## Output Format

Return:

### 1. Character Design
A concise description of the historically appropriate appearance.

### 2. Main Prompt
One complete prompt ready to paste into an image-generation model. It should explicitly include the character name, historical context, costume and equipment, fixed visual language, pose, composition, white background, lighting, and material details.

### 3. Negative Prompt
Use a reusable negative prompt and add any character-specific exclusions needed to prevent historical or visual mistakes.

Recommended baseline negative prompt:

modern clothing, modern hairstyle, modern weapons, modern objects, science fiction, cyberpunk, anime, manga, chibi, cartoon, photorealistic studio photography, low-poly, plastic skin, distorted anatomy, incorrect historical costume, anachronistic equipment, mixed civilizations, mixed historical periods, random cultural symbols, multiple people, background characters, architecture, landscape, scenery, text, logo, watermark, UI, frame, cropped head, cropped hands, cropped weapon, cut-off costume, blurry, low resolution, low detail, stiff pose, exaggerated pose

## Consistency Rules

For a series of characters, keep these invariant unless the user explicitly requests otherwise:

- pure white background
- single-character presentation
- centered composition
- front or three-quarter view
- standing heroic pose
- high-end 3D strategy-game character rendering
- PBR materials
- cinematic soft directional lighting
- painterly concept-art finish
- clean silhouette and contact shadow

Only the historically specific layer should change between characters.

## Response Behavior

If the user supplies only a name, do not ask them to restate the style. Generate the prompt directly.

If the name is ambiguous, ask a short clarification only when the ambiguity materially changes the historical design.

If the user supplies an image of a character, preserve the requested visual identity and composition constraints while adapting the prompt to the historical figure.

If the user asks for a different aspect ratio, camera angle, background, or rendering style, change only the requested variable unless it conflicts with the series consistency requirements.
