# Episode 001 Keyframe Prompts v001

## 用途

用于生成《咕咕嘎嘎企鹅：滑倒拯救南极》第一集 60 秒短片的关键帧。第一幕提供 3 张关键帧：风平浪静、雪怪诞生、雪怪攻击；其余段落每段 2 张关键帧，共 13 张。

## 实际引用资产

- 咕咕嘎嘎主参考：`00_references/character/images/selected/gugugaga_primary_reference.png`
- 咕咕嘎嘎设定图：`00_references/character/images/model_sheets/ep001_gugugaga_model_sheet_v001.png`
- 咕咕嘎嘎动作图：`00_references/character/images/pose_sheets/ep001_gugugaga_pose_sheet_v002.png`
- 雪怪主参考：`00_references/monster/images/selected/snowstorm_monster_primary_reference.png`
- 雪怪比例校准设定图：`00_references/monster/images/model_sheets/ep001_snowstorm_monster_model_sheet_v002_scale_corrected.png`
- 雪怪动作图：`00_references/monster/images/pose_sheets/ep001_snowstorm_monster_pose_sheet_v001.png`

## 资产使用规则

- 生成包含咕咕嘎嘎的关键帧时，上传咕咕嘎嘎主参考、设定图、动作图。
- 生成包含雪怪的关键帧时，上传雪怪主参考、设定图、动作图。
- 同时出现两者时，上传全部 6 张参考图，但提示词必须强调“do not redesign either character”。
- 道具、场景、VFX 暂无独立图片资产时，用本文件文字描述约束：鱼桶、小鱼、冰锣、冰柱、雪球、南极冰面、雪山、暴风雪、雪崩、白雪遮屏。
- 雪怪尺度必须锁定：直接按照雪怪比例校准设定图中的冰山、雪山和小动物比例来画；雪怪要明显小于远处雪山和大型冰山，最终雪球可达到雪怪高度的 1.2-1.5 倍并吞没它。
- 雪怪出场和攻击帧必须参考 `ep001_snowstorm_monster_model_sheet_v002_scale_corrected.png` 中的冰山比例：雪怪可以比小动物巨大，但不能超过或压倒大型冰山与远处雪山。

## 输出目录

- KF01A 平静南极开场：`03_keyframes/episode_001/KF01A_calm_antarctica/`
- KF01B 雪怪诞生：`03_keyframes/episode_001/KF01B_monster_birth/`
- KF01C 雪怪攻击：`03_keyframes/episode_001/KF01C_monster_first_attack/`
- KF02A 咕咕嘎嘎登场：`03_keyframes/episode_001/KF02A_gugugaga_appears/`
- KF02B 认真准备冲刺：`03_keyframes/episode_001/KF02B_gugugaga_charge_ready/`
- KF03A 英雄迈步：`03_keyframes/episode_001/KF03A_hero_first_step/`
- KF03B 第一秒滑倒：`03_keyframes/episode_001/KF03B_first_slip/`
- KF04A 撞飞鱼桶：`03_keyframes/episode_001/KF04A_bucket_impact/`
- KF04B 冰柱倒向冰锣：`03_keyframes/episode_001/KF04B_ice_pillar_to_gong/`
- KF05A 冰锣引发雪崩：`03_keyframes/episode_001/KF05A_gong_avalanche/`
- KF05B 雪球冲向雪怪：`03_keyframes/episode_001/KF05B_snowball_to_monster/`
- KF06A 雪球撞上雪怪：`03_keyframes/episode_001/KF06A_snowball_hits_monster/`
- KF06B 南极最大雪人：`03_keyframes/episode_001/KF06B_final_snowman/`

## 生成文件命名

- 候选图：`ep001_<keyframe_id>_candidate_v001.png`
- 修正版：`ep001_<keyframe_id>_candidate_v002.png`
- 选中图：`ep001_<keyframe_id>_selected.png`
- 例子：`ep001_KF03B_candidate_v001.png`、`ep001_KF03B_selected.png`

## 全局正向 Prompt

```text
Create a horizontal 16:9 cinematic keyframe for a cute Pixar-like 3D animated comedy short film, "Gugugaga Penguin Saves Antarctica by Slipping". Use the uploaded reference images as strict visual anchors. Keep Gugugaga exactly consistent with the reference: cute round penguin-girl mascot, red scarf, blue hair clip, penguin hood, black short hair, big expressive eyes, small clumsy body. Keep the snowstorm monster exactly consistent with the reference: living snow-cloud boss, dark storm cloud body, blue glowing eyes, cloud-hole mouth, ice crystal accents, wide snow-mist base, powerful but clumsy.

Do not redesign either character. Keep a family-friendly animated comedy tone: danger first, funny accident, warm victory. Use icy blue Antarctic color palette, cinematic lighting, soft snow particles, readable silhouettes, strong depth, clean composition, high quality stylized 3D animation.
```

## 全局负向 Prompt

```text
redesigning Gugugaga, changing the main character, realistic penguin, animal-only penguin, adult human, realistic human body, new outfit, missing red scarf, missing blue hair clip, wrong hair, wrong face, different mascot, scary child character, uncanny face, extra limbs, distorted body, photorealistic people, live action, collage, split image, photo overlay,

redesigning the snowstorm monster, mountain-sized monster, monster larger than mountains, kaiju scale, skyscraper-sized monster, impossible-to-wrap monster, snowman king, Santa Claus, old man face, human face, humanoid giant, muscular arms, fists, hands, fingers, legs, feet, crown, beard, mustache, eyebrows, hair, ice armor, weapon, sharp teeth, claws, demon, dragon, robot, golem, storm titan, living wall, pure abstract storm cloud, realistic tornado, thin tornado funnel, horror monster, nightmare creature,

text, logo, watermark, subtitles, speech bubbles, title card, unreadable clutter, blurry, low quality, wrong aspect ratio, vertical composition
```

## KF01A Segment 01 起始：平静南极开场

### 输出目录

- `03_keyframes/episode_001/KF01A_calm_antarctica/`

### 使用资产

- `00_references/monster/images/selected/snowstorm_monster_primary_reference.png`
- `00_references/monster/images/model_sheets/ep001_snowstorm_monster_model_sheet_v002_scale_corrected.png`

### 正向 Prompt

```text
Horizontal 16:9 cinematic wide shot. Antarctica is calm and peaceful before the crisis: pale blue sky, soft sunlight, glossy quiet ice field, distant snow mountains, and large blue icebergs framing the horizon. Tiny penguins and seals relax on the ice, a wooden fish bucket sits still near them, no storm yet. The composition should clearly establish normal peaceful life before the monster appears. Use the iceberg scale from the uploaded snowstorm monster scale-corrected model sheet as the world reference, but do not show the monster yet. Clean readable family-friendly Pixar-like 3D animation, icy blue palette, calm atmosphere.
```

### 负向 Prompt

```text
snowstorm monster visible, dark storm already present, panic already happening, mountain-sized monster, monster larger than mountains, kaiju scale, realistic disaster wall, pure tornado, human giant, snowman king, crown, beard, old man face, horror, blood, text, watermark, vertical image
```

## KF01B Segment 01 中段：雪怪诞生

### 输出目录

- `03_keyframes/episode_001/KF01B_monster_birth/`

### 使用资产

- `00_references/monster/images/selected/snowstorm_monster_primary_reference.png`
- `00_references/monster/images/model_sheets/ep001_snowstorm_monster_model_sheet_v002_scale_corrected.png`
- `00_references/monster/images/pose_sheets/ep001_snowstorm_monster_pose_sheet_v001.png`
- 本帧不要上传咕咕嘎嘎参考图；咕咕嘎嘎此时还没有出场。

### 正向 Prompt

```text
Horizontal 16:9 keyframe. The peaceful Antarctic scene begins to change: the pale blue sky darkens from one side, wind picks up, snow mist curls along the ice, and tiny penguins and seals look upward in confusion before panic starts. The snowstorm monster is being born behind mid-sized blue icebergs, rising out of swirling snow clouds: only the upper snow-cloud body, blue glowing eyes, cloud-hole mouth silhouette, drifting ice crystals, and wide misty base are visible. Use the uploaded scale-corrected monster model sheet as the strict visual scale reference: follow the iceberg and animal size relationships shown in that reference image, keeping the monster huge compared with small Antarctic animals but clearly smaller than large icebergs and far snow mountains. Do not show Gugugaga in this frame; the main character has not appeared yet. This is the birth/reveal moment, not the attack yet. Cinematic suspense, family-friendly Pixar-like 3D animation.
```

### 负向 Prompt

```text
Gugugaga visible, main character visible, red scarf, blue hair clip, hero penguin, monster attacking already, shattered iceberg already, mountain-sized monster, monster larger than large icebergs, monster larger than far snow mountains, ignoring the scale reference, kaiju scale, ice titan, muscular arms, fists, hands, fingers, legs, feet, crown, beard, sharp teeth, scary horror, realistic tornado, text, logo, watermark
```

## KF01C Segment 01 结尾：雪怪第一次攻击

### 输出目录

- `03_keyframes/episode_001/KF01C_monster_first_attack/`

### 使用资产

- `00_references/monster/images/selected/snowstorm_monster_primary_reference.png`
- `00_references/monster/images/model_sheets/ep001_snowstorm_monster_model_sheet_v002_scale_corrected.png`
- `00_references/monster/images/pose_sheets/ep001_snowstorm_monster_pose_sheet_v001.png`

### 正向 Prompt

```text
Horizontal 16:9 keyframe. The snowstorm monster has fully emerged on the Antarctic ice field and performs its first attack. Use the uploaded scale-corrected monster model sheet as the strict visual scale reference: follow the iceberg, snow mountain, and small animal size relationships shown in that reference image, keeping the monster huge compared with penguins and seals but clearly smaller than large icebergs and far snow mountains. From its wide dark cloud-hole mouth and swirling storm body, a concentrated blue-white blizzard blast shoots sideways across the frame and shatters a small nearby iceberg into sparkling ice chunks. Tiny penguins and seals flee below, a wooden fish bucket slides across the ice, snow dust and ice fragments fly through the air. Clear attack action, readable cause and effect, dangerous but family-friendly Pixar-like animated comedy.
```

### 负向 Prompt

```text
monster being born only, no attack, mountain-sized monster, monster larger than large icebergs, monster larger than far snow mountains, ignoring the scale reference, ice titan, muscular arms, fists, hands, fingers, legs, feet, crown, beard, sharp teeth, scary horror, realistic tornado, text, logo, watermark
```

## KF02A Segment 02 起始：咕咕嘎嘎登场

### 输出目录

- `03_keyframes/episode_001/KF02A_gugugaga_appears/`

### 使用资产

- `00_references/character/images/selected/gugugaga_primary_reference.png`
- `00_references/character/images/model_sheets/ep001_gugugaga_model_sheet_v001.png`

### 正向 Prompt

```text
Horizontal 16:9 medium close-up. Gugugaga stands alone on shiny Antarctic ice, cute round penguin-girl mascot with red scarf, blue hair clip, penguin hood, black short hair, big innocent eyes, holding a tiny silver fish in its beak. The red scarf flutters lightly in the cold wind. Background is soft focus: dark storm sky and the snowstorm monster far away as a blurred threat. Comedic pause, innocent expression, Pixar-like 3D animation, icy blue palette.
```

### 负向 Prompt

```text
realistic penguin, normal animal penguin, missing red scarf, missing blue hair clip, human body, adult human, different costume, scary face, text, watermark
```

## KF02B Segment 02 结尾：认真准备冲刺

### 输出目录

- `03_keyframes/episode_001/KF02B_gugugaga_charge_ready/`

### 使用资产

- `00_references/character/images/selected/gugugaga_primary_reference.png`
- `00_references/character/images/pose_sheets/ep001_gugugaga_pose_sheet_v002.png`
- `00_references/monster/images/selected/snowstorm_monster_primary_reference.png`

### 正向 Prompt

```text
Horizontal 16:9 low-angle comedic hero shot. Gugugaga has turned toward the distant snowstorm monster and suddenly looks determined, tiny body leaning forward as if about to charge. Red scarf flies dramatically, blue hair clip visible, penguin hood unchanged. The monster looms far behind but remains out of focus and correctly scaled, much smaller than far mountains. The mood is mock-heroic: epic lighting on a very clumsy tiny hero, Pixar-like 3D animation.
```

### 负向 Prompt

```text
changed character, long legs, human warrior, weapon, armor, missing scarf, missing hair clip, realistic photo, monster larger than mountains, text, watermark
```

## KF03A Segment 03 起始：英雄迈步

### 输出目录

- `03_keyframes/episode_001/KF03A_hero_first_step/`

### 使用资产

- `00_references/character/images/selected/gugugaga_primary_reference.png`
- `00_references/character/images/pose_sheets/ep001_gugugaga_pose_sheet_v002.png`

### 正向 Prompt

```text
Horizontal 16:9 keyframe. Gugugaga starts the heroic charge on slick Antarctic ice, one tiny foot stepping forward, eyes focused, red scarf streaming behind. The pose should feel brave but slightly ridiculous because the character is very small and round. Camera low and close to the ice, showing slippery reflections and faint skid lines. Distant storm clouds and blue snow particles in the background. Cute Pixar-like 3D animation, action comedy tone.
```

### 负向 Prompt

```text
realistic penguin, human legs, new outfit, missing scarf, missing blue hair clip, weapon, battle armor, scary expression, text, watermark
```

## KF03B Segment 03 结尾：第一秒滑倒

### 输出目录

- `03_keyframes/episode_001/KF03B_first_slip/`

### 使用资产

- `00_references/character/images/selected/gugugaga_primary_reference.png`
- `00_references/character/images/pose_sheets/ep001_gugugaga_pose_sheet_v002.png`

### 正向 Prompt

```text
Horizontal 16:9 slapstick action keyframe. Gugugaga slips immediately on the glossy ice, tiny feet flying upward, round body spinning like a bowling ball, red scarf spiraling around, eyes wide in panic. Motion smear and snow sparkles emphasize speed, but the face and costume remain recognizable. A wooden fish bucket is visible ahead on the ice as the next collision target. Funny Pixar-like 3D animation, clean readable action.
```

### 负向 Prompt

```text
distorted body, extra limbs, changed face, missing red scarf, missing blue hair clip, realistic motion blur hiding character, horror, text, watermark
```

## KF04A Segment 04 起始：撞飞鱼桶

### 输出目录

- `03_keyframes/episode_001/KF04A_bucket_impact/`

### 使用资产

- `00_references/character/images/selected/gugugaga_primary_reference.png`
- `00_references/character/images/pose_sheets/ep001_gugugaga_pose_sheet_v002.png`

### 正向 Prompt

```text
Horizontal 16:9 comedic impact keyframe. Gugugaga, still spinning like a round bowling ball, crashes into a wooden fish bucket on the Antarctic ice. The bucket flips into the air, small silver fish scatter in slow motion, snow puffs burst from the impact. Gugugaga's red scarf and blue hair clip remain visible, expression confused and dizzy. In the background, a tall leaning ice pillar is positioned as the next chain-reaction target. Pixar-like 3D animation, crisp readable chaos.
```

### 负向 Prompt

```text
different character, missing scarf, missing hair clip, gore, broken body, real fish photo, unreadable clutter, text, watermark
```

## KF04B Segment 04 结尾：冰柱倒向冰锣

### 输出目录

- `03_keyframes/episode_001/KF04B_ice_pillar_to_gong/`

### 使用资产

- `00_references/character/images/pose_sheets/ep001_gugugaga_pose_sheet_v002.png`

### 正向 Prompt

```text
Horizontal 16:9 chain-reaction keyframe. The wooden fish bucket and scattered fish hit a tall translucent ice pillar, making it tilt dramatically toward a row of large blue ice gongs in the distance. Gugugaga slides through the foreground in a dizzy spin trail, mostly motion but still recognizable with red scarf. The composition should clearly show cause and effect: bucket impact, leaning ice pillar, target ice gongs. Stylized Pixar-like 3D animation, icy blue comedy action.
```

### 负向 Prompt

```text
unclear action, too many props, city objects, metal gong, realistic photo, text labels, watermark, vertical composition
```

## KF05A Segment 05 起始：冰锣引发雪崩

### 输出目录

- `03_keyframes/episode_001/KF05A_gong_avalanche/`

### 使用资产

- `00_references/character/images/pose_sheets/ep001_gugugaga_pose_sheet_v002.png`

### 正向 Prompt

```text
Horizontal 16:9 wide action keyframe. A leaning ice pillar strikes a row of giant blue ice gongs, sending visible circular sound waves across the Antarctic valley. The sound waves shake a snowy mountain slope in the background, cracks forming in the snowpack. Gugugaga is small in the lower foreground, still sliding helplessly. Cinematic icy blue lighting, clear cause-and-effect composition, Pixar-like 3D animation, no text.
```

### 负向 Prompt

```text
metal concert gong, city environment, unclear sound waves, text, subtitles, logo, realistic disaster documentary, horror
```

## KF05B Segment 05 结尾：雪球冲向雪怪

### 输出目录

- `03_keyframes/episode_001/KF05B_snowball_to_monster/`

### 使用资产

- `00_references/character/images/selected/gugugaga_primary_reference.png`
- `00_references/character/images/pose_sheets/ep001_gugugaga_pose_sheet_v002.png`
- `00_references/monster/images/selected/snowstorm_monster_primary_reference.png`
- `00_references/monster/images/model_sheets/ep001_snowstorm_monster_model_sheet_v002_scale_corrected.png`

### 正向 Prompt

```text
Horizontal 16:9 dynamic keyframe. A giant rolling snowball races down the Antarctic ice toward the snowstorm monster. Gugugaga is trapped inside the snowball with only confused face, red scarf, and a hint of blue hair clip visible through the snow. The snowstorm monster is ahead, shocked and confused, correctly scaled: huge next to animals but smaller than mountains and large icebergs. The snowball is about 1.2-1.5 times the monster height, large enough to swallow it. Strong motion trail, snow spray, Pixar-like 3D action comedy.
```

### 负向 Prompt

```text
snowball too small, monster larger than mountains, kaiju scale, missing Gugugaga face, missing red scarf, redesigning monster, horror, text, watermark
```

## KF06A Segment 06 起始：雪球撞上雪怪

### 输出目录

- `03_keyframes/episode_001/KF06A_snowball_hits_monster/`

### 使用资产

- `00_references/character/images/pose_sheets/ep001_gugugaga_pose_sheet_v002.png`
- `00_references/monster/images/selected/snowstorm_monster_primary_reference.png`
- `00_references/monster/images/pose_sheets/ep001_snowstorm_monster_pose_sheet_v001.png`

### 正向 Prompt

```text
Horizontal 16:9 impact keyframe. The giant rolling snowball slams into the snowstorm monster, beginning to wrap around its soft snow-cloud body. Snow explodes outward in a bright white puff, partially hiding the impact. The monster's blue glowing eyes look surprised, its cloud side masses try to block the snowball but are being swallowed. Gugugaga's confused face and red scarf are barely visible in the snowball. Funny but epic Pixar-like 3D animation, strong white snow wipe energy.
```

### 负向 Prompt

```text
explosion fire, blood, monster destroyed violently, sharp teeth, hands, fists, snowball too small, mountain-sized monster, text, watermark
```

## KF06B Segment 06 结尾：南极最大雪人

### 输出目录

- `03_keyframes/episode_001/KF06B_final_snowman/`

### 使用资产

- `00_references/character/images/selected/gugugaga_primary_reference.png`
- `00_references/character/images/pose_sheets/ep001_gugugaga_pose_sheet_v002.png`
- `00_references/monster/images/pose_sheets/ep001_snowstorm_monster_pose_sheet_v001.png`

### 正向 Prompt

```text
Horizontal 16:9 joyful finale keyframe. The former snowstorm monster is now a harmless giant snowman version of itself, rounded and wrapped in snow, with a small silver fish comically stuck on its face. Its blue eyes look dazed and confused, no longer threatening. The sky clears with warm sunlight over the icy Antarctic field. Tiny penguins and seals cheer around it. Gugugaga stands in front, innocent and confused, red scarf bright, then preparing to slip again. Family-friendly Pixar-like 3D animation, warm victory tone.
```

### 负向 Prompt

```text
evil monster still attacking, horror, blood, realistic photo, snowman king, crown, beard, human face, missing Gugugaga, missing red scarf, text, logo, watermark
```

## 生成建议

- 先生成第一幕三张：`KF01A`、`KF01B`、`KF01C`，确认“平静南极 -> 雪怪诞生 -> 雪怪攻击”的节奏、尺度和冰山比例都成立。
- 再生成 `KF02A`、`KF03B`、`KF05B`、`KF06B`，验证主角一致性、滑倒笑点、雪球机制和结尾反转。
- 最后补齐剩余关键帧。
- 每张图都使用 16:9 横屏，不要生成竖屏构图。
- 如果工具支持负向 prompt，请把对应“负向 Prompt”粘贴到负向输入框。
- 如果工具不支持负向 prompt，请在正向末尾追加：`Avoid: ...`，不要把负向词直接混成想要生成的元素。
