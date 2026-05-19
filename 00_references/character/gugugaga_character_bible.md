# 咕咕嘎嘎企鹅角色设定

## 核心人设

咕咕嘎嘎企鹅不是一只真实企鹅，而是一个“穿企鹅外套的 Q 版少女 IP / anime penguin-girl mascot character”。它看起来呆呆的，只会说“咕咕”“嘎嘎”。它没有主动战斗能力，也没有明确的英雄意识，但每次都会因为滑倒、撞飞、弹跳、误触机关等意外行为，误打误撞拯救南极。

## 参考图路径

- 原始参考图目录：`00_references/character/images/raw/`
- 当前主参考图：`00_references/character/images/selected/gugugaga_primary_reference.png`
- AI 候选角色图目录：`00_references/character/images/variations/`

使用方式：

- 原始参考图先放入 `images/raw/`，保留原始文件。
- 当前最重要、每次生成都要上传的参考图统一命名为 `images/selected/gugugaga_primary_reference.png`。
- 每次 AI 生成出来的角色候选图放入 `images/variations/`，按 prompt 版本和候选编号命名。

## 固定外观

- 身份：穿企鹅 hood / 企鹅外套的 Q 版少女 IP，不是纯企鹅。
- 脸部：必须保留少女人脸，不能变成鸟脸或真实企鹅脸。
- 发型：必须保留黑短发。
- 发饰：必须保留蓝色发卡。
- 体型：圆滚滚、米团形、小短腿，保持参考图原始比例。
- 眼睛：保留参考图里的原始眼型，大而无辜，略微空洞。
- 原始配饰：主参考图里有胸前 / 脖子处的银色回形针配饰，原图身份锁定版可以保留。
- 红围巾变体：移除原有银色回形针 / 金属夹配饰，用亮红色小围巾替换；红围巾不能遮挡蓝色发卡、黑短发、少女人脸和企鹅 hood 等核心特征。
- 气质：呆萌、认真、慢半拍，看起来不太聪明。
- 行为：摇摇晃晃走路，容易滑倒，动作夸张但可爱。

## 角色一致性描述

```text
Gugugaga is always the same character from the primary reference image: a chibi anime penguin-hoodie girl mascot character, a cute little girl wearing a black plush penguin hood / penguin costume, with a soft simplified human anime girl face area, black bob haircut, blue hairpin, yellow penguin beak on the hood, white fluffy belly patch, rounded body silhouette, yellow penguin feet, silly but serious expression. In the original identity-lock version, the silver paperclip accessory on the chest can stay. In the red scarf variant, remove the silver paperclip / metal clip accessory and replace it with a small bright red scarf around the neck.
```

## 当前推荐角色定稿图 Prompt

```text
原图身份锁定版：`02_prompts/character/gugugaga_character_prompt_v003_penguin_girl_identity.md`
红围巾实验版：`02_prompts/character/gugugaga_character_prompt_v004_red_scarf_variant.md`
```

## 三视图 Prompt

```text
Character turnaround sheet of Gugugaga, the same chibi anime penguin-girl mascot character from the primary reference image, cute little girl wearing a penguin hood / penguin costume, human anime girl face, black bob haircut, blue hairpin, original face shape, original eyes, rounded rice-ball-like body silhouette, tiny cute feet, front view, side view, back view, clean white background, premium stylized 3D animated character look, soft studio lighting, consistent character design, high quality
```

## 视频段落中必须重复的约束

```text
Keep Gugugaga's appearance exactly consistent with the primary reference image. Preserve the anime girl face area, black bob haircut, blue hairpin, penguin hood / costume, yellow beak, white belly patch, body shape, colors, and overall identity. If using the original identity-lock version, the silver paperclip accessory can stay. If using the red scarf variant, remove the original silver paperclip / metal clip accessory and replace it with a small bright red scarf while keeping all other identity features visible. Do not convert her into a real penguin or pure penguin mascot.
```

## 禁止项

- 不要把咕咕嘎嘎做成写实企鹅。
- 不要把咕咕嘎嘎做成纯企鹅吉祥物。
- 不要删除少女人脸、黑短发、蓝色发卡。
- 原图身份锁定版不要随意删除胸前银色回形针。
- 红围巾版本不要保留银色回形针、金属夹或项链夹。
- 不要让红围巾遮住脸、发卡或黑短发。
- 不要变成瘦高体型。
- 不要增加武器、盔甲、披风等复杂配件。
- 不要让它说完整人话，只能“咕咕”“嘎嘎”。
