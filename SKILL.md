---
name: civilization-vi-governor-portrait-skill
description: Generate Civilization VI-inspired Governor portrait prompts from either a historical character name or a free-form character description. Automatically translate the input into an expressive, stylized AAA strategy-game 3D portrait with exaggerated facial identity, culturally appropriate costume, soft white background, chest-up framing, and a characteristic lower-body fade.
---

# Civilization VI Governor Portrait Prompt Skill

## Purpose

Create a unified set of Civilization VI-inspired Governor portraits.

This skill accepts either:

1. A named historical character, such as 岳飞, 诸葛亮, 花木兰, or 亚历山大大帝.
2. A free-form visual description, such as:
   - 一个中国男性，魁梧、武将、正义
   - 一个印度女性，优雅、聪慧、商人
   - 一个北欧男性，年长、粗犷、探险家

The output is a production-ready image-generation prompt.

## Input Interpretation

### Named historical character

When the input is a real historical figure:

1. Identify and disambiguate the figure if necessary.
2. Determine the most representative historical era and cultural context.
3. Infer historically appropriate age, facial features, hairstyle, facial hair, clothing, headwear, weapons, jewelry, accessories, and cultural motifs.
4. Preserve recognizable historical identity while translating it into a stylized strategy-game character.

If historical evidence is uncertain, use historically plausible details rather than inventing false certainty.

### Free-form character description

When the input is descriptive rather than a name, do not force historical attribution.

Automatically derive the stated gender presentation, approximate age, ethnicity/cultural setting, body type, profession/archetype, personality, clothing, accessories, color palette, facial expression, and pose.

If the description includes a culture or historical period, keep the costume and visual details consistent with it. If no period is specified, use a broadly believable interpretation and avoid unnecessary anachronisms.

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
- detailed skin, hair, fabric, leather, and metal
- painterly finish integrated with 3D rendering

### Face and expression

The face is the primary focal point.

Use a memorable, characterful expression appropriate to the input: confident, stern, benevolent, clever, dignified, humorous, determined, contemplative, warm, intimidating, or another fitting expression.

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
- selectable strategy-game Governor portrait feeling

### Character clothing

For named historical figures, use historically appropriate clothing and accessories.

For descriptive inputs, design clothing from the stated occupation, culture, personality, and era.

Use layered materials such as wool, cotton, linen, silk, leather, bronze, iron, steel, wood, jade, gold, and painted fabric where appropriate.

Keep the costume readable at portrait scale.

### Lighting and rendering

- soft studio-like directional light
- gentle rim light
- subtle ambient occlusion
- smooth global illumination
- controlled specular highlights
- soft shadows
- detailed but not gritty skin
- useful warm/cool material separation
- polished game-render presentation
- painterly highlights and controlled edge definition

Avoid harsh photographic lighting and flat vector illustration.

### Background and lower fade

Use a clean pure white background with no environment, architecture, landscape, secondary characters, text, logo, UI, or decorative border.

The lower portion of the portrait should gradually fade into the white background with a soft, feathered silhouette transition. This fade is an important part of the Governor-portrait presentation.

Do not use a hard rectangular crop.

### Color

Use a coherent palette derived from the character. Military characters may use restrained metallic, leather, deep red/brown/blue; scholars muted fabric and warm neutrals; merchants richer textiles and jewelry; ceremonial figures culturally appropriate colors; rulers richer materials and controlled metallic accents.

Do not force one palette onto every character.

## Output Format

Return three sections.

### 1. Character Interpretation

Briefly explain how the input was interpreted. For a named person, include historical identity and representative period. For a description, summarize the inferred visual identity.

### 2. Main Prompt

Write one complete image-generation prompt containing character identity, appearance, expression, costume, accessories, pose, stylized 3D modeling, PBR materials, lighting, white background, soft lower fade, composition, framing, and overall Civilization VI-inspired Governor portrait presentation.

### 3. Negative Prompt

Baseline:

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

Only character-specific identity, costume, expression, accessories, and palette should change.

## Important Distinction

This Governor skill is optimized for compact portrait presentation.

It emphasizes face, personality, caricature, expression, chest/waist-up composition, and soft fade into white.

It is intentionally different from a full-body historical leader portrait skill, which emphasizes complete body silhouette, heroic stance, and full historical costume/equipment.

## Response Behavior

If the user gives only a name, generate the prompt directly.

If the user gives only a descriptive phrase, generate the character directly without unnecessary clarification.

Ask for clarification only when the input is too ambiguous to determine a materially different character design.

## Style Reference

Use Civilization VI as a high-level visual reference for strategy-game character presentation. Do not reproduce proprietary character models or assets.
