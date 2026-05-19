# Gugugaga Character Prompt v003 - Penguin Girl Identity Lock

## 用途

用于基于参考图生成咕咕嘎嘎角色设定图。该版本不再把角色定义为“真实企鹅”或“纯企鹅吉祥物”，而是明确锁定为“穿企鹅外套的 Q 版少女 IP / anime penguin-girl mascot character”。

## 参考图

- 当前主参考图路径：`00_references/character/images/selected/gugugaga_primary_reference.png`
- 原始参考图目录：`00_references/character/images/raw/`
- 候选角色图输出目录：`00_references/character/images/variations/`

生成时必须上传当前主参考图，并优先遵循参考图。文字 prompt 只用于约束“小修”和“不要跑偏”。

## 核心修正

- 保留参考图中的少女人脸。
- 保留黑短发。
- 保留蓝色发卡。
- 保留企鹅 hood / 企鹅外套身份。
- 保留米团身体和原始比例。
- 不要把角色改成纯企鹅。
- 不要把角色改成真实企鹅。

## 正向 Prompt

```text
Use the provided reference image as the strict primary source. Preserve the exact character identity from the reference image: a chibi anime penguin-girl mascot character, a cute little girl wearing a penguin hood / penguin costume, with a human anime girl face, black bob haircut, blue hairpin, original face shape, original eyes, original proportions, rounded rice-ball-like body silhouette, tiny cute feet, soft cute expression, slightly silly but serious personality.

Only make small refinements: clean up the design, make the full-body character sheet clearer, improve lighting and polish, keep the same character identity, keep the same face, keep the same hairstyle, keep the same blue hairpin, keep the same penguin-hood girl concept. Simple front-facing standing pose, clean light background, subtle icy floor, premium stylized 3D animated character look, soft studio lighting, high quality character sheet, consistent proportions, full body, front view.

Do not redesign the character. Do not convert her into a real penguin. Do not remove the anime girl face. Do not remove the black bob haircut. Do not remove the blue hairpin. Follow the reference image closely.
```

## 负向 Prompt

```text
realistic penguin, pure penguin mascot, real bird anatomy, natural penguin feathers, wildlife documentary, Antarctic penguin, animal-only character, no human face, missing anime girl face, missing black bob haircut, missing blue hairpin, redesigned character, not following reference image, scary, aggressive, superhero armor, cape, weapon, tall thin body, long legs, extra limbs, deformed eyes, complex background, multiple characters, text, logo, watermark, blurry, low quality
```

## 推荐参数

| 参数 | 建议 |
| --- | --- |
| reference strength | 90-95% |
| style strength | 30-50% |
| prompt strength | 35-50% |
| denoise / variation | 低 |
| aspect ratio | 1:1 或 3:4 |
| output | full-body character sheet |

## 使用说明

- 这一版必须配合参考图使用。
- 默认参考图为 `00_references/character/images/selected/gugugaga_primary_reference.png`。
- 如果工具支持参考图权重，把参考图权重拉到最高或接近最高。
- 不要再使用 `Antarctic penguin` 作为主体定义。
- 如果模型仍然变成纯企鹅，进一步弱化 `penguin`，改成 `penguin-hood girl` / `girl in penguin costume` / `chibi anime girl mascot`。

## 生成记录

| 日期 | 模型 | 结果 | 问题 | 下一步 |
| --- | --- | --- | --- | --- |
| 2026-05-16 | 待填写 | 待生成 | 待记录 | 用高参考图权重测试 |
