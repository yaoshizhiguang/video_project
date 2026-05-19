# Episode 001 Segment 01 Video Prompt v001

## 用途

用于把前三张关键帧合成为第一段 10 秒左右横屏视频：平静南极 -> 雪怪诞生 -> 雪怪第一次攻击。

## 参考图片

按顺序上传或作为首尾/中间关键帧使用：

- 起始关键帧：`03_keyframes/episode_001/KF01A_calm_antarctica/ep001_KF01A_candidate_v001.png`
- 中间关键帧：`03_keyframes/episode_001/KF01B_monster_birth/ep001_KF01B_candidate_v001.png`
- 结束关键帧：`03_keyframes/episode_001/KF01C_monster_first_attack/ep001_KF01C_candidate_v001.png`

辅助参考图：

- 雪怪主参考：`00_references/monster/images/selected/snowstorm_monster_primary_reference.png`，用于锁定雪怪的核心外观设计，不要重设计。
- 雪怪比例校准图：`00_references/monster/images/model_sheets/ep001_snowstorm_monster_model_sheet_v002_scale_corrected.png`，用于锁定雪怪与冰山、雪山、小动物之间的尺度关系。
- 雪怪动作图：`00_references/monster/images/pose_sheets/ep001_snowstorm_monster_pose_sheet_v001.png`，用于参考雪怪诞生、咆哮、释放暴风雪攻击时的姿态和动态，不作为剧情关键帧。

不要上传咕咕嘎嘎参考图；第一段中咕咕嘎嘎还没有出场。

## 正向 Prompt

```text
Create a horizontal 16:9 cinematic 3D animated video, about 10 seconds long, using the three uploaded keyframes as strict visual anchors in order.

Image 1 is the starting keyframe: calm Antarctica before the crisis, used for seconds 0-2.
Image 2 is the middle keyframe: the snowstorm monster birth/reveal moment, used for seconds 2-5.
Image 3 is the ending keyframe: the snowstorm monster's first attack shattering a small iceberg, used for seconds 5-10.
Additional Monster Reference 1 is the snowstorm monster primary reference: use it to lock the monster's core visual design, including dark storm-cloud body, blue glowing eyes, cloud-hole mouth, ice crystal accents, wide snow-mist base, powerful but clumsy silhouette. Do not redesign the monster.
Additional Monster Reference 2 is the scale-corrected monster model sheet: use it to lock the size relationship between the monster, blue icebergs, far snow mountains, and small Antarctic animals. The monster must be huge compared with small animals but clearly smaller than large icebergs and far snow mountains.
Additional Monster Reference 3 is the monster pose sheet: use it only for the monster's birth, roaring, swirling-body motion, and blizzard-attack body language. Do not treat it as a story keyframe or split-screen layout.

The video starts from the calm Antarctic establishing keyframe: a peaceful glossy ice field under a pale blue sky, distant snow mountains, large blue icebergs, tiny penguins and seals resting on the ice, and a wooden fish bucket sitting quietly. The atmosphere should feel calm, clean, and safe at first.

From seconds 2 to 5, transition into the monster birth keyframe. The sky gradually darkens from one side, cold wind begins to rise, snow mist curls low across the ice, and the small Antarctic animals slowly notice something wrong. Behind the mid-sized blue icebergs, the snowstorm monster begins to form from swirling snow clouds. Keep the monster design consistent with the uploaded snowstorm monster reference: dark storm-cloud body, blue glowing eyes, cloud-hole mouth, ice crystal accents, wide snow-mist base, powerful but clumsy. Follow the uploaded scale-corrected monster model sheet for scale: use the iceberg, snow mountain, and small animal size relationships shown in the reference image; the monster is huge compared with small animals but clearly smaller than large icebergs and far snow mountains.

From seconds 5 to 10, transition into the first attack keyframe. The snowstorm monster fully emerges and performs its first clear attack. From its wide dark cloud-hole mouth and swirling storm body, a concentrated blue-white blizzard blast shoots sideways across the frame and shatters a small nearby iceberg into sparkling ice chunks. Tiny penguins and seals flee below, the wooden fish bucket slides across the ice, snow dust and ice fragments fly through the air. The action must clearly show cause and effect: monster breathes/blasts -> small iceberg shatters -> animals panic and run.

Camera direction: begin with a wide peaceful establishing shot, then a slow cinematic push-in as the sky darkens and the monster is born, then a stronger dynamic camera move and slight shake during the iceberg-shattering attack. Keep the motion smooth and readable, not chaotic. Maintain a family-friendly Pixar-like 3D animated comedy tone: suspenseful and dangerous, but still cute, clean, and suitable for children. Use icy blue Antarctic palette, soft snow particles, cinematic lighting, clean silhouettes, high quality stylized 3D animation. No text, no subtitles, no watermark.
```

## 负向 Prompt

```text
Gugugaga visible, main character visible, red scarf, blue hair clip, hero penguin, showing the hero too early, monster larger than large icebergs, monster larger than far snow mountains, mountain-sized monster, kaiju scale, ignoring the scale-corrected reference, pure tornado, realistic disaster footage, live action, photorealistic horror, human giant, muscular arms, fists, hands, fingers, legs, feet, crown, beard, old man face, snowman king, sharp teeth, demon, dragon, robot, gore, blood, dark horror tone, unreadable chaos, excessive camera shake, vertical video, wrong aspect ratio, text, logo, watermark, subtitles
```

## 使用建议

- 如果工具支持三张图到视频，把 `KF01A` 作为起始帧、`KF01B` 作为中间关键帧、`KF01C` 作为结束帧。
- 如果工具只支持首尾帧，先用 `KF01A` 到 `KF01B` 生成 4-5 秒“雪怪诞生”，再用 `KF01B` 到 `KF01C` 生成 5-6 秒“雪怪攻击”，最后拼接。
- 如果工具支持负向 prompt，请把“负向 Prompt”单独粘贴到负向输入框。
- 如果工具没有负向 prompt 输入框，请在正向 prompt 末尾追加：`Avoid: Gugugaga visible, main character visible, red scarf, blue hair clip, monster larger than large icebergs, monster larger than far snow mountains, text, logo, watermark.`
