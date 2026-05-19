# 暴风雪怪设定

## 核心定位

暴风雪怪是第一集的喜剧型灾难反派，由乌云、雪团、少量冰晶和雪雾组成。它体型巨大，第一眼有压迫感和记忆点，但本质笨重、慢半拍，像一个会被咕咕嘎嘎误打误撞包成雪人的巨大靶子。它不是普通雪云怪，也不能设计成史诗冰雪 Boss、风暴泰坦或冰巨人；更准确的方向是“南极暴风雪之王，一个圆滚滚、发着极光蓝光、戴冰晶王冠的笨蛋反派”。

## 固定外观

- 身体：巨大的圆滚滚乌云雪团，像活的暴风雪雪人雏形。
- 眼睛：发光的极光蓝眼睛，表情略呆、略困惑，也可以有点“我很可怕吧？”的过度自信。
- 记忆点：头顶有天然蓝色冰晶王冠，肩部有少量漂亮蓝色冰晶装饰，身体缠绕淡蓝色极光光带。
- 面部特征：夸张白色云眉毛、大云胡子 / 云髭，软椭圆云洞嘴，不要尖牙。
- 轮廓：整体偏圆、厚重、可读，接近三层巨大雪云雪人比例，有模糊雪云手臂。
- 下半身：宽宽软软的旋转雪雾底座，像蓬松旋转雪堆，不是细长龙卷风，不是双腿。
- 质感：乌云、蓬松雪团、雪雾、少量冰晶混合；冰晶只是装饰，不是武器或盔甲。
- 气质：看起来巨大但笨重，吓人但不聪明，适合被喜剧连锁反应制服。
- 结局形态：被雪球包成巨大无害三层雪人，脸上插着一条鱼。

## 参考图路径

- 原始参考图目录：`00_references/monster/images/raw/`
- 当前主参考图：`00_references/monster/images/selected/snowstorm_monster_primary_reference.png`
- AI 候选怪物图目录：`00_references/monster/images/variations/`

使用方式：

- 原始素材或外部参考先放入 `images/raw/`，保留原始文件。
- 每次 AI 生成出来的雪怪候选图放入 `images/variations/`，按 prompt 版本和候选编号命名。
- 当前最重要、每次生成都要上传的雪怪参考图统一命名为 `images/selected/snowstorm_monster_primary_reference.png`。

## 怪物设定图 Prompt

当前推荐版本：`02_prompts/monster/snowstorm_monster_prompt_v006_memorable_storm_king.md`

### 正向 Prompt

```text
A clean single creature concept art of the Antarctic Snowstorm King, a memorable family-friendly villain for a cute Pixar-like animated comedy short film. He is not an epic final boss, but a huge round clumsy snowstorm boss who looks impressive at first glance, then funny and a little dumb on second glance. The design must be eye-catching and easy to remember. The monster has a giant rounded snow-cloud snowman silhouette, with a large round head, a bulky round upper snow-cloud body, and a wide soft swirling snow-cloud base that looks easy to wrap into a giant snowman later. No legs, no feet, no sharp tornado funnel. His body is made of dark storm clouds, fluffy white snow, soft snow mist, and a few beautiful blue ice crystals. Give him strong visual anchors: a natural blue ice crystal crown on top of his head, a few elegant blue ice crystal shoulder ornaments, subtle aurora-blue glowing lines swirling around his snow-cloud body, oversized fluffy white cloud eyebrows, and a big curled cloud beard / cloud mustache. His eyes glow bright aurora blue, but the expression is goofy and overconfident, like “I am scary, right?” while actually being slow and dumb. Use a soft oval cloud-mouth with a silly grin or harmless open “aww” expression, no teeth, no sharp mouth edges. The monster should feel large enough to scare tiny Antarctic animals, but still funny, rounded, and family-friendly. Keep the silhouette simple, readable, iconic, and toy-like. Antarctic icebergs frame the lower sides for scale without blocking the body. Clean centered creature design, cute cinematic 3D animation style, icy blue Antarctic color palette, aurora blue glow, soft snow particles, high quality character concept art, front view.
```

### 负向 Prompt

```text
ugly snow lump, plain snow cloud, forgettable design, generic cloud monster, epic final boss, evil demon, storm titan, ice titan, ice giant, wind demon, tornado monster, sharp tornado funnel, realistic tornado, disaster movie, realistic storm, horror monster, scary horror, nightmare creature, dragon, golem, muscular body, human body, human legs, two legs, feet, shoes, pants, human lower body, standing humanoid, ice armor, crystal armor, weapon, sharp claws, sharp teeth, too many teeth, blood, gore, skull, corpse, zombie, red eyes, too many sharp spikes, full body covered in spikes, aggressive monster roar, wide scary mouth, thin body, tall skinny body, overly complex silhouette, unreadable silhouette, collage, split image, photo overlay, real person, human photo, text, logo, watermark, blurry, low quality
```

## 视频中固定描述

```text
A giant clumsy Antarctic Snowstorm King made of dark storm clouds, fluffy snow piles, soft snow mist, a few blue ice crystals, aurora-blue glowing lines, glowing blue eyes, cloud eyebrows, and a curled cloud beard; huge, round, memorable, slightly dumb, family-friendly, and easy to wrap into a giant snowman.
```

## 禁止项

- 不要血腥。
- 不要骷髅、尖牙过多、恐怖片风格。
- 不要写实灾难片质感。
- 不要让怪物太复杂导致模型无法复现。
- 不要红眼睛，固定发光蓝眼睛。
- 不要做成纯龙、纯巨人、纯人形肌肉怪。
- 不要出现双腿、脚、裤子或人类下半身；下半身应是旋转雪雾 / 暴风云柱。
- 不要拼贴、分屏、照片叠加、真人遮挡或画面污染；必须是单一完整雪怪设定图。
- 不要设计成史诗最终 Boss、风暴泰坦、冰巨人、龙卷风魔王。
- 不要让冰晶成为主体；冰晶只能少量点缀，方便后续被雪覆盖成雪人。
- 不要血盆大口或尖牙；嘴巴应是软椭圆云洞嘴，笨笨张开。
- 不要做成没有记忆点的普通雪团；必须保留冰晶王冠、极光蓝纹路、云眉毛 / 云胡子等视觉锚点。
