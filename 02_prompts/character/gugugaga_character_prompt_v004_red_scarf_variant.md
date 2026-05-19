# Gugugaga Character Prompt v004 - Red Scarf Variant

## 用途

用于基于主参考图生成“红围巾版咕咕嘎嘎”。该版本保留参考图里的企鹅外套少女身份，但移除原图脖子 / 胸前的银色回形针配饰，并用醒目的红围巾替换它，不重新设计角色。

## 参考图

- 当前主参考图路径：`00_references/character/images/selected/gugugaga_primary_reference.png`
- 原始参考图目录：`00_references/character/images/raw/`
- 候选角色图输出目录：`00_references/character/images/variations/`

生成时必须上传当前主参考图，并优先遵循参考图。文字 prompt 只用于约束“小修”和“替换配饰”，不能覆盖参考图身份。红围巾是对原图脖子 / 胸前银色回形针配饰的替换，只替换这个配饰；不能覆盖或替代少女人脸、黑短发、蓝色发卡、企鹅 hood、白肚皮等核心身份特征。

## 核心修正

- 保留参考图中的少女人脸 / 简化脸部区域。
- 保留黑短发。
- 保留蓝色发卡。
- 保留企鹅 hood / 黑色毛绒企鹅外套身份，主体是“穿企鹅服的 Q 版少女”，不是动物企鹅。
- 保留 hood 上的黄色嘴、白色肚皮、黄色小脚等服装特征。
- 移除原图脖子 / 胸前的银色回形针装饰，不要让回形针、金属夹或项链夹残留可见。
- 用亮红色小围巾替换原有脖子 / 胸前配饰，围在脖子处，成为醒目的系列化识别元素。
- 不要把角色改成纯企鹅。
- 不要把角色改成真实企鹅。

## 正向 Prompt

```text
Use the provided reference image as the strict primary source. This is not a real penguin and not an animal-only mascot. Preserve the exact character identity from the reference image: a chibi anime little girl wearing a black plush penguin hooded costume, with a soft simplified human anime girl face area, black bob haircut visible under the hood, blue hairpin on the left side, a yellow beak attached to the hood, white fluffy belly patch on the costume, rounded rice-ball-like body proportions, tiny cute costume feet, plush toy texture, silly but serious expression.

Create a red scarf variant of the same reference character. Remove only the original silver paperclip / metal clip accessory from the neck or chest area, and replace it with a small bright red scarf around her neck. The red scarf must be bright red, soft, cute, clearly visible, and must not cover the face, black hair, blue hairpin, penguin hood, or white belly patch.

Only make small refinements: clean up the design, improve lighting and polish, keep the same face area, same hairstyle, same blue hairpin, same hood shape, same body proportions, same cute plush costume identity. Simple front-facing standing pose, clean light background, subtle icy floor, premium stylized 3D animated character sheet, soft studio lighting, high quality, full body, front view.

Do not redesign the character. Do not convert her into a real penguin. Do not make an animal-only penguin mascot. Do not remove the anime girl face area. Do not remove the black bob haircut. Do not remove the blue hairpin. Do not keep the silver paperclip accessory. Follow the reference image closely, only replacing the original neck / chest accessory with the red scarf.
```

## 负向 Prompt

```text
realistic penguin, pure penguin mascot, animal-only mascot, bird-only character, real bird anatomy, natural penguin feathers, wildlife documentary, Antarctic penguin, no human face, missing anime girl face area, missing black bob haircut, missing blue hairpin, silver paperclip accessory, paperclip on chest, metal clip, necklace clip, original chest clip still visible, missing red scarf, red scarf covering the face, red scarf covering hair, red scarf covering blue hairpin, redesigned character, different face, different hairstyle, different body proportions, not following reference image, scary, aggressive, superhero armor, cape, weapon, tall thin body, long legs, extra limbs, deformed eyes, complex background, multiple characters, text, logo, watermark, blurry, low quality
```

## 推荐参数

| 参数 | 建议 |
| --- | --- |
| reference strength | 90-95% |
| style strength | 25-45% |
| prompt strength | 35-45% |
| denoise / variation | 低 |
| aspect ratio | 1:1 或 3:4 |
| output | full-body character sheet |

## 使用说明

- 这一版必须配合主参考图使用。
- 目标是“把原角色脖子 / 胸前的银色回形针配饰替换成红围巾”，不是重新设计一个角色。
- 如果工具支持参考图权重，把参考图权重拉到最高或接近最高；文字 prompt 不要盖过参考图。
- 如果模型仍保留回形针、金属夹或项链夹，继续强化 `remove the original silver paperclip accessory` 和 `replace it with a red scarf`。
- 如果红围巾导致蓝色发卡消失，降低 prompt strength 或明确要求蓝色发卡仍可见。
- 如果模型又变成纯企鹅，继续弱化 `penguin mascot`，强化 `chibi anime little girl wearing a plush penguin hooded costume`。

## 生成记录

| 日期 | 模型 | 结果 | 问题 | 下一步 |
| --- | --- | --- | --- | --- |
| 2026-05-16 | 待填写 | 待生成 | 待记录 | 测试红围巾是否能替换原有银色回形针配饰 |
