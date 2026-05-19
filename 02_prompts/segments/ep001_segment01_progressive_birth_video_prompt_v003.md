# Episode 001 Segment 01 Progressive Birth Video Prompt v003

## 用途

用于把第一段视频改成“背景母版 + 渐进式雪怪生成”的 10 秒连续镜头。  
本版替代 v001 的三关键帧硬切思路，也比 v002 更细：把雪怪出场拆成平静、异变、聚合、半成型、完整现身、首次攻击六个连续状态。

## 推荐上传

优先上传：

- Shot A 背景母版：`03_keyframes/episode_001/KF01A_master_calm_antarctica/`
- Shot B 异变开始：`03_keyframes/episode_001/KF01B_crisis_start/`
- Shot C 雪怪聚合：`03_keyframes/episode_001/KF01C_monster_forming/`
- Shot D 半成型：`03_keyframes/episode_001/KF01D_monster_half_formed/`
- Shot E 完整现身：`03_keyframes/episode_001/KF01E_monster_reveal_attack_ready/`
- Shot F 首次攻击：`03_keyframes/episode_001/KF01F_monster_first_attack/`

参考资产：

- 雪怪主参考：`00_references/monster/images/selected/snowstorm_monster_primary_reference.png`
- 雪怪比例参考：`00_references/monster/images/model_sheets/ep001_snowstorm_monster_model_sheet_v002_scale_corrected.png`
- 可选构图参考：`03_keyframes/episode_001/KF01E_monster_reveal_attack_ready/ep001_KF01E_front_camera_reference_v001.png` 只用于参考正面压迫感和构图，不代表怪物应该在 2-6 秒提前完整成型。

如果视频工具上传关键帧数量有限，优先使用 Shot A、Shot C、Shot E、Shot F。  
如果只能上传首尾帧，优先使用 Shot A 和 Shot E/F，并把完整时间轴写入 prompt。

## 一键复制 Prompt（正向内容 + Avoid 负向约束）

说明：下面是一整段可直接复制到生成工具的 prompt。`Avoid:` 之后是负向约束，不要删掉。

```text
Create a horizontal 16:9 cinematic 3D animated video, about 10 seconds long, as one continuous shot in the same Antarctic environment. Use the uploaded keyframes as progressive states of the same scene, not as separate locations. Preserve the same camera angle, horizon line, foreground ice field composition, central blue iceberg group, far mountain silhouettes, animal staging, and wooden fish bucket position throughout the video.

0-2s: peaceful Antarctica. Pale blue sky, glossy ice field, calm animals, wooden fish bucket, mid-sized blue icebergs, distant snow mountains.

2-4s: crisis begins in the same scene. One side of the sky darkens, wind rises, thin snow mist curls low across the ice, loose ice crystals begin drifting upward, animals look up nervously. No full monster yet, only a subtle stormy snow-cloud core behind the mid-sized icebergs.

4-6s: elemental monster formation. Behind the same icebergs, violent storm snow clouds, ground snow mist, cold wind streams, and floating blue ice crystals gather into a living storm core. Two bright cold blue glowing eyes appear first inside the snow cloud; they are the first clear sign that the storm is alive. A faint dark cloud-hole mouth shadow only barely begins to appear beneath the eyes. The creature has no complete head yet, no complete round body yet, no solid arms yet, and no fully readable silhouette. Thick snow-cloud body masses are still forming out of rotating blizzard matter. The monster is not complete yet.

6-8s: half-formed reveal. The snowstorm monster rises higher and becomes mostly readable. Its upper body forms from thick dark storm cloud, rolling snow mist, and embedded glowing ice crystals. The broad upper body and bulky side cloud masses are established, but the lower body still blends into a rotating snowstorm base. Animals begin fleeing, the fish bucket starts sliding.

8-10s: complete reveal and first attack. The snowstorm monster fully emerges, opens its dark cloud-hole mouth, and releases a concentrated blue-white blizzard blast sideways across the frame. The blast strikes a smaller nearby iceberg and shatters it into sparkling ice chunks and snow dust. Keep scale controlled: the monster is huge compared with the visible penguins, seals, and wooden fish bucket, but clearly smaller than the large blue icebergs and far snow mountains. Do not introduce the later hero character in this segment; this segment only contains ordinary Antarctic animals, the fish bucket, the environment, and the snowstorm monster.

The whole video must feel like: peaceful scene -> crisis begins -> storm gathers -> monster forms -> first attack. Smooth continuous camera push-in, no hard cuts, no scene replacement. Family-friendly Pixar-like 3D animation, icy blue palette, cinematic lighting, spectacular elemental VFX, dramatic but not horror, no text, no subtitles, no watermark.

Avoid: later hero character visible, red scarf, blue hair clip, special main character penguin, hard cut, jump cut, scene change, different background, changed camera angle, changed horizon line, changed iceberg layout, changed far mountain silhouettes, changed foreground ice field, full monster visible too early, complete snowman body before 6 seconds, complete round body before 6 seconds, readable arms before 6 seconds, full open mouth too early, monster already standing from the start, simple monster rising from behind iceberg only, attack too early, no formation process, split screen, collage, pose sheet layout, monster larger than large icebergs, monster larger than far mountains, mountain-sized monster, kaiju scale, muscular anatomy, fists, hands, fingers, legs, feet, crown, beard, sharp teeth, realistic tornado, realistic disaster footage, horror, blood, gore, vertical video, wrong aspect ratio, text, logo, watermark, subtitles.
```
