# Episode 001 Keyframe Prompts v003 - Progressive Monster Birth

## 用途

用于重做第一段雪怪出场关键帧。  
本版按“背景母版 + 递进改图”的工作流，把雪怪出场从结果图改成渐进式元素生成镜头：平静 -> 异变 -> 聚合 -> 半成型 -> 完整现身 -> 首次攻击。

## 方法论

不要每张关键帧都从零生成。先确定一张 16:9 背景母版，然后基于同一张母版连续改图。每一张都必须保留：

- same camera angle
- same horizon line
- same foreground ice field composition
- same central blue iceberg group
- same far mountain silhouettes
- same approximate fish bucket and animal staging

只允许变化：

- sky brightness and storm direction
- wind and snow amount
- floating ice crystal amount
- animal emotion and movement
- snowstorm monster formation stage
- attack VFX

## 推荐输出目录

- Shot A 平静母版：`03_keyframes/episode_001/KF01A_master_calm_antarctica/`
- Shot B 异变开始：`03_keyframes/episode_001/KF01B_crisis_start/`
- Shot C 雪怪聚合生成中：`03_keyframes/episode_001/KF01C_monster_forming/`
- Shot D 雪怪半成型抬升：`03_keyframes/episode_001/KF01D_monster_half_formed/`
- Shot E 完整现身 + 攻击准备：`03_keyframes/episode_001/KF01E_monster_reveal_attack_ready/`
- Shot F 首次攻击：`03_keyframes/episode_001/KF01F_monster_first_attack/`

## 推荐上传资产

- 背景母版：生成 Shot A 后，后续 Shot B-F 都上传 Shot A 作为主场景参考。
- 雪怪主参考：`00_references/monster/images/selected/snowstorm_monster_primary_reference.png`
- 雪怪比例参考：`00_references/monster/images/model_sheets/ep001_snowstorm_monster_model_sheet_v002_scale_corrected.png`

不要上传多格动作 sheet 作为核心动作控制。若必须上传 `00_references/monster/images/pose_sheets/ep001_snowstorm_monster_pose_sheet_v001.png`，只把它当作外观/局部姿态参考，不要让模型模仿分屏布局。

## 当前帧选择判断

- Shot A 母版已选用：`03_keyframes/episode_001/KF01A_master_calm_antarctica/ep001_KF01A_selected.png`。
- Shot B 异变开始已选用：`03_keyframes/episode_001/KF01B_crisis_start/ep001_KF01B_from_selected_A_candidate_v001.png`。
- Shot C 雪怪身体雏形已选用：`03_keyframes/episode_001/KF01C_monster_forming/ep001_KF01C_selected.png`。
- Shot C 最新候选源文件：`03_keyframes/episode_001/KF01C_monster_forming/ep001_KF01C_animals_facing_storm_candidate_v002.png`。
- Shot D 蓝眼点亮、身体汇聚候选：`03_keyframes/episode_001/KF01D_monster_half_formed/ep001_KF01D_eyes_lit_body_forming_candidate_v001.png`。
- Shot E 完整成型、动物逃跑候选：`03_keyframes/episode_001/KF01E_monster_reveal_attack_ready/ep001_KF01E_full_body_animals_flee_candidate_v001.png`。
- Shot F 首次横扫攻击候选：`03_keyframes/episode_001/KF01F_monster_first_attack/ep001_KF01F_sweeping_ice_ray_candidate_v001.png`。
- 正面视角参考已保存：`03_keyframes/episode_001/KF01E_monster_reveal_attack_ready/ep001_KF01E_front_camera_reference_v001.png`。
- 当前 Shot A 和 Shot B 的内容节奏是对的，但机位偏侧向、右侧大冰山更抢画面。如果决定采用正面压迫感路线，应按正面视角参考重建 Shot A 和 Shot B，让中央冰山 / 中央远景成为雪怪后续聚合的位置。
- 当前先采用 Shot A/B/C 同一构图体系继续推进。Shot D 才进入蓝眼睛点亮和更清楚的头部可读阶段。

## 正面视角重建建议

第三张正面参考的优点是镜头更像舞台正面，雪怪后续可以从中央冰山和天空云团后方压下来，视觉焦点更集中。建议采用，但必须重建整组 Segment 01 关键帧，不能把旧侧向 Shot A/B 和新正面 Shot C/E 混用。

正面版 Shot A/B 要保留这些连续锚点：

- central mid-sized iceberg group as the future monster birth area
- open water / glossy ice leading lines toward the center
- fish bucket and ordinary animals in the foreground as scale anchors
- left-side sky area reserved for incoming dark storm
- far mountains kept smaller than the monster birth area, not replaced each time

正面版 Shot A/B 避免：

- right-side giant iceberg dominating the whole composition
- camera angle changing between A and B
- animals and fish bucket jumping to unrelated positions
- storm core already becoming a full monster in Shot B

### 正面版 Shot A 重建 Prompt（一键复制）

```text
Recreate the peaceful Antarctic master plate with a more frontal cinematic camera angle, using the uploaded calm Antarctica image as content reference and the uploaded front-camera monster reveal image only as camera/framing reference. Horizontal 16:9 wide shot. Keep the scene peaceful with no monster and no storm. Compose the environment like a frontal stage: a recognizable central mid-sized blue iceberg group in the middle distance where the snowstorm will later gather, glossy open ice and water leading toward the center, far snow mountains on the horizon, ordinary penguins and seals in the foreground, and a wooden fish bucket near the foreground as a scale anchor. Pale blue sky, soft sunlight, calm animals, clean Pixar-like 3D animated style, icy blue palette, stable horizon line, readable symmetrical composition. This image will be the new master plate for the entire monster birth sequence.

Avoid: snowstorm monster, dark storm, panic, blizzard, attack, shattered ice, huge right-side iceberg dominating the frame, changed aspect ratio, vertical image, text, logo, watermark, subtitles, horror, realistic disaster.
```

### 正面版 Shot B 重建 Prompt（一键复制）

```text
Edit the new frontal Antarctic master plate into the beginning of the crisis while preserving the exact same frontal camera angle, horizon line, central iceberg group, far mountain silhouettes, foreground ice field, animal positions, and wooden fish bucket position. Horizontal 16:9 cinematic wide shot. The peaceful sky begins to darken from the upper left side, wind rises, thin snow mist curls low across the ice, loose ice crystals drift upward, and ordinary penguins and seals look up nervously. Behind and above the central mid-sized iceberg group, a subtle stormy snow-cloud core begins forming, but it is still only weather and atmosphere, not a readable creature. No glowing eyes yet, no mouth yet, no body yet. Family-friendly Pixar-like 3D animation, cinematic suspense, same scene continuity.

Avoid: full monster visible, glowing eyes already visible, mouth already visible, body silhouette, attack, shattered iceberg, changed camera angle, changed horizon line, changed iceberg layout, changed foreground animals, changed fish bucket position, huge right-side iceberg dominating the frame, mountain-sized monster, horror, text, logo, watermark, subtitles, vertical image, wrong aspect ratio.
```

## Shot A - 背景母版 / 平静南极建立镜头

### 输出目录

- `03_keyframes/episode_001/KF01A_master_calm_antarctica/`

### 一键复制 Prompt（正向内容 + Avoid 负向约束）

```text
Horizontal 16:9 cinematic wide shot, peaceful Antarctica before the crisis. Keep this image as the background master plate for later continuity. A glossy frozen ice field in the foreground with subtle ice texture and reflective patches, a clear stable horizon line, a recognizable group of mid-sized blue icebergs in the middle distance, and larger far snow mountains in the background. Pale blue sky, soft sunlight, calm atmosphere, no storm yet. Tiny penguins and seals are peacefully resting on the ice, and a wooden fish bucket sits quietly nearby. Clean readable composition, family-friendly Pixar-like 3D animation, soft icy blue palette, simple but beautiful staging, highly consistent environment layout, no monster yet.

Important continuity requirement: This shot must feel like the fixed master environment for a sequence. The foreground ice field, the central iceberg group, the large iceberg silhouettes, and the far mountain shapes should all be clear and memorable so later shots can preserve the same layout.

Avoid: snowstorm monster, dark storm already present, panic, shattered ice, attack, blizzard blast, mountain-sized monster, kaiju scale, realistic disaster, horror, blood, text, logo, watermark, subtitles, vertical image, wrong aspect ratio.
```

## Shot B - 异变开始 / 背景连续版

### 输出目录

- `03_keyframes/episode_001/KF01B_crisis_start/`

### 一键复制 Prompt（正向内容 + Avoid 负向约束）

```text
Edit the same Antarctic master environment into the beginning of the crisis while preserving the exact same camera angle, horizon line, iceberg layout, far mountain silhouettes, and foreground ice field composition. Horizontal 16:9 cinematic wide shot. The peaceful Antarctic scene begins to change: the pale blue sky darkens from one side, wind picks up, thin snow mist starts curling low across the ice, and loose ice crystals begin to drift in the air. Tiny penguins and seals look upward in confusion and unease, but panic has only just begun. The wooden fish bucket is still nearby on the ice. No full monster yet. In the far middle distance behind the mid-sized blue icebergs, a stormy snow-cloud core is beginning to form, subtle and ominous, but not yet readable as a full creature. Family-friendly Pixar-like 3D animation, cinematic suspense, clear continuity with the previous shot.

Important: Preserve the same environment and layout as the master plate. This is a progression shot, not a new scene.

Avoid: full monster already visible, attack already happening, shattered iceberg, huge scale jump, mountain-sized creature, monster larger than big icebergs, monster larger than far mountains, changed camera angle, changed horizon line, changed iceberg layout, changed far mountain silhouettes, changed foreground ice field, realistic tornado, horror, text, logo, watermark, subtitles, vertical image, wrong aspect ratio.
```

## Shot C - 雪怪聚合生成中 / 惊艳出场核心镜头

### 输出目录

- `03_keyframes/episode_001/KF01C_monster_forming/`

### 一键复制 Prompt（正向内容 + Avoid 负向约束）

```text
Edit the same Antarctic master environment again, preserving the same camera angle, horizon line, iceberg layout, far mountain silhouettes, and foreground ice field composition. Horizontal 16:9 cinematic wide shot. This is the dramatic early formation moment of the snowstorm monster, but the creature is still unfinished and not attacking. Behind the mid-sized blue icebergs, a rough giant body prototype begins to form from dark storm clouds, snow mist, icy vapor, and floating crystal shards. The center of the unfinished belly contains a bright rotating storm-cloud vortex that pulls in ice crystals, snow, mist, and dark clouds. Above the belly vortex, a heavy dark cloud mass gathers where the head will later form, creating contrast for the next frame when blue eyes will light up, but there are no visible eyes yet. The body shape is only a cloudy prototype, with no complete face, no mouth, no full arms, no hands, no fingers, no legs, and no attack. Tiny penguins and seals in the foreground have turned around or raised their heads toward the storm position, watching the formation in fear and awe. The wooden fish bucket remains as a foreground scale anchor. Keep the ice field and water clean, readable, and low-noise, without dense tiny particles or dirty texture. Family-friendly Pixar-like 3D animation, magical elemental creature birth effect, highly cinematic, awe-inspiring but not horror.

Important: This must feel like a spectacular elemental formation effect, not a simple monster already standing there shot. The background must remain continuous with earlier shots.

Avoid: blue glowing eyes, visible eyes, mouth, full face, full head, fully complete monster already standing cleanly, complete snowman body, complete round body, readable arms, fists, hands, fingers, legs, feet, attack already firing, shattered iceberg already, mountain-sized monster, monster larger than large icebergs, monster larger than far mountains, changed camera angle, changed horizon line, changed iceberg layout, changed far mountain silhouettes, animals facing away from the storm, dirty noisy ground texture, dense tiny particles on the ice or water, muscular anatomy, crown, beard, sharp teeth, realistic tornado, horror, text, logo, watermark, subtitles, vertical image, wrong aspect ratio.
```

## Shot D - 雪怪半成型抬升 / 出场完成前一步

### 输出目录

- `03_keyframes/episode_001/KF01D_monster_half_formed/`

### 一键复制 Prompt（正向内容 + Avoid 负向约束）

```text
Edit the same Antarctic master environment again, preserving the same camera angle, horizon line, iceberg layout, far mountain silhouettes, and foreground ice field composition. Horizontal 16:9 cinematic wide shot. The snowstorm monster is now rising higher behind the mid-sized icebergs and has become mostly readable. Its huge upper body is formed from thick dark storm cloud, rolling snow mist, and embedded glowing ice crystals. Two bright blue glowing eyes stare out clearly, and the wide dark cloud-hole mouth is visible. The broad heavy upper body and bulky side cloud masses are now established, but the lower body still blends into a rotating snowstorm base and drifting wind-blown mist, making it feel born out of the blizzard itself. Snow particles and icy fragments swirl around the creature. Tiny penguins and seals now run in panic below, and the wooden fish bucket begins sliding across the ice. The monster is huge compared with the visible animals and fish bucket but still clearly smaller than the large background icebergs and far snow mountains. Family-friendly Pixar-like 3D animation, dramatic reveal, readable silhouette, cinematic suspense.

Avoid: attack blast already firing, shattered iceberg already, mountain-sized monster, monster larger than large icebergs, monster larger than far mountains, changed camera angle, changed horizon line, changed iceberg layout, changed far mountain silhouettes, ice titan, muscular arms, fists, hands, fingers, legs, feet, crown, beard, horror, text, logo, watermark, subtitles, vertical image, wrong aspect ratio.
```

## Shot E - 完整现身 + 首次攻击准备

### 输出目录

- `03_keyframes/episode_001/KF01E_monster_reveal_attack_ready/`

### 一键复制 Prompt（正向内容 + Avoid 负向约束）

```text
Edit the same Antarctic master environment again, preserving the same camera angle, horizon line, iceberg layout, far mountain silhouettes, and foreground ice field composition. Horizontal 16:9 cinematic wide shot. The snowstorm monster has now fully emerged onto the Antarctic ice field. It stands in full readable form with a broad heavy snow-cloud body, two bright blue glowing eyes, a wide dark cloud-hole mouth opening in a roar, swirling snow mist inside and around its body, and sharp blue icy crystal accents embedded across the upper mass. The lower body still dissolves into a wide snow-mist base rather than legs and feet. Tiny penguins and seals flee below, and the wooden fish bucket slides quickly across the ice. The monster remains huge compared with the visible animals and fish bucket, but clearly smaller than the large background icebergs and far snow mountains. This is the end of the entrance and the start of the attack beat. Family-friendly Pixar-like 3D animation, spectacular reveal, dangerous but comedic tone.

Avoid: monster larger than large icebergs, monster larger than far mountains, mountain-sized monster, kaiju scale, changed camera angle, changed horizon line, changed iceberg layout, changed far mountain silhouettes, muscular arms, fists, hands, fingers, legs, feet, crown, beard, sharp teeth, horror, realistic tornado, text, logo, watermark, subtitles, vertical image, wrong aspect ratio.
```

## Shot F - 首次攻击关键帧 / 连续背景版

### 输出目录

- `03_keyframes/episode_001/KF01F_monster_first_attack/`

### 一键复制 Prompt（正向内容 + Avoid 负向约束）

```text
Edit the same Antarctic master environment again, preserving the same camera angle, horizon line, iceberg layout, far mountain silhouettes, and foreground ice field composition. Horizontal 16:9 cinematic wide shot. The snowstorm monster performs its first attack. From its wide dark cloud-hole mouth and swirling storm body, a concentrated blue-white blizzard blast shoots sideways across the frame and strikes a smaller nearby iceberg, shattering it into sparkling ice chunks and snow dust. Tiny penguins and seals flee below, the wooden fish bucket slides across the ice, and fragments of ice and snow swirl through the air. The snowstorm monster keeps the same scale as the previous reveal shot: huge compared with the visible animals and fish bucket, but clearly smaller than the large background icebergs and far snow mountains. Pixar-like family-friendly animated comedy tone, strong readable action, clear cause and effect, dramatic but not horror.

Avoid: background changing to a completely different scene, monster growing to mountain scale, monster larger than large icebergs, monster larger than far mountains, changed camera angle, changed horizon line, changed iceberg layout, changed far mountain silhouettes, muscular anatomy, fists, hands, fingers, legs, feet, crown, beard, sharp teeth, realistic disaster wall, horror, text, logo, watermark, subtitles, vertical image, wrong aspect ratio.
```

## 视频段落建议

- 0-2s：Shot A，平静南极建立镜头。
- 2-4s：Shot B，天空一侧变暗，地面风雪卷起，小动物抬头。
- 4-6s：Shot C，远处冰山后身体雏形聚合，肚子中心暴风云团吸引冰晶和乌云，动物转身看向风暴。
- 6-8s：Shot D/E，蓝眼睛点亮，雪怪半成型到完整现身，张口准备攻击。
- 8-10s：Shot F，首次暴风雪攻击击碎小冰山。

## 使用提醒

每个 Shot 的 prompt 都已经是完整可复制文本块，末尾自带 `Avoid:` 负向约束。生成时直接复制对应 Shot 的整段文本即可。
