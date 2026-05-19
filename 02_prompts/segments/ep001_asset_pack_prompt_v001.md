# Episode 001 Asset Pack Prompt v001

## 用途

用于基于已确认主参考图，生成《咕咕嘎嘎企鹅：滑倒拯救南极》的资产包。当前不再重新设计角色和雪怪，只围绕主参考图制作一致性资产。

## 主参考图

- 咕咕嘎嘎主参考：`00_references/character/images/selected/gugugaga_primary_reference.png`
- 暴风雪怪主参考：`00_references/monster/images/selected/snowstorm_monster_primary_reference.png`

## 输出目录

- 咕咕嘎嘎设定图：`00_references/character/images/model_sheets/`
- 咕咕嘎嘎动作图：`00_references/character/images/pose_sheets/`
- 雪怪设定图：`00_references/monster/images/model_sheets/`
- 雪怪动作图：`00_references/monster/images/pose_sheets/`
- 比例关系图：`00_references/episode_001/scale_lineup/`
- 道具资产：`00_references/episode_001/props/`
- 场景资产：`00_references/episode_001/environments/`
- 特效资产：`00_references/episode_001/vfx/`
- 选中成品：`00_references/episode_001/final_selected/`
- 废稿归档：`00_references/episode_001/rejected/`

## 资产包目标

- 角色设定资产：咕咕嘎嘎三视图、表情、材质细节、比例设定、颜色参考。
- 角色动作资产：咕咕嘎嘎登场、转头、困惑、下决心、滑倒、旋转、撞桶、被卷入雪球、胜利后再次滑倒。
- 怪物设定资产：暴风雪怪三视图、体块结构、冰晶分布、蓝光设定、比例设定。
- 怪物动作资产：暴风雪怪苏醒、升起、咆哮、攻击、困惑、被雪球撞击、半包裹、完全变雪人。
- 道具资产：鱼桶、小鱼、冰锣、冰柱、滚雪球、最终巨大雪人。
- 场景资产：南极冰面、远处冰山、雪山、冰锣区域、开场暴风雪天空、结尾放晴天空。
- 特效资产：暴风雪、蓝色风暴内发光、雪崩、雪球滚动轨迹、冰锣声波。
- 比例资产：咕咕嘎嘎、暴风雪怪、小企鹅、小海豹、鱼桶、雪球的统一尺度关系。

## 雪怪尺度约束

- 雪怪必须是“小动物视角下巨大”，不是“山脉级巨大”。
- 雪怪应约为咕咕嘎嘎高度的 8-12 倍，足够形成危机，但仍能被雪崩雪球包住。
- 雪怪必须明显小于远处雪山和大型冰山，不能比山还高。
- 最终滚雪球应能达到雪怪高度的 1.2-1.5 倍，视觉上可以合理吞没它。
- 任何雪怪设定图、比例图和分镜资产都必须验证“能被雪球包成巨大雪人”这一剧情机制。

## 剧情动作覆盖清单

- Segment 01 危机降临：雪怪苏醒、从冰山后升起、张嘴咆哮、凝聚暴风雪、小动物逃跑、鱼桶滑走。
- Segment 02 主角登场：咕咕嘎嘎叼鱼站立、慢慢转头、眨眼困惑、看见雪怪、表情认真、红围巾被风吹起。
- Segment 03 冲刺滑倒：英雄站姿、迈出第一步、脚底打滑、身体后仰、旋转滑行、保龄球式滚动、惊慌表情、即将撞桶。
- Segment 04 连锁反应：撞飞鱼桶、鱼桶翻滚、小鱼飞散、鱼拍脸、冰柱被砸中、冰柱倾斜、咕咕嘎嘎继续滑走。
- Segment 05 雪崩雪球：冰柱撞冰锣、冰锣声波、雪山震动、雪崩落下、雪球形成、咕咕嘎嘎被卷入雪球、只露脸和红围巾、雪球冲向雪怪。
- Segment 06 反转胜利：雪怪发现雪球、雪怪困惑、雪怪试图阻挡、雪球撞上、雪雾遮屏、雪怪被包裹中、最终巨大雪人形态、鱼插在脸上、小动物欢呼、咕咕嘎嘎得意走路、再次滑倒飞出画面。

## 全局正向 Prompt

```text
Create a clean production asset pack for a cute Pixar-like animated comedy short film called "Gugugaga Penguin Saves Antarctica by Slipping". Use the provided reference images as strict visual anchors:

1. Gugugaga main character reference: keep the same cute round penguin-girl mascot identity, red scarf, black short hair, blue hair clip, penguin hood, big expressive eyes, small body, clumsy and sincere personality.
2. Snowstorm monster main reference: keep the same giant snow-cloud monster identity from the first successful design, with dark storm cloud body, swirling snow mist, blue glowing eyes, cloud-hole mouth, icy crystal accents, bulky snow-cloud silhouette, and creature-scale Antarctic size. The monster is huge compared with Gugugaga and small animals, but clearly smaller than mountains and large icebergs, so a rolling avalanche snowball can wrap it into a giant snowman later.

Do not redesign either character. Do not invent new costumes, new species, new facial structure, or new monster identity. The goal is asset production consistency, not concept redesign.

Generate a complete visual asset sheet with multiple neatly separated panels on a clean light blue or neutral background. Each panel should be clear, readable, and production-friendly. Use a consistent stylized 3D animated look, cute cinematic lighting, icy blue Antarctic color palette, soft snow particles, rounded forms, family-friendly tone, high quality character and environment concept art.

Include the following asset groups:

A. Character scale lineup:
Gugugaga standing next to tiny Antarctic animals, fish bucket, rolling snowball, and the giant snowstorm monster. Keep Gugugaga very small compared to the monster for comedy contrast, but keep the monster about 8-12 times Gugugaga's height and clearly smaller than mountains and large icebergs.

B. Gugugaga character model sheet:
front view, side view, back view, three-quarter view, head close-up, red scarf close-up, blue hair clip close-up, penguin hood detail, color palette swatches, scale note with a fish bucket. Keep the same identity as the reference image.

C. Gugugaga pose sheet:
front view, side view, back view, holding or biting a small fish, confused blink, slow head turn, surprised stare at the monster, determined heroic pose, first-step slipping pose, body leaning backward on ice, spinning like a bowling ball, crashing into a fish bucket, tangled with flying fish, stuck inside a rolling snowball with only face and red scarf visible, proud victory walk, slipping again at the ending.

D. Snowstorm monster model sheet:
front view matching the primary snowstorm monster reference, side view, back view, three-quarter view, close-up of blue glowing eyes, cloud-hole mouth detail, ice crystal accent detail, storm-cloud body material detail, wide snow-mist base detail, size comparison with Gugugaga, one iceberg, and the final rolling snowball. Keep it as the same snow-cloud boss and keep the scale wrap-able by the snowball.

E. Snowstorm monster pose sheet:
front view matching the primary snowstorm monster reference, slight side view, rising from behind icebergs, open cloudy roar, glowing-eye glare, gathering blizzard wind, releasing a snowstorm attack, slow heavy movement pose, looking down at tiny animals, confused reaction to the incoming snowball, trying to block the snowball with soft cloud side masses, being hit by the rolling snowball, half-wrapped transition form, fully wrapped final giant snowman form. Keep the monster as the same snow-cloud boss, not a new design, and do not make it mountain-scale.

F. Prop sheet:
wooden fish bucket in normal state, bucket sliding on ice, bucket flipping in the air, several small silver fish, one fish stuck on a face, ice gong, ice gong mallet or striker shape if needed, leaning ice pillar, cracked ice pillar, small starter snowball, growing rolling snowball, giant rolling snowball large enough to swallow the monster, final giant snowman version of the monster with a fish stuck on its face. Props should be simple, readable, and toy-like.

G. Environment sheet:
Antarctic ice field, distant blue icebergs, snow mountain for avalanche, ice gong area, stormy opening sky, clear happy ending sky. Use horizontal 16:9 cinematic composition references when possible.

H. VFX sheet:
soft blizzard wind, blue glowing storm cracks inside the monster, drifting snow particles, ice cracking, slippery ice streaks, spinning motion smear for Gugugaga, impact snow puffs, fish bucket impact burst, ice gong sound wave rings, snow mountain shake, snow avalanche cloud, rolling snowball motion trail, snowball growth stages, white snow wipe transition, clear-sky reveal glow.

Keep all assets consistent with episode 001 story: the snowstorm monster creates the opening crisis, Gugugaga slips by accident, the chain reaction creates a rolling snowball, and the monster is wrapped into a giant snowman. The tone should be action comedy: danger first, then funny accident, then warm victory.

Full asset sheet, clean layout, separated panels, no text labels embedded in the image unless the tool supports labels cleanly, no watermark.
```

## 全局负向 Prompt

```text
redesigning Gugugaga, changing the main character, realistic penguin, animal-only penguin, adult human, realistic human body, new outfit, missing red scarf, missing blue hair clip, wrong hair, wrong face, different mascot, scary child character, uncanny face, extra limbs, distorted body, gore, blood, horror, dark adult fantasy, realistic photo, live action, photorealistic people, real human photo, collage, split image, photo overlay, text, logo, watermark, blurry, low quality,

redesigning the snowstorm monster, mountain-sized monster, monster larger than mountains, kaiju scale, skyscraper-sized monster, impossible-to-wrap monster, snowman king, Santa Claus, old man face, human face, humanoid giant, muscular arms, fists, hands, fingers, legs, feet, shoes, pants, crown, beard, mustache, eyebrows, hair, ice armor, weapon, sharp teeth, too many teeth, claws, demon, dragon, robot, golem, storm titan, ice titan, living wall, pure abstract storm cloud, realistic tornado, thin tornado funnel, horror monster, nightmare creature, overly complex silhouette, unreadable clutter, full body covered in spikes,

unrelated assets, non-Antarctic setting, desert, city street, forest, volcano, sci-fi spaceship, medieval castle, text-heavy poster, comic panels with speech bubbles, subtitles, title cards
```

## 单独生成：咕咕嘎嘎角色设定图

### 正向 Prompt

```text
Using `00_references/character/images/selected/gugugaga_primary_reference.png` as the strict reference, create a Gugugaga character model sheet for episode 001. This is a production design sheet, not an action sheet. Keep the exact same identity, face, red scarf, blue hair clip, penguin hood, black short hair, round body, cute clumsy personality, and Pixar-like 3D animation style.

Show clearly separated panels: front view, side view, back view, three-quarter view, head close-up, face expression mini row, red scarf detail, blue hair clip detail, penguin hood detail, color palette swatches, and a small scale comparison with a wooden fish bucket. Keep proportions consistent across all views. Clean neutral background, production model sheet layout, no redesign.
```

### 负向 Prompt

```text
realistic penguin, animal-only penguin, adult human, different character, changed face, new outfit, missing red scarf, missing blue hair clip, missing penguin hood, long legs, realistic human body, scary expression, action scene, dynamic motion blur, extra limbs, distorted body, text, watermark, blurry, low quality
```

## 单独生成：角色动作资产

### 正向 Prompt

```text
Using `00_references/character/images/selected/gugugaga_primary_reference.png` as the strict reference, create a Gugugaga character pose sheet for episode 001. Keep the same face, red scarf, blue hair clip, penguin hood, round body, cute clumsy personality, and Pixar-like 3D animation style.

Show separated production-friendly poses covering the full episode:

1. neutral front standing;
2. side standing;
3. back view;
4. holding or biting a small fish;
5. slow head turn toward the monster;
6. confused blink;
7. surprised wide-eyed stare;
8. determined heroic pose before charging;
9. first step forward;
10. foot slipping on ice;
11. body leaning backward with panic;
12. spinning on ice like a bowling ball;
13. sliding fast toward the fish bucket;
14. crashing into the wooden fish bucket;
15. tangled with flying fish;
16. stuck inside a growing rolling snowball with only face and red scarf visible;
17. dizzy face after the snowball impact;
18. proud victory walk;
19. slipping again at the ending and flying out of frame.

Keep all poses as the same character, same proportions, same costume, same face, and same red scarf and blue hair clip. Clean production sheet, consistent proportions, light neutral background, no redesign.
```

### 负向 Prompt

```text
realistic penguin, animal-only penguin, adult human, different character, missing red scarf, missing blue hair clip, new outfit, changed face, long legs, scary expression, extra limbs, distorted body, text, watermark, blurry, low quality
```

## 单独生成：雪怪动作资产

### 正向 Prompt

```text
Using `00_references/monster/images/selected/snowstorm_monster_primary_reference.png` as the strict reference, create a snowstorm monster production pose sheet for episode 001. Keep the same giant snow-cloud boss identity, dark storm cloud body, snow mist, blue glowing eyes, cloud-hole mouth, icy crystal accents, bulky readable silhouette, and creature-scale Antarctic size. The monster should feel huge next to Gugugaga, penguins, and seals, but it must be clearly smaller than nearby mountains and large icebergs.

Show separated production-friendly poses covering the full episode:

1. neutral front view matching the primary reference;
2. slight side view;
3. back view showing cloud mass and ice crystal placement;
4. rising from behind smaller icebergs;
5. glowing-eye glare toward tiny animals;
6. open cloudy roar;
7. gathering blizzard wind inside its body;
8. releasing a snowstorm attack;
9. slow heavy movement pose;
10. looking down at Gugugaga;
11. confused reaction when Gugugaga slips instead of fighting;
12. noticing the giant incoming snowball;
13. trying to block the snowball with soft cloud side masses, not hands or fists;
14. impact moment as the rolling snowball hits;
15. half-wrapped transition form with snow covering the lower body;
16. mostly wrapped form with only glowing eyes and mouth still visible;
17. final harmless giant snowman form with a fish stuck on its face;
18. dazed defeated expression after the sky clears.

The rolling snowball should be large enough to plausibly swallow the monster, about 1.2-1.5 times the monster height. Do not redesign the monster. Keep it powerful but clumsy, family-friendly, and suitable for a cute animated comedy short film.
```

### 负向 Prompt

```text
mountain-sized monster, monster larger than mountains, kaiju scale, skyscraper-sized monster, impossible-to-wrap monster, snowman king, crown, beard, mustache, eyebrows, old man face, human face, muscular arms, fists, hands, fingers, legs, feet, ice armor, weapon, sharp teeth, horror monster, realistic tornado, storm titan, pure disaster wall, new monster design, text, watermark, blurry, low quality
```

## 单独生成：雪怪设定图

最新生产版请优先使用：

- Prompt 位置：`02_prompts/prompt_library.md` 的“单独生成：雪怪设定图（已选定 v003）”
- 设定图结果：`00_references/monster/images/model_sheets/ep001_snowstorm_monster_model_sheet_v003_production.png`
- 选定说明：v003 是雪怪生产设定图，不是主参考图；主参考仍然是 `00_references/monster/images/selected/snowstorm_monster_primary_reference.png`。
- 注意：该 prompt 是资产设定图 / 比例 lineup，可提到咕咕嘎嘎；不要直接复制到咕咕嘎嘎未出场的剧情镜头里。

## 单独生成：道具与场景资产

### 正向 Prompt

```text
Create a clean production asset sheet for episode 001 props and Antarctic environments in a cute Pixar-like 3D animated style. Include separated props: wooden fish bucket, small silver fish, ice gong, leaning ice pillar, rolling snowball, final giant snowman version of the snowstorm monster with a fish stuck on its face. Include separated environment thumbnails: Antarctic ice field, blue icebergs, snow mountain avalanche area, ice gong area, stormy opening sky, clear happy ending sky.

Keep everything simple, readable, toy-like, icy blue, family-friendly, and consistent with the story "Gugugaga Penguin Saves Antarctica by Slipping".
```

### 负向 Prompt

```text
realistic photo, live action, human photo, city, forest, desert, volcano, sci-fi, medieval, horror, gore, blood, complex clutter, unreadable props, text, logo, watermark, blurry, low quality
```

## 推荐使用方式

- 如果生成工具支持多图参考，上传 `gugugaga_primary_reference.png` 和 `snowstorm_monster_primary_reference.png`。
- 推荐先生成“咕咕嘎嘎角色设定图”和“雪怪设定图”，再生成动作资产。
- 角色设定图和角色动作资产只上传咕咕嘎嘎主参考。
- 雪怪设定图和雪怪动作资产只上传雪怪主参考。
- 道具与场景资产可以不上传角色图，避免角色污染道具。
- 每次生成后先检查一致性，再检查画质；不要因为某张图更酷就接受角色重设计。

## 生成记录

| 日期 | 模型 | 结果 | 问题 | 下一步 |
| --- | --- | --- | --- | --- |
| 2026-05-17 | 待生成 | 待生成 | 用户确认雪怪 v001 作为主参考图 | 使用咕咕嘎嘎主参考和雪怪主参考生成 episode 001 资产包 |
