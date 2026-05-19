# Snowstorm Monster Prompt v004 - Clean Creature Concept

## 用途

用于修正 v003 生成失败的问题。v003 虽然解决了“不要腿”的方向，但模型把画面生成成了疑似照片拼贴 / 真人暗部遮挡 / 画面污染，雪怪主体消失，不能作为设定图。v004 目标是回到干净、单一、完整的暴风雪怪概念图。

## 核心修正

- 必须是单一完整雪怪设定图，不能是拼贴、分屏、照片叠加或遮挡画面。
- 保留 v001 的压迫感：巨大、从冰山后升起、像活的暴风雪。
- 避免 v002 的腿部问题：下半身是旋转雪云 / 雪雾云团，不是腿和脚。
- 避免 v003 的画面污染：不要真人、衣服、皮肤、照片边框、黑色遮挡、裁切拼贴。
- 保留两只蓝色发光眼睛、云雾状大嘴、粗壮雪云手臂、冰晶点缀。
- 画面要 clean creature concept art，主体居中，完整可读。

## 正向 Prompt

```text
A clean single creature concept art of a giant family-friendly snowstorm monster for a cute cinematic animated short film. One complete monster only, centered in the frame, full body visible, no collage, no split image, no photo overlay. The monster rises from behind Antarctic icebergs like a massive living blizzard, made entirely of swirling snow, dark storm clouds, icy crystals, and soft snow mist. It has two glowing blue eyes, a wide cloud-like mouth, a huge powerful storm-cloud torso, and vague bulky snow-cloud arms. The lower body dissolves into a swirling snow cloud base and storm mist, not legs, not feet, not human lower body. The silhouette is huge, intimidating, readable, and powerful, with strong scale and pressure, but still safe for children and slightly clumsy like a bulky animated villain. Add icy crystals as dramatic accents around the shoulders and cloud body, moderate amount only. Stylized Pixar-like 3D animation, icy blue Antarctic lighting, volumetric snow particles, cinematic rim light, high quality creature design sheet, front view.
```

## 负向 Prompt

```text
collage, split image, photo overlay, human photo, real person, skin, hair, clothing, pants, black frame, black border, dark block, cropped body, partial image, duplicated scene, multiple panels, mixed images, unrelated foreground, human legs, two legs, feet, shoes, human lower body, standing humanoid, muscular body, bodybuilder, pure giant, ice giant, troll, yeti, ape, realistic human anatomy, horror monster, scary horror, nightmare creature, bloody, gore, skull, corpse, zombie, sharp teeth, too many teeth, disgusting, realistic disaster, realistic tornado only, red eyes, multiple heads, extra limbs, too many sharp spikes, ice spike monster, complex armor, weapon, fire, lava, overly cute, tiny body, unreadable silhouette, text, logo, watermark, blurry, low quality
```

## 推荐参数

| 参数 | 建议 |
| --- | --- |
| aspect ratio | 1:1 或 3:4 |
| output | clean creature concept art |
| style strength | 中 |
| variation | 低到中低 |

## 使用说明

- 使用时必须把“正向 Prompt”和“负向 Prompt”分别粘贴到生成工具对应的输入框。
- 如果工具没有单独的负向 prompt 输入框，不要把负向词直接拼到正向 prompt 里；改用明确句式：`Avoid: ...` 或 `Do not include: ...`。
- 如果工具支持 negative prompt，负向输入框里只填负向词，不要加进正向描述。
- 这一版优先解决 v003 的“画面污染 / 拼贴 / 真人遮挡”问题。
- 如果仍出现照片拼贴，继续强化 `clean single creature concept art`、`one complete monster only`、`no collage`。
- 如果又出现腿，强化 `lower body dissolves into a swirling snow cloud base` 和负向词 `human legs, two legs, feet`。
- 如果压迫感不足，强化 `massive living blizzard`、`strong scale and pressure`、`towering behind Antarctic icebergs`。

## 无负向输入框时的写法

```text
Generate the creature using the positive prompt above.

Avoid: collage, split image, photo overlay, human photo, real person, skin, hair, clothing, pants, black frame, black border, dark block, cropped body, partial image, duplicated scene, multiple panels, mixed images, unrelated foreground, human legs, two legs, feet, shoes, human lower body, standing humanoid, muscular body, bodybuilder, pure giant, ice giant, troll, yeti, ape, realistic human anatomy, horror monster, scary horror, nightmare creature, bloody, gore, skull, corpse, zombie, sharp teeth, too many teeth, disgusting, realistic disaster, realistic tornado only, red eyes, multiple heads, extra limbs, too many sharp spikes, ice spike monster, complex armor, weapon, fire, lava, overly cute, tiny body, unreadable silhouette, text, logo, watermark, blurry, low quality.
```

## 生成记录

| 日期 | 模型 | 结果 | 问题 | 下一步 |
| --- | --- | --- | --- | --- |
| 2026-05-16 | 待填写 | 待生成 | 待记录 | 生成干净、单一、完整且无腿部出戏的雪怪设定图 |
