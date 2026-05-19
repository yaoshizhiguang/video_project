# Episode 001 Keyframe Prompts v002 - Continuity Rebuild

## 用途

用于重做第一段 `KF01A/KF01B/KF01C`。  
v001 的三张图画面质量各自可用，但背景、天空、冰山位置、镜头角度不统一，导致视频生成时在关键节点生硬切换。v002 的目标不是让每张图单独好看，而是让三张图像同一镜头里的不同时间点。

## 核心策略

- 先把 `KF01A` 当作母场景板：冰山布局、远山轮廓、水面位置、鱼桶位置、动物大致区域都固定。
- `KF01B` 和 `KF01C` 必须基于 `KF01A` 做 image-to-image / variation，不要从纯文本重新生成。
- 只允许天气、云团、雪雾、雪怪形成、攻击特效发生变化；不要改机位、不要换背景、不要重排冰山。
- 当前多格动作 sheet 不作为关键动作输入；动作改用文字描述锁定。

## 共同上传资产

- 起始母场景：`03_keyframes/episode_001/KF01A_calm_antarctica/ep001_KF01A_candidate_v001.png`
- 雪怪主参考：`00_references/monster/images/selected/snowstorm_monster_primary_reference.png`
- 雪怪比例参考：`00_references/monster/images/model_sheets/ep001_snowstorm_monster_model_sheet_v002_scale_corrected.png`

可选参考：

- `00_references/monster/images/pose_sheets/ep001_snowstorm_monster_pose_sheet_v001.png`

如果使用可选动作图，请明确告诉工具：它只用于雪怪外观和局部姿态参考，不是分屏布局，不是剧情关键帧。

## 全局正向 Prompt

```text
Create horizontal 16:9 cinematic keyframes for the same continuous Antarctic shot in a cute Pixar-like 3D animated comedy short film. Use the uploaded calm Antarctic image as the master background plate. Preserve the same camera angle, horizon line, ice field, water edge, main blue icebergs, distant snow mountains, fish bucket position, and animal staging across all three keyframes.

Only the weather, snow particles, storm clouds, monster formation, and attack effects should evolve over time. Do not redesign the location between keyframes. Keep the snowstorm monster consistent with the uploaded primary reference: dark storm-cloud body, glowing blue eyes, cloud-hole mouth, ice crystal accents, wide snow-mist base, powerful but clumsy silhouette. Use the scale-corrected model sheet for scale: huge compared with penguins and seals, clearly smaller than large icebergs and far snow mountains.

Family-friendly Pixar-like 3D animation, icy blue Antarctic palette, cinematic lighting, soft snow particles, clean readable silhouettes, no text, no watermark.
```

## 全局负向 Prompt

```text
different background, different iceberg layout, different mountain layout, different camera angle, hard continuity break, new location, unrelated composition, split screen, collage, storyboard panels, pose sheet layout, monster larger than large icebergs, monster larger than far snow mountains, mountain-sized monster, kaiju scale, pure tornado, realistic disaster footage, live action, horror, blood, gore, text, logo, watermark, subtitles, vertical image, wrong aspect ratio
```

## KF01A v002 起始母场景：平静南极

### 输出目录

- `03_keyframes/episode_001/KF01A_calm_antarctica/`

### 正向 Prompt

```text
Horizontal 16:9 cinematic wide shot, calm Antarctica before the crisis. This is the master background plate for the whole first video segment. Pale blue sky, soft sunlight, glossy quiet ice field, reflective water edge, distant snow mountains, large blue icebergs with clear readable shapes, tiny penguins and seals relaxing, and a wooden fish bucket sitting still on the ice. Leave enough sky and mid-ground space behind the main icebergs for storm clouds and the monster to form later. No storm yet, no monster yet, no panic yet. Clean family-friendly Pixar-like 3D animation.
```

### 负向 Prompt

```text
snowstorm monster visible, dark storm already present, panic already happening, shattered iceberg, attack effects, different camera angle, vertical image, text, logo, watermark
```

## KF01B v002 中段：风暴云团聚集并形成雪怪

### 输出目录

- `03_keyframes/episode_001/KF01B_monster_birth/`

### 正向 Prompt

```text
Horizontal 16:9 keyframe based on the uploaded KF01A master background plate. Keep the same camera angle, same main icebergs, same distant mountains, same ice field, same water edge, same fish bucket position, and same animal areas.

The calm scene is transforming into a supernatural storm birth moment. Dark clouds gather from the upper left of the same sky, snow mist crawls across the same ice, and multiple swirling streams of wind, snow, and cloud converge behind the mid-ground blue icebergs. The snowstorm monster is not simply rising from behind an iceberg; it is being formed by the storm. Show storm clouds compressing into the monster's rounded dark cloud body, blue glowing eyes appearing inside the cloud, a cloud-hole mouth opening, ice crystals orbiting around the forming body, and a wide snow-mist base touching the ice. Penguins and seals are just starting to notice the danger.

Use the monster primary reference for design consistency and the scale-corrected model sheet for size. The monster is huge compared with animals but clearly smaller than the large blue icebergs and far snow mountains. Suspenseful but still cute Pixar-like 3D animation.
```

### 负向 Prompt

```text
simple monster rising from behind iceberg only, fully attacking already, shattered iceberg already, different background, changed iceberg positions, changed mountain positions, new camera angle, Gugugaga visible, monster larger than icebergs, monster larger than mountains, mountain-sized monster, pure tornado, human giant, hands, fingers, legs, feet, crown, beard, sharp teeth, horror, text, watermark
```

## KF01C v002 结尾：同一场景内第一次攻击

### 输出目录

- `03_keyframes/episode_001/KF01C_monster_first_attack/`

### 正向 Prompt

```text
Horizontal 16:9 keyframe based on the uploaded KF01A master background plate and the KF01B storm formation direction. Keep the same camera angle, same main icebergs, same distant mountains, same ice field, same water edge, same fish bucket position, and same animal areas. Do not change the location.

The snowstorm monster has now fully formed from the storm clouds in the same mid-ground area. It leans forward and releases its first attack: a concentrated blue-white blizzard blast from its dark cloud-hole mouth. The blast crosses the same frame and shatters a small nearby iceberg into sparkling ice chunks. Snow dust, ice fragments, and blue-white wind trails fill the air, but the background layout remains recognizable. Tiny penguins and seals flee across the same ice field, and the wooden fish bucket skids away.

Show clear cause and effect: storm-formed monster -> blizzard breath -> small iceberg shatters -> animals panic. Keep the monster scale controlled by the scale-corrected model sheet: huge compared with small animals, clearly smaller than large icebergs and distant snow mountains. Family-friendly Pixar-like animated comedy, dramatic but not horror.
```

### 负向 Prompt

```text
different location, changed iceberg layout, changed mountains, hard cut feeling, monster being born only with no attack, no blizzard blast, no shattered small iceberg, monster larger than large icebergs, monster larger than far snow mountains, kaiju scale, pure tornado, human giant, muscular arms, hands, fingers, legs, feet, crown, beard, sharp teeth, horror, gore, blood, text, logo, watermark
```

## 生成顺序

- 第一步：如果当前 `KF01A_candidate_v001` 满意，就把它作为母场景，不再重做。
- 第二步：用 `KF01A_candidate_v001` 图生图生成 `KF01B_candidate_v002`，强制保持背景布局。
- 第三步：继续用 `KF01A_candidate_v001` + `KF01B_candidate_v002` 作为参考生成 `KF01C_candidate_v002`。
- 第四步：视频生成时优先使用 `KF01A_candidate_v001` 单起始帧 + `ep001_segment01_one_shot_video_prompt_v002.md`，不要把背景不一致的 v001 三关键帧一起喂给视频模型。
