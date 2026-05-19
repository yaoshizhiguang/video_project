# Gugugaga Character Prompt v002 - Reference First

## 用途

用于基于已提供的咕咕嘎嘎参考图生成角色设定图。目标不是重新设计角色，而是保留参考图里的咕咕嘎嘎形象，只做轻微美化、清晰化和角色设定图整理。

## 适用场景

- 图生图
- 角色定稿
- 参考图优先
- 全身角色图
- 轻微修图，不重画角色

## 正向 Prompt

```text
Use the provided reference image as the primary source. Keep the character identity, face, body shape, proportions, colors, and overall cute internet-meme mascot feeling from the reference image. Only make small refinements to turn it into a clean full-body character design sheet.

A cute chubby Gugugaga mascot character, round rice-ball shaped body, tiny short legs, big innocent eyes, silly but serious expression, slightly clueless and slow-reacting personality, adorable, clumsy, harmless, bright red scarf kept clearly visible, simple front-facing standing pose, clean light background, subtle icy floor, premium stylized 3D animated mascot look, soft studio lighting, high quality character sheet, consistent proportions, full body, front view.

Do not redesign the character. Do not turn it into a realistic penguin. Follow the reference image closely.
```

## 负向 Prompt

```text
realistic penguin, wildlife documentary, real bird anatomy, natural penguin feathers, scary, aggressive, superhero armor, cape, weapon, human body, tall thin body, long legs, extra limbs, deformed eyes, missing red scarf, different scarf color, complex background, multiple characters, text, logo, watermark, blurry, low quality, redesigned character, not following reference image
```

## 推荐参数

| 参数 | 建议 |
| --- | --- |
| reference strength | 80-90% |
| style strength | 40-60% |
| prompt strength | 40-60% |
| aspect ratio | 1:1 或 3:4 |
| output | full-body character sheet |

## 使用说明

- 必须配合参考图使用。
- 参考图优先级应高于文字 prompt。
- 目标是“修整参考图角色”，不是“生成一只企鹅”。
- 如果仍然生成真实企鹅，继续降低 `penguin` 相关词权重，改用 `mascot character` / `cartoon creature` / `internet meme character`。

## 生成记录

| 日期 | 模型 | 结果 | 问题 | 下一步 |
| --- | --- | --- | --- | --- |
| 2026-05-16 | 待填写 | 待生成 | 待记录 | 使用参考图高权重测试 |
