# Gugugaga Character Prompt v001 - 初始企鹅描述版

## 用途

用于第一次生成咕咕嘎嘎角色设定图。该版本偏“企鹅角色设计”，第一次实测后发现模型容易生成真实企鹅，因此仅保留为历史版本，不建议继续使用。

## 适用场景

- 历史记录
- 复盘 prompt 问题
- 不建议作为下一轮主 prompt

## 正向 Prompt

```text
Full-body character design of Gugugaga, a cute chubby little Antarctic penguin, rice-ball shaped round body, tiny short legs, big innocent eyes, small orange beak, small orange feet, soft black and white feathers, wearing a bright red scarf, silly but serious expression, slightly clueless and slow-reacting personality, adorable, clumsy, harmless, no weapon, no armor, no cape, standing still in a simple front-facing pose, clean light background, subtle icy floor, premium stylized 3D animated film look, soft studio lighting, high quality character sheet, consistent proportions, front view
```

## 负向 Prompt

```text
realistic penguin, wildlife documentary, scary, aggressive, superhero armor, cape, weapon, human body, tall thin body, long legs, extra limbs, deformed eyes, missing red scarf, different scarf color, complex background, multiple characters, text, logo, watermark, blurry, low quality
```

## 生成结果复盘

| 日期 | 结果 | 问题 | 下一步 |
| --- | --- | --- | --- |
| 2026-05-16 | 失败 | 生成了一只真实企鹅，没有遵循参考图 | 改用 v002 reference-first prompt |

## 问题分析

- `Antarctic penguin`、`soft black and white feathers`、`small orange beak` 等词把模型拉向真实企鹅。
- 没有明确“参考图优先”。
- 没有强调“不要重新设计角色”。
