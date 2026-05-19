# 暴风雪怪设计复盘 - 2026-05-17

## 当前结论

先暂停继续生成。当前问题不是某一版 prompt 不够精确，而是我们在几个互相冲突的方向之间反复摇摆：主参考需要的是“有角色轮廓的雪云怪”，但 prompt 经常被推向“雪人王”“灾害墙”“肌肉云巨人”或“过度喜剧靶子”。

## 最接近主参考的方向

`00_references/monster/images/variations/snowstorm_monster_v001_001.png` 仍然是最接近主参考的候选。

它的优点：

- 有清晰角色轮廓：蓝眼睛、云雾大嘴、雪云身体、模糊粗壮云臂。
- 有 boss 压迫感，但还没有变成写实灾害片。
- 有儿童动画可接受的怪物感，不是老人、雪人王、冰巨人或纯自然灾害。
- 和咕咕嘎嘎形成反差：小主角面对大雪云怪，喜剧结构成立。

它的问题：

- 人形趋势已经开始出现，尤其是粗壮手臂和站立姿态。
- “笨重、会被包成雪人”的剧情功能还不够明确。
- 视觉记忆点够用但不够惊艳，短视频首帧吸引力还可加强。

## 过去案例问题

| 样本 | 主要问题 | 根因 |
| --- | --- | --- |
| v001 | 最接近方向，但略有人形手臂和史诗 boss 倾向 | `vague bulky arm shapes`、`powerful`、`intimidating` 同时触发了巨人轮廓 |
| v002 | 更圆但压迫感下降，腿部/站立感出戏 | 为了变圆加入 `round bulky body`，但没有锁住下半身云雾结构 |
| v005 | 剧情功能对了，但变普通，吸睛不足 | 过度强调 `round`、`snowman`、`target`，削弱了 boss 记忆点 |
| v006/v007 雪人王 | 太像人、友善、违和，不像 boss | `king`、`crown`、`eyebrows`、`beard`、`mustache`、`goofy` 强触发老人雪人王 |
| v008 灾害墙 | 不像人了，但太写实、太灾害奇观，缺少角色轮廓 | `living blizzard wall`、`natural disaster`、`snow-tsunami` 把模型推向场景而非角色 |
| v009 云团巨人 | 回到角色但太像肌肉云巨人，嘴过大，轮廓过满 | `cloud-arm shapes`、`thick rounded body`、`boss-like` 叠加后生成健身怪轮廓 |

## 真正的设计约束

必须保留：

- 两只冷蓝色发光眼睛。
- 一个模糊的云雾大嘴，但不能是恐怖深洞或笑脸。
- 主体是雪云怪，不是雪人、老人、冰巨人、纯云墙或龙卷风。
- 体型巨大，能压住画面，但轮廓要简单。
- 身体大、厚、慢、笨重，最终能被雪球包成巨大雪人。

必须避免：

- `king`、`crown`、`beard`、`mustache`、`eyebrows`：会变雪人王/老人。
- `humanoid`、`shoulders`、`fists`、`muscular arms`、`body`：会变肌肉巨人。
- `snowman silhouette`、`round snowman`：会提前变成雪人，失去怪物感。
- `living blizzard wall`、`natural disaster`、`snow-tsunami`：会变成背景灾害，缺少角色。
- 过度强调 `goofy`、`friendly`：会削弱 boss 感。
- 过度强调 `intimidating`、`powerful`：会推向史诗最终 boss。

## 建议的下一步

先不要继续生成。建议先做一页“怪物设计规格表”，把视觉元素分成必选、可选、禁止三类，再决定是否继续 prompt。

下一版若要继续，应该采用“v001 结构锁定 + 限制改动”的策略：

- 只允许调整光效、冰晶数量、身体边缘和表情强度。
- 不再新增身份词，如 king、lord、titan、wall。
- 不再新增人脸装饰词，如 beard、eyebrows、mustache。
- 不再使用 `snowman` 描述当前形态，只描述“later can be wrapped into a snowman”。
- 不再把“好包成雪人”写成外观，而写成剧情功能。

已落地文件：

- `02_prompts/monster/snowstorm_monster_design_spec_v001.md`
- `02_prompts/monster/snowstorm_monster_prompt_v010_v001_locked_refine.md`

v010 的关键限制：

- 以 `snowstorm_monster_v001_001.png` 为主参考。
- 只做小幅强化，不重新发明怪物。
- 惊艳来源限定为光效、体量、蓝色内发光、冰晶漂浮和风雪氛围。
- 禁止使用 `King / crown / beard / snowman-like / wall / natural disaster` 作为正向方向。
- 当前形态不能直接写成雪人，只能写“之后能被雪球包成巨大雪人”。

## 当前 v009 评价

`00_references/monster/images/variations/snowstorm_monster_v009_001.png` 比雪人王方向更接近怪物，但不应作为主参考。

优点：

- 有清晰 boss 体量。
- 蓝眼睛、冰晶、蓝色内发光都有吸睛效果。
- 相比雪人王，少了老人感和友善笑脸。

问题：

- 过度厚重，像云团肌肉巨人。
- 大嘴太像恐怖空洞，儿童动画安全感变弱。
- 双臂太像拳头，重新触发人形怪问题。
- 画面复杂度比 v001 高，轮廓不如 v001 清晰。

建议状态：保留为失败复盘样本，不选主参考。

## 当前 v010 评价修正

`00_references/monster/images/variations/snowstorm_monster_v010_001.png` 是合规候选，但不应高于 v001。

优点：

- 保留了雪云怪主体，没有跑向雪人王、冰巨人、灾害墙或肌肉怪。
- 蓝色内发光、漂浮冰晶和风雪氛围比 v001 更干净。
- 侧翼没有明显变成拳头或手掌。

问题：

- 整体偏白偏软，暗色暴风云体块弱于 v001。
- 表情更像惊讶或可爱，开场 boss 压迫感不如 v001。
- 画面更亮更干净，但“更干净”不等于“更适合主参考”。
- v001 的粗粝风暴感、危险感和简单怪物轮廓仍更关键。

修正结论：v001 仍是主参考优先级第一；v010 只作为“合规但偏软”的对照候选。

## 当前 v011 评价修正

`00_references/monster/images/variations/snowstorm_monster_v011_001.png` 此前被误判为技术性失败。重新读取文件后确认：它是与 v001 非常接近的雪云怪候选，不是现实照片拼贴。

优点：

- 与 v001 的主体方向高度一致：巨大雪云身体、蓝色发光眼、云洞大嘴、冰晶点缀、南极冰面场景。
- 比 v010 更接近 v001，没有明显洗白成软萌怪。
- 仍然有儿童动画 boss 的体量感和可读轮廓。

问题：

- 相比 v001，冰晶更集中在头顶，略有“冠”的风险。
- 手部末端更像爪或手，仍需警惕人形化。
- 整体仍略偏明亮，v001 的暗色风暴压迫感更稳。

修正结论：v011 恢复为强候选，应与 v001 并排评估；此前“技术性失败/废弃”结论作废。
