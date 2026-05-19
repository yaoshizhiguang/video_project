# Snowstorm Monster Prompt v008 - v001 Main Reference Refine

## 用途

用于继续生成第一集暴风雪怪设定图。该版本承认 v001 候选图是目前最接近主参考的方向：它不是纯灾害墙，也不是人形雪人王，而是一个有清晰角色轮廓的雪云怪物。v008 的目标是在 v001 基础上强化短视频第一眼吸引力，同时避免后来版本出现的老人脸、友善笑脸、王冠、胡子、拳头和过度写实灾害感。

## 核心修正

- 主方向回到 v001：巨大、有压迫感、可识别的雪云怪物，而不是抽象暴风雪墙。
- 保留角色轮廓：发光蓝眼睛、云雾大嘴、模糊粗壮云臂、深色暴风云身体、雪雾和冰晶。
- 增强吸睛点：更强的蓝色内发光、少量漂浮冰晶、清晰暗蓝风暴体块、漂亮雪雾边缘光。
- 控制人格化：不能像老人、雪人王、圣诞老人、巨人、健身怪或友善吉祥物。
- 控制灾害感：不能太写实、太末日、太不可战胜；仍然要像儿童动画里会被误打误撞制服的 boss。
- 服务剧情功能：身体要大、厚、圆、笨重，最终能被巨大雪球自然包成雪人。

## 正向 Prompt

```text
A clean single creature concept art of a giant family-friendly snowstorm monster for a cute Pixar-like animated comedy short film, based on the first successful design direction: a huge readable snow-cloud creature, not a human, not a snowman king, not a realistic disaster wall.

The monster is made of swirling snow, dark navy storm clouds, soft snow mist, and a few beautiful blue ice crystal fragments. It has two bright glowing blue eyes, a wide dark cloud-like mouth, vague bulky cloud-arm shapes, and a thick rounded snowstorm body. The silhouette should feel powerful and boss-like, but also slow, heavy, clumsy, and slightly dumb, like a big animated villain that can accidentally be defeated by a rolling snowball.

Keep the body broad, rounded, and easy to wrap into a giant snowman later: large storm-cloud upper mass, chunky snow-cloud sides, wide snowy lower base, no legs, no feet, no sharp tornado funnel. Add stronger short-video visual appeal with aurora-blue glow inside the cloud body, soft rim light on the snow mist, drifting snow particles, and a small number of floating blue ice crystals around it. The ice crystals are decorative and magical, not armor, not weapons, not a crown.

The expression should be intimidating but not evil: glowing eyes staring down at tiny Antarctic animals, mouth open in a cloudy roar, no teeth, no smile, no friendly grin. It should look like the main boss of episode one, scary enough for the opening crisis but still safe for children and funny enough to become a huge snowman at the end.

Antarctic icebergs frame the lower sides for scale, tiny frightened penguins and seals can appear far below, full silhouette visible, clean centered creature design, stylized Pixar-like 3D animation, icy blue Antarctic palette, cinematic lighting, high quality character concept art, front view, vertical 3:4 composition.
```

## 负向 Prompt

```text
friendly snowman, snowman king, Santa Claus, old man face, human face, humanoid body, human body, giant man, ice giant, storm titan, realistic disaster wall, pure abstract storm cloud, no character face, beard, mustache, eyebrows, hair, crown, helmet, shoulders like a man, muscular arms, fists, hands, fingers, legs, feet, shoes, pants, standing humanoid pose, cute smile, big friendly grin, goofy happy mascot, plush toy, carrot nose, buttons, scarf, weapon, sword, armor, ice armor, crystal armor, full body covered in spikes, sharp teeth, too many teeth, claws, demon, horror, nightmare creature, skull, blood, gore, corpse, zombie, red eyes, realistic tornado, thin tornado funnel, fire, lava, robot, dragon, golem, overly complex silhouette, unreadable clutter, collage, split image, photo overlay, real person, human photo, text, logo, watermark, blurry, low quality
```

## 推荐参数

| 参数 | 建议 |
| --- | --- |
| aspect ratio | 3:4 |
| output | clean creature concept art |
| style strength | 中 |
| variation | 中低 |
| reference | `00_references/monster/images/variations/snowstorm_monster_v001_001.png` |

## 使用说明

- 使用时必须把“正向 Prompt”和“负向 Prompt”分别粘贴到生成工具对应的输入框。
- 如果工具支持参考图，优先上传 `00_references/monster/images/variations/snowstorm_monster_v001_001.png`，并设置较高参考权重。
- 这一版不是重做方向，而是“以 v001 为主参考继续精修”。
- 如果结果又像人，强化 `not a human`、`no legs`、`no feet`、`no humanoid body`，并保留负向里的 `beard`、`crown`、`fists`。
- 如果结果太抽象，强化 `two bright glowing blue eyes`、`wide dark cloud-like mouth`、`vague bulky cloud-arm shapes`。
- 如果结果太友善，强化 `no smile`、`no friendly grin`、`cloudy roar`。
- 如果工具没有单独负向 prompt 输入框，用 `Avoid: ...` 句式表达负向内容，不要直接把负向词当作正向内容粘贴。

## 无负向输入框时的写法

```text
Generate the creature using the positive prompt above.

Avoid: friendly snowman, snowman king, Santa Claus, old man face, human face, humanoid body, human body, giant man, ice giant, storm titan, realistic disaster wall, pure abstract storm cloud, no character face, beard, mustache, eyebrows, hair, crown, helmet, shoulders like a man, muscular arms, fists, hands, fingers, legs, feet, shoes, pants, standing humanoid pose, cute smile, big friendly grin, goofy happy mascot, plush toy, carrot nose, buttons, scarf, weapon, sword, armor, ice armor, crystal armor, full body covered in spikes, sharp teeth, too many teeth, claws, demon, horror, nightmare creature, skull, blood, gore, corpse, zombie, red eyes, realistic tornado, thin tornado funnel, fire, lava, robot, dragon, golem, overly complex silhouette, unreadable clutter, collage, split image, photo overlay, real person, human photo, text, logo, watermark, blurry, low quality.
```

## 生成记录

| 日期 | 模型 | 结果 | 问题 | 下一步 |
| --- | --- | --- | --- | --- |
| 2026-05-17 | 待生成 | 待生成 | 用户纠正：最接近主参考的是 v001，而不是 v008 灾害墙候选图 | 使用 v001 作为参考图继续精修，增强吸睛度但不改变主体方向 |
