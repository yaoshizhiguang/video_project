# Snowstorm Monster Prompt v007 - Living Blizzard Wall

## 用途

用于重置暴风雪怪方向。上一版结果太像友善的人形雪人王：有眉毛、胡子、拳头、肩膀和清晰笑脸，导致它既不够像 boss，也和“南极暴风雪怪”设定违和。v007 改为“活的南极暴风雪墙”：它首先是自然灾害，其次才是可读角色。

## 核心修正

- 去人格化：不要胡子、眉毛、拳头、肩膀、肌肉、衣服、王冠和人类五官。
- 怪物主体是移动的暴风雪墙、雪雾巨浪、乌云旋涡和冰晶碎片，不是雪人、巨人或老爷爷。
- 只保留最低限度的角色识别：两只冷蓝色发光眼睛、一个模糊云洞嘴、一个巨大压迫性的整体轮廓。
- 视觉记忆点改成“灾害形状”：像雪崩海啸一样的宽大雪墙、内部旋涡、蓝色极光裂纹、漂浮冰晶碎片。
- 仍要服务剧情：整体宽、圆、厚、慢，最后能被巨大雪球包住并变成笨拙雪人。
- 风格保持儿童动画可接受的危机感，不走恐怖、恶魔、写实灾难片方向。

## 正向 Prompt

```text
A clean single creature concept art of the Antarctic Living Blizzard Wall, a non-humanoid snowstorm boss for a cute Pixar-like animated comedy short film. The creature should feel like a natural disaster that has barely formed a face, not like a man, not like a snowman, not like a friendly old king.

Design it as a huge moving wall of blizzard snow, dark storm clouds, rolling snow mist, and icy wind, with a broad heavy silhouette like a slow snow avalanche wave. The body is wide, thick, rounded, and heavy, with no legs and no human torso. It has no arms shaped like fists; only large uneven cloud masses and snow gusts can extend from the sides. The lower body is a broad rolling snowbank base, easy to wrap into a giant snowman later, not a tornado funnel.

Give it only minimal facial features: two cold aurora-blue glowing eyes buried inside the storm, and a vague dark cloud-hole mouth. The expression should be threatening and unreadable, like a storm staring at tiny animals, but still safe for a family animated comedy. Add memorable disaster-shaped visual anchors: a wide snow-tsunami silhouette, swirling internal storm rings, thin aurora-blue glowing cracks inside the cloud, and a few floating blue ice crystal shards caught in the wind. Keep the design simple, iconic, readable, and not human.

Antarctic icebergs and tiny frightened animals can appear at the bottom for scale, but the monster remains the clear centered subject. Cute cinematic 3D animation style, icy blue and dark navy palette, soft snow particles, dramatic backlight, high quality creature concept art, front three-quarter view, full silhouette visible.
```

## 负向 Prompt

```text
friendly snowman, Santa Claus, old man face, human face, human body, humanoid boss, giant man, ice giant, storm king, king, beard, mustache, eyebrows, hair, crown, helmet, shoulders, muscular arms, fists, hands, fingers, legs, feet, shoes, pants, standing pose, cute smile, big friendly grin, goofy happy face, round mascot, plush toy, snowman with face, carrot nose, buttons, scarf, weapon, armor, ice armor, crystal armor, too many spikes, demon, horror, skull, blood, gore, realistic disaster photo, realistic tornado, thin tornado funnel, dragon, golem, robot, overly complex silhouette, unreadable clutter, collage, split image, photo overlay, real person, human photo, text, logo, watermark, blurry, low quality
```

## 推荐参数

| 参数 | 建议 |
| --- | --- |
| aspect ratio | 3:4 或 9:16 |
| output | clean non-humanoid creature concept art |
| style strength | 中 |
| variation | 中 |

## 使用说明

- 使用时必须把“正向 Prompt”和“负向 Prompt”分别粘贴到生成工具对应的输入框。
- 这版的目标不是更凶的人形 boss，而是“暴风雪本身像 boss”。
- 如果结果仍像人，强化 `non-humanoid`、`not like a man`、`no human torso`，并在负向 prompt 中保留 `beard`、`eyebrows`、`fists`、`shoulders`。
- 如果结果太抽象看不出角色，强化 `two cold aurora-blue glowing eyes` 和 `vague dark cloud-hole mouth`。
- 如果工具没有单独负向 prompt 输入框，用 `Avoid: ...` 句式表达负向内容，不要直接把负向词当作正向内容粘贴。

## 无负向输入框时的写法

```text
Generate the creature using the positive prompt above.

Avoid: friendly snowman, Santa Claus, old man face, human face, human body, humanoid boss, giant man, ice giant, storm king, king, beard, mustache, eyebrows, hair, crown, helmet, shoulders, muscular arms, fists, hands, fingers, legs, feet, shoes, pants, standing pose, cute smile, big friendly grin, goofy happy face, round mascot, plush toy, snowman with face, carrot nose, buttons, scarf, weapon, armor, ice armor, crystal armor, too many spikes, demon, horror, skull, blood, gore, realistic disaster photo, realistic tornado, thin tornado funnel, dragon, golem, robot, overly complex silhouette, unreadable clutter, collage, split image, photo overlay, real person, human photo, text, logo, watermark, blurry, low quality.
```

## 生成记录

| 日期 | 模型 | 结果 | 问题 | 下一步 |
| --- | --- | --- | --- | --- |
| 2026-05-17 | 待生成 | 待生成 | v006/v007 候选图太拟人、太友善、像雪人王而不是暴风雪怪 | 使用非人形“活的暴风雪墙”方向重新生成 |
