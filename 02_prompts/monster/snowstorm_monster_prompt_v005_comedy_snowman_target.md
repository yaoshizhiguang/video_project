# Snowstorm Monster Prompt v005 - Comedy Snowman Target

## 用途

用于生成更贴合第一集剧情功能的暴风雪怪设定图。该版本不再把雪怪当成“史诗冰雪 Boss”，而是定位为“喜剧型灾难反派”：巨大、吓人但笨重，像一团活的暴风雪，最终能被滚雪球自然包成巨大雪人。

## 核心修正

- 怪物不是最终 Boss，而是会被喜剧连锁反应制服的笨重靶子。
- 设计重点是：大、笨、慢、圆、好包裹、能变雪人。
- 整体像圆滚滚乌云雪团，不是冰巨人、风暴泰坦、龙卷风魔王。
- 下半身是宽宽软软的旋转雪雾底座，像蓬松旋转雪堆，不是细长龙卷风漏斗。
- 嘴巴是软椭圆云洞嘴，表情笨笨张开，像在“嗷呜”，不要尖牙和血盆大口。
- 冰晶只能是少量装饰，不能成为主体武器或冰刺盔甲。
- 造型要预埋“会被包成三层雪人”的结构基础。

## 正向 Prompt

```text
A clean single creature concept art of a giant clumsy snowstorm monster for a cute Pixar-like animated comedy short film. The monster is a comedy disaster villain, not an epic final boss. It looks huge and threatening at first glance, but also slow, round, heavy, and a little dumb, like a big target that can be accidentally wrapped into a snowman by a rolling snowball.

The body is made of soft dark storm clouds, fluffy snow piles, swirling snow mist, and a few small icy crystals. The overall silhouette is round and bulky, like a giant living snow-cloud snowman shape: a large rounded upper snow-cloud body, a wider rounded lower snow-cloud base, and soft chunky cloud arms. The lower body is a broad soft swirling snow-cloud base, like a fluffy rotating snow pile, not a sharp tornado funnel, not legs, not feet. It has two glowing blue eyes with a slightly confused goofy expression, and a soft oval cloud-mouth, open like a harmless “aww” roar, no teeth, no sharp mouth edges.

The monster should feel big enough to scare small Antarctic animals, but still family-friendly and funny. It should look easy to cover with snow and transform into a giant harmless snowman later. Ice crystals are only small decorative accents on the cloud body, not armor, not weapons, not sharp spikes. Full silhouette visible, Antarctic icebergs only frame the lower sides for scale and do not block the monster. Clean centered creature design, simple readable shape, icy blue Antarctic color palette, soft snow particles, cute cinematic 3D animation style, high quality character concept art, front view.
```

## 负向 Prompt

```text
epic final boss, storm titan, ice titan, ice giant, wind demon, tornado monster, sharp tornado funnel, realistic tornado, disaster movie, realistic storm, horror monster, scary horror, nightmare creature, evil demon, dragon, golem, muscular body, human body, human legs, two legs, feet, shoes, pants, human lower body, standing humanoid, ice armor, crystal armor, weapon, sharp claws, sharp teeth, too many teeth, blood, gore, skull, corpse, zombie, red eyes, too many sharp spikes, ice spike monster, aggressive monster roar, wide scary mouth, thin body, tall skinny body, overly complex silhouette, unreadable silhouette, collage, split image, photo overlay, real person, human photo, text, logo, watermark, blurry, low quality
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
- 如果工具没有单独负向 prompt 输入框，不要把负向词直接拼到正向 prompt 里；改用 `Avoid: ...` 或 `Do not include: ...`。
- 这一版的重点不是画质，而是剧情功能：雪怪必须像“能被雪球包成雪人”的圆笨靶子。
- 如果结果太史诗，弱化 `threatening`，强化 `comedy disaster villain`、`slow, round, heavy, and a little dumb`。
- 如果结果像龙卷风，强化 `fluffy rotating snow pile` 和 `not a sharp tornado funnel`。
- 如果结果像冰巨人，强化 `living snow-cloud snowman shape`，负向加强 `ice giant`、`storm titan`。

## 无负向输入框时的写法

```text
Generate the creature using the positive prompt above.

Avoid: epic final boss, storm titan, ice titan, ice giant, wind demon, tornado monster, sharp tornado funnel, realistic tornado, disaster movie, realistic storm, horror monster, scary horror, nightmare creature, evil demon, dragon, golem, muscular body, human body, human legs, two legs, feet, shoes, pants, human lower body, standing humanoid, ice armor, crystal armor, weapon, sharp claws, sharp teeth, too many teeth, blood, gore, skull, corpse, zombie, red eyes, too many sharp spikes, ice spike monster, aggressive monster roar, wide scary mouth, thin body, tall skinny body, overly complex silhouette, unreadable silhouette, collage, split image, photo overlay, real person, human photo, text, logo, watermark, blurry, low quality.
```

## 生成记录

| 日期 | 模型 | 结果 | 问题 | 下一步 |
| --- | --- | --- | --- | --- |
| 2026-05-16 | 待填写 | 待生成 | 待记录 | 生成剧情功能对齐的喜剧型笨重雪云怪 |
