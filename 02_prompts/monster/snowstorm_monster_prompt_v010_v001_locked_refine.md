# Snowstorm Monster Prompt v010 - v001 Locked Refine

## 用途

用于基于 `snowstorm_monster_v001_001.png` 做小幅强化。该版本不重新设计怪物，不新增 king、titan、wall、snowman 等新身份，只让 v001 的同一个雪云 Boss 变得更高级。

## 设计约束

- 主参考：`00_references/monster/images/variations/snowstorm_monster_v001_001.png`
- 规格表：`02_prompts/monster/snowstorm_monster_design_spec_v001.md`
- 核心策略：`based on the first successful design, only refine the same snow-cloud boss`
- 惊艳来源：光效、体量、蓝色内发光、冰晶漂浮、风雪氛围
- 禁止来源：王冠、胡子、肌肉、尖刺、复杂表情、新身份

## 正向 Prompt

```text
A clean single creature concept art of a giant family-friendly snowstorm monster for a cute Pixar-like animated comedy short film, based on the first successful snow-cloud monster design direction. Based on the first successful design, only refine the same snow-cloud boss.

The creature is a huge readable snow-cloud boss, not a human, not a snowman king, not a storm titan, and not a realistic disaster wall. It should feel like a giant living blizzard creature with a clear character face, but still made entirely of snow, storm clouds, mist, and wind.

The monster has a thick rounded snowstorm body, a broad heavy upper cloud mass, vague bulky snow-cloud side masses, and a wide soft rolling snow-mist base. No legs, no feet, no human torso, no sharp tornado funnel. The side masses should feel like uneven cloud bulges and snow gusts, not arms, not fists, not hands.

It has two bright cold blue glowing eyes buried in the snow cloud, and one wide dark cloud-hole mouth open in a cloudy roar. The expression is intimidating but not evil, like a slow heavy dumb animated boss staring down at tiny Antarctic animals. No smile, no teeth, no eyebrows, no beard, no mustache, no crown, no human face details.

The silhouette should be simple, iconic, broad, heavy, readable, and memorable. It must look powerful enough to create the opening crisis, but still clumsy and soft enough that a rolling snowball could accidentally wrap it into a giant snowman later.

Add stronger short-video visual appeal: subtle aurora-blue glow inside the cloud body, thin blue glowing cracks inside the storm cloud, soft rim light on the snow mist, drifting snow particles, and a few floating blue ice crystal fragments caught in the wind. The crystals are decorative magical fragments, not armor, not spikes, not a crown.

Antarctic icebergs frame the lower sides for scale, with tiny frightened penguins and seals far below. The monster remains the clear centered subject. Full silhouette visible, front view, vertical 3:4 composition, stylized Pixar-like 3D animation, icy blue Antarctic palette, cinematic lighting, high quality creature concept art.
```

## 负向 Prompt

```text
friendly snowman, snowman king, Santa Claus, old man face, human face, humanoid body, giant man, ice giant, storm titan, living wall, realistic disaster wall, pure abstract storm cloud, no character face, beard, mustache, eyebrows, hair, crown, helmet, human shoulders, muscular arms, fists, hands, fingers, legs, feet, shoes, pants, standing humanoid pose, cute smile, big friendly grin, goofy happy mascot, plush toy, carrot nose, buttons, scarf, weapon, sword, armor, ice armor, crystal armor, full body covered in spikes, sharp teeth, too many teeth, claws, demon, horror, nightmare creature, skull, blood, gore, corpse, zombie, red eyes, realistic tornado, thin tornado funnel, fire, lava, robot, dragon, golem, overly complex silhouette, unreadable clutter, collage, split image, photo overlay, real person, human photo, text, logo, watermark, blurry, low quality
```

## 推荐参数

| 参数 | 建议 |
| --- | --- |
| reference image | `00_references/monster/images/variations/snowstorm_monster_v001_001.png` |
| reference weight | 高 |
| aspect ratio | 3:4 |
| output | clean creature concept art |
| variation | 低 |
| style strength | 中 |

## 使用说明

- 使用时必须把“正向 Prompt”和“负向 Prompt”分别粘贴到生成工具对应的输入框。
- 如果工具支持参考图，必须上传 `00_references/monster/images/variations/snowstorm_monster_v001_001.png`，并设置较高参考权重。
- 这版目标不是“更惊艳的新怪物”，而是“v001 变得更高级”。
- 如果结果像新物种，说明自由度过高：降低 variation，提高参考图权重。
- 如果结果像人，检查是否出现拳头、手掌、肩膀、腿、脚；这些都应直接判失败。
- 如果工具没有单独负向 prompt 输入框，用 `Avoid: ...` 句式表达负向内容，不要直接把负向词当作正向内容粘贴。

## 无负向输入框时的写法

```text
Generate the creature using the positive prompt above.

Avoid: friendly snowman, snowman king, Santa Claus, old man face, human face, humanoid body, giant man, ice giant, storm titan, living wall, realistic disaster wall, pure abstract storm cloud, no character face, beard, mustache, eyebrows, hair, crown, helmet, human shoulders, muscular arms, fists, hands, fingers, legs, feet, shoes, pants, standing humanoid pose, cute smile, big friendly grin, goofy happy mascot, plush toy, carrot nose, buttons, scarf, weapon, sword, armor, ice armor, crystal armor, full body covered in spikes, sharp teeth, too many teeth, claws, demon, horror, nightmare creature, skull, blood, gore, corpse, zombie, red eyes, realistic tornado, thin tornado funnel, fire, lava, robot, dragon, golem, overly complex silhouette, unreadable clutter, collage, split image, photo overlay, real person, human photo, text, logo, watermark, blurry, low quality.
```

## 生成记录

| 日期 | 模型 | 结果 | 问题 | 下一步 |
| --- | --- | --- | --- | --- |
| 2026-05-17 | 待生成 | 待生成 | v009 证明 v008 仍会跑向云团肌肉巨人 | 使用 v010，锁定 v001，只允许小幅强化光效、体量、蓝色内发光、冰晶漂浮和风雪氛围 |
