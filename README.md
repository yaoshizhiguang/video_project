# 咕咕嘎嘎企鹅 AI 视频工程

这个工程用于记录“咕咕嘎嘎企鹅”系列 AI 视频从创意、角色设定、脚本、prompt、关键帧、预览试错到最终导出的全过程。

## 当前项目方向

- IP 名称：咕咕嘎嘎企鹅。
- 核心类型：反差英雄 + 萌系动作喜剧。
- 第一集：《咕咕嘎嘎企鹅：滑倒拯救南极》。
- 叙事核心：主角看起来呆呆的，只会“咕咕嘎嘎”，但误打误撞拯救南极。

## 目录说明

- `00_references/`: 角色、怪物、风格参考图和设定文档。
- `01_scripts/`: 每集剧本、分镜、旁白、音效设计。
- `02_prompts/`: 基础 prompt、分段 prompt、负面词和模型参数。
- `03_keyframes/`: 每段视频的首帧、尾帧和关键帧 prompt。
- `04_preview_tests/`: 低成本预览、小样、失败版本和试错流程。
- `05_video_clips/`: 正式生成的视频片段和最终选中片段。
- `06_audio/`: 旁白、BGM、音效。
- `07_editing/`: 剪辑工程、时间线、工程文件。
- `08_exports/`: 草稿导出和最终成片。
- `09_logs/`: 每次生成的参数、结果、问题和决策记录。
- `assets/`: 字体、贴纸、覆盖层等通用素材。

## 推荐流程

1. 在 `00_references/character/` 固定咕咕嘎嘎角色图。
2. 在 `00_references/monster/` 固定暴风雪怪图。
3. 在 `03_keyframes/episode_001/` 生成每段关键帧。
4. 将关键帧整合成单张故事板图，作为视频生成的剧情流程输入。
5. 在 `04_preview_tests/episode_001/` 做 2-3 秒低成本小样。
6. 通过后在 `05_video_clips/episode_001/` 生成 10 秒正式片段。
7. 选中片段复制到 `05_video_clips/selected/`。
8. 剪辑工程放到 `07_editing/`。
9. 导出草稿到 `08_exports/drafts/`，最终成片到 `08_exports/final/`。
10. 每次生成都更新 `09_logs/generation_log.csv`。

## 视频生成输入方法论

- 默认不要把多张独立关键帧同时上传给视频模型。
- 先用关键帧确定剧情阶段，再生成一张单图参考；如果是故事板，它只用于阶段、构图和状态参考；如果是静态布局图，它只用于背景元素、动物初始位置、道具位置和怪物最终站位参考。
- 视频生成时优先上传：角色/怪物设定图 + 单张故事板图或单张静态布局图。
- 单图参考不能替代动态描述。
- Prompt 必须用中文清楚描述所有运动、特效、时间轴、能量流向、因果关系和起止状态。
- Prompt 必须要求把故事板转化为一镜到底的连续动画，并禁止显示分格、caption、白边、硬切、淡入淡出和幻灯片式转场。

## 最重要的一致性规则

```text
Gugugaga is always the same character: a cute round chubby penguin with a rice-ball shaped body, bright red scarf, big innocent eyes, tiny short legs, small orange beak, silly but serious expression.
```

每段视频都必须保留亮红色围巾，其他企鹅不能戴红围巾。
