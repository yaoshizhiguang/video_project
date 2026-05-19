# Generation Log 填写说明

`generation_log.csv` 字段说明：

| 字段 | 含义 |
| --- | --- |
| date | 生成日期 |
| episode | 第几集，例如 ep001 |
| segment | 第几段，例如 seg03 |
| model | 使用的视频模型 |
| mode | 文生视频 / 图生视频 / 首尾帧视频 |
| input_reference | 使用的参考图路径 |
| prompt_file | prompt 文件路径 |
| seed | seed，没有则写 none |
| duration | 视频时长 |
| resolution | 分辨率 |
| result_path | 生成结果路径 |
| score | 1-5 分 |
| issue | 存在问题 |
| next_action | 下一步动作 |

## 示例

```csv
2026-05-16,ep001,seg03,model_name,image-to-video,00_references/character/gugugaga_character_ref.png,02_prompts/segments/episode_001_segments.md,12345,3s,540x960,04_preview_tests/episode_001/ep001_seg03_preview_v001.mp4,4,"滑倒动作好，但红围巾有一帧消失","提高角色参考强度后重试"
```
