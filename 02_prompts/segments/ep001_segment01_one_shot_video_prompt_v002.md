# Episode 001 Segment 01 One-Shot Video Prompt v002

## 用途

用于重新生成第一段视频：平静南极 -> 风暴聚集 -> 雪怪由云团冰雪形成 -> 第一次攻击。  
本版修正 v001 的核心问题：不要把三张背景不一致的关键帧都当作严格锚点，否则视频会在节点处硬切；改为使用一个连续母场景和一条时间轴完成一镜到底。

## 推荐上传资产

- 必传起始场景：`03_keyframes/episode_001/KF01A_calm_antarctica/ep001_KF01A_candidate_v001.png`
- 必传雪怪主参考：`00_references/monster/images/selected/snowstorm_monster_primary_reference.png`
- 必传雪怪比例参考：`00_references/monster/images/model_sheets/ep001_snowstorm_monster_model_sheet_v002_scale_corrected.png`
- 可选雪怪设定参考：`00_references/monster/images/pose_sheets/ep001_snowstorm_monster_pose_sheet_v001.png`

不要把 `KF01B` 和 `KF01C` 作为严格中间 / 结束关键帧上传给本轮视频生成；它们当前的天空、冰山布局、镜头位置差异太大，会诱发硬切。可仅把它们当作“效果方向参考”人工看，不作为模型必须匹配的视觉锚点。

## 动作图使用判断

当前多格动作 sheet 对图生视频帮助有限，尤其是 `ep001_snowstorm_monster_pose_sheet_v001.png` 这种很多动作拼在一张里的图，模型容易忽略具体动作，或者把它理解成分屏 / 拼贴。  
本轮建议不依赖动作图驱动视频动作，而是用文字时间轴明确动作。动作图只作为雪怪外观参考的补充，不作为关键动作锚点。

## 正向 Prompt

```text
Create a horizontal 16:9 cinematic 3D animated one-shot video, about 10 seconds long, based on the uploaded calm Antarctic starting image as the single continuous scene anchor.

Important continuity rule: keep the same camera direction, same horizon line, same ice field, same water edge, same main blue icebergs, same distant snow mountains, and same wooden fish bucket position throughout the whole video. Do not cut to a different background. Do not jump to a new composition. The whole scene must feel like one continuous camera take where the weather and monster effects gradually develop inside the same Antarctic location.

Use the uploaded snowstorm monster primary reference only to lock the monster design: dark storm-cloud body, blue glowing eyes, cloud-hole mouth, ice crystal accents, wide snow-mist base, powerful but clumsy silhouette. Use the scale-corrected monster model sheet to lock scale: the monster is huge compared with penguins and seals, but clearly smaller than the large blue icebergs and far snow mountains.

Timeline:
Seconds 0-2: Start exactly from the calm Antarctic scene. Pale blue sky, glossy quiet ice, distant snow mountains, large blue icebergs, tiny penguins and seals resting, a wooden fish bucket sitting still. Camera begins as a wide peaceful establishing shot with very slow forward drift.

Seconds 2-4: The weather changes without cutting. Dark clouds roll in from the upper left of the same sky. Fine snow begins to blow across the same ice field. The water reflection becomes darker. The animals slowly notice the wind. Low snow mist crawls around the base of the same mid-ground icebergs.

Seconds 4-7: The monster birth must be a special effects formation, not a simple rise from behind an iceberg. Above and behind the mid-ground icebergs, multiple storm-cloud streams spiral inward, snow dust rises from the ice, blue-white ice crystals orbit the forming cloud mass, and a dark blizzard cloud gradually compresses into the snowstorm monster's body. First show only glowing blue eyes inside the swirling cloud, then the cloud-hole mouth opens, then the wide snow-mist base and soft cloud arms take shape. The monster is forming from storm clouds, wind, snow, and ice particles in the same location.

Seconds 7-10: The newly formed monster releases its first attack. Without changing background or cutting, it leans forward and exhales a concentrated blue-white blizzard blast from the cloud-hole mouth. The blast travels across the same frame and shatters a small nearby iceberg into sparkling ice chunks. Tiny penguins and seals panic and slide away; the fish bucket skids across the glossy ice. Show clear cause and effect: monster forms -> monster breathes/blasts -> small iceberg shatters -> animals flee.

Camera: one continuous cinematic push-in with a slight arc, then subtle shake during the blast. No hard cuts, no shot-reverse-shot, no scene replacement. Keep motion smooth and readable, with a family-friendly Pixar-like 3D animated comedy tone. Icy blue Antarctic palette, soft snow particles, cinematic lighting, high quality stylized 3D animation. No text, no subtitles, no watermark.
```

## 负向 Prompt

```text
hard cut, jump cut, scene change, different background, changing iceberg layout, changing mountain layout, changing camera angle abruptly, teleporting characters, using multiple unrelated keyframes, split screen, collage, storyboard panel, pose sheet layout, frozen still image slideshow, Gugugaga visible, main character visible, red scarf, blue hair clip, monster larger than large icebergs, monster larger than far snow mountains, mountain-sized monster, kaiju scale, simple monster rising from behind iceberg only, no storm formation, no cloud formation, pure tornado, realistic disaster footage, live action, photorealistic horror, human giant, muscular arms, hands, fingers, legs, feet, crown, beard, old man face, snowman king, sharp teeth, demon, dragon, robot, gore, blood, excessive camera shake, vertical video, wrong aspect ratio, text, logo, watermark, subtitles
```

## 如果工具没有负向 Prompt 输入框

在正向 prompt 末尾追加：

```text
Avoid: hard cut, jump cut, scene change, different background, changing iceberg layout, changing mountain layout, split screen, collage, pose sheet layout, Gugugaga visible, monster larger than large icebergs or far snow mountains, simple monster rising from behind iceberg only, text, logo, watermark.
```

## 生成建议

- 第一轮只上传 `KF01A`、雪怪主参考、比例参考，先测试“一镜到底”和风暴形成是否成立。
- 如果工具必须上传首尾帧，先重新生成与 `KF01A` 同构图的 `KF01C_v002`，不要使用当前 `KF01C_candidate_v001` 作为结束帧。
- 如果动作仍不够准，优先改文字时间轴，不要继续堆多格动作 sheet。
