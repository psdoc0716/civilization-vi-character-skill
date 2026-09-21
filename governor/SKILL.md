---
name: civilization-vi-governor-portrait-skill
description: Generate Civilization VI-inspired Governor portrait prompts from either a historical character name or a free-form character description. Automatically translate the input into an expressive, stylized AAA strategy-game 3D portrait with exaggerated facial identity, culturally appropriate costume, soft white background, chest-up framing, and a characteristic lower-body fade.
---

# Civilization VI Governor Portrait Prompt Skill

## Purpose

Create a unified set of Civilization VI-inspired Governor portraits.

This skill accepts either:

1. A named historical character, such as:
   - 岳飞
   - 诸葛亮
   - 花木兰
   - 亚历山大大帝

2. A free-form visual description, such as:
   - 一个中国男性，魁梧、武将、正义
   - 一个印度女性，优雅、聪慧、商人
   - 一个北欧男性，年长、粗犷、探险家

The output should be a production-ready image-generation prompt.

## Input Interpretation

### Named historical character

When the input is a real historical figure:

1. Identify the figure and disambiguate if necessary.
2. Determine the most representative historical era and cultural context.
3. Infer historically appropriate:
   - age
   - facial features
   - hairstyle and facial hair
   - clothing
   - headwear
   - weapons
   - jewelry and accessories
   - cultural motifs
4. Preserve the person's recognizable historical identity while translating it into a stylized game character.

If historical evidence is uncertain, use historically plausible details rather than inventing false certainty.

### Free-form character description

When the input is descriptive rather than a name, do not force historical attribution.

Automatically derive:

- gender presentation if stated
- approximate age
- ethnicity/cultural setting if stated
- body type
- profession or archetype
- personality
- clothing
- accessories
- color palette
- facial expression
- pose

If the description includes a culture or historical period, make the costume and visual details consistent with that context.

If no period is specified, prefer a broadly believable cultural interpretation and avoid unnecessary anachronisms.

## Governor Portrait Visual Language

The target is a stylized strategy-game Governor portrait inspired by the presentation language of Civilization VI Governor illustrations.

### Character modeling

- high-quality stylized 3D character
- polished AAA strategy-game character art
- strong silhouette
- highly recognizable face
- expressive, slightly exaggerated facial proportions
- distinctive nose, jaw, cheeks, brows, eyes, ears, lips, or facial hair
- appealing caricature without becoming cartoonish or chibi
- realistic anatomy underneath stylization
- rich PBR materials
- detailed skin, hair, fabric, leather and metal
- painterly finish integrated with 3D rendering

### Face and expression

The face is the primary focal point.

Use a memorable, characterful expression appropriate to the input:

- confident
- stern
- benevolent
- clever
- dignified
- humorous
- determined
- contemplative
- warm
- intimidating

Do not make every character conventionally handsome or symmetrical. Distinctive facial identity is important.

### Pose and framing

- single character
- chest-up to approximately waist-up portrait
- centered or slightly offset centered composition
- facing camera or subtle three-quarter angle
- shoulders and upper torso clearly visible
- natural head tilt when appropriate
- expressive but restrained pose
- hands generally outside the frame unless an accessory naturally enters the composition
- character should feel like a selectable strategy-game Governor portrait

### Character clothing

Costume must support the character's identity.

For named historical figures, use historically appropriate clothing and accessories.

For descriptive inputs, design clothing from the stated occupation, culture, personality, and era.

Use layered materials such as:

- wool
- cotton
- linen
- silk
- leather
- bronze
- iron
- steel
- wood
- jade
- gold
- painted fabric

Keep the costume readable at portrait scale. Avoid filling the image with tiny decorative details that do not survive downsampling.

### Lighting and rendering

- soft studio-like directional light
- gentle rim light
- subtle ambient occlusion
- smooth global illumination
- controlled specular highlights
- soft shadows
- detailed but not gritty skin
- warm/cool material separation where useful
- polished game-render presentation
- painterly highlights and controlled edge definition

Avoid harsh photographic lighting and avoid flat vector illustration.

### Background and lower fade

Use:

- clean pure white background
- no environment
- no architecture
- no landscape
- no secondary characters
- no text
- no logo
- no UI
- no decorative border

The lower portion of the portrait should gradually fade into the white background with a soft, feathered silhouette transition. This fade is an important part of the Governor-portrait presentation.

Do not use a hard rectangular crop.

### Color

Use a coherent palette derived from the character.

For example:

- military characters: restrained metallic, leather, deep red/brown/blue
- scholars: muted fabric, parchment, dark ink, warm neutral accents
- merchants: richer textiles, jewelry, warm saturated accents
- religious figures: culturally appropriate ceremonial colors
- rulers: richer materials and controlled metallic accents

Do not force the same color palette onto every character.

## Output Format

Return three sections.

### 1. Character Interpretation

Briefly explain how the input was interpreted.

For a named person, include the historical identity and representative period.

For a description, summarize the inferred visual identity.

### 2. Main Prompt

Write one complete image-generation prompt containing:

- character identity
- appearance
- expression
- costume
- accessories
- pose
- stylized 3D modeling
- PBR materials
- lighting
- white background
- soft lower fade
- composition and framing
- overall Civilization VI-inspired Governor portrait presentation

### 3. Negative Prompt

Use this baseline:

modern clothing, random modern objects, science fiction, cyberpunk, anime, manga, chibi, cute mascot, flat vector art, photorealistic photography, low-poly, crude cartoon, plastic skin, distorted anatomy, generic face, expressionless face, incorrect historical costume, mixed historical periods, mixed civilizations, random cultural symbols, multiple characters, background characters, environment, architecture, landscape, busy background, text, logo, watermark, UI, border, hard rectangular crop, harsh shadow, extreme contrast, excessive detail noise, blurry, low resolution, low detail

Add input-specific exclusions when useful.

## Consistency Rules

For a series, keep these presentation variables stable:

- single character
- chest-up/waist-up framing
- stylized AAA 3D strategy-game character
- expressive exaggerated facial identity
- polished PBR materials
- soft directional studio lighting
- pure white background
- soft lower-body fade into white
- clean silhouette
- no text or UI

Only the character-specific identity, costume, expression, accessories, and palette should change.

## Important Distinction

This skill is intentionally different from the full-body historical leader portrait skill.

Governor portraits emphasize:

- face
- personality
- caricature
- expression
- chest/waist-up composition
- soft fade into white

Leader portraits emphasize:

- full-body presence
- historical costume
- heroic stance
- complete equipment and silhouette

Use the Governor skill when the desired output resembles a compact selectable Governor portrait rather than a full-body leader illustration.

## Response Behavior

If the user gives only a name, generate the prompt directly.

If the user gives only a descriptive phrase, generate the character directly from that description without asking for unnecessary clarification.

Ask a clarification only when the input is too ambiguous to determine a materially different character design.
