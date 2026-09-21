# Civilization VI Historical Character Prompt Skill

A strict prompt-generation Skill for creating **stylized Civilization VI-inspired historical leader portraits**.

## Input

Enter a historical character name:

> 岳飞

> 秦始皇

> 宋徽宗

> 拿破仑

The Skill automatically determines the historical context, costume, colors, facial characteristics, and visual identity.

## Output

The Skill returns **only one main image-generation prompt**.

There is intentionally **no negative prompt**. The visual constraints are embedded directly into the main prompt because many image-generation workflows handle positive descriptive prompting more reliably than a separate negative prompt.

## Key visual target

The prompt is designed to produce:

- stylized high-quality 3D rendering
- grand strategy game leader art
- Civilization VI-inspired visual language
- expressive and slightly exaggerated facial proportions
- polished PBR materials
- highly detailed historical costume
- full-body standing character
- empty hands
- pure white background
- soft dramatic studio lighting
- clear silhouette
- rich four-color palette
- painterly 3D game-render finish

## Important difference from a realistic historical portrait

This Skill does not simply describe a historically accurate person and append "3D".

It deliberately reinforces the **designed, stylized, game-character quality** throughout the prompt so the result stays closer to a grand-strategy-game leader illustration rather than a realistic historical portrait.

## Example

Input:

> 岳飞

The generated prompt will contain:

- Song-dynasty historical identity
- military-leader visual characteristics
- historically appropriate clothing and hair/headwear
- expressive and stylized facial design
- detailed fabric and ornament
- full-body standing pose
- empty hands
- pure white background
- soft dramatic studio lighting
- a coherent historical color palette

## Style reference

Civilization VI is used as a high-level visual reference for strategy-game leader presentation. This Skill does not reproduce proprietary character models or assets.
