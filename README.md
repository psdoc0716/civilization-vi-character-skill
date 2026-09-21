# Civilization VI Historical Character Prompt Skill

A strict prompt-generation Skill for creating **medium-realism, stylized Civilization VI-inspired historical leader portraits**.

## The key visual target

The intended look is:

**中等写实 + 风格化 + 明显 3D 建模感 + 策略游戏角色质感**

It should look like a professionally modeled and rendered game character, not like a photograph of a real person.

### What to emphasize

- stylized 3D game character
- medium realism
- visible 3D modeling
- slightly exaggerated but natural proportions
- simplified facial planes
- expressive character design
- painterly game-rendered surfaces
- controlled game lighting
- clear 3D shadow structure
- historically accurate costume design
- full-body standing character
- pure white background

### What to avoid

The Skill deliberately avoids pushing the image model toward:

- photorealistic portraits
- hyperrealistic skin
- documentary photography
- live-action movie stills
- photographic lighting
- microscopic skin pores
- excessive realistic wrinkles
- generic realistic historical portraits

It also avoids relying on a negative prompt. The visual target is established directly inside the main prompt.

## Input

Enter a historical character name:

> 岳飞

> 秦始皇

> 宋徽宗

> 拿破仑

The Skill automatically determines the historical context, costume, colors, facial characteristics, and visual identity.

## Output

The Skill returns **only one main image-generation prompt**.

There is intentionally **no negative prompt**.

## Example visual logic

For a historical character, the Skill separates two layers:

**Historical layer**

- era
- clothing
- headwear
- hairstyle
- accessories
- colors
- symbols

**Game-art layer**

- stylized 3D modeling
- moderate realism
- slightly exaggerated facial proportions
- simplified facial planes
- designed character silhouette
- game-rendered materials
- controlled 3D lighting

This separation is important: historical details provide authenticity, while the game-art layer prevents the result from becoming a realistic historical photograph.

## Style reference

Civilization VI is used as a high-level visual reference for strategy-game character presentation. The target is medium-realism, stylized 3D game art rather than photorealistic photography or cartoon illustration. This Skill does not reproduce proprietary character models or assets.
