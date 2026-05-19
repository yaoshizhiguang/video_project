# Episode 001 Keyframe Directory

This directory stores keyframe prompts and generated keyframe images for episode 001.

## Aspect Ratio

- Current production aspect ratio: `16:9` horizontal.
- Do not use old `9:16` vertical prompts for episode 001 keyframes.

## Prompt Files

- `ep001_keyframe_prompts_v004_progressive_monster_birth_ice_magic_no_crystals.md`: current ice-magic-safe variant; based on v003 but avoids floating rhombus crystals and cheap hard-crystal VFX.
- `ep001_keyframe_prompts_v003_progressive_monster_birth.md`: current Segment 01 progressive monster birth prompt file.
- `ep001_keyframe_prompts_v002_continuity_rebuild.md`: previous continuity rebuild prompt, kept for history.
- `ep001_keyframe_prompts_v001.md`: early 12-keyframe prompt file, kept for history.
- `keyframe_prompts.md`: early draft, kept for history only.

## Prompt Version Rule

Do not directly overwrite an established prompt file when revising prompt wording. Create a new version file instead, then record the reason in `09_logs/decision_log.md`.

## Segment 01 Progressive Output Folders

- `KF01A_master_calm_antarctica/`: selected master plate for the continuous Antarctic environment.
- `KF01B_crisis_start/`: crisis begins; weather changes but no readable monster yet.
- `KF01C_monster_forming/`: monster body prototype starts forming around a belly storm core; no blue eyes, mouth, full face, full arms, or attack yet.
- `KF01D_monster_half_formed/`: monster is half-formed and rising, still not fully solid.
- `KF01E_monster_reveal_attack_ready/`: complete monster reveal and attack preparation.
- `KF01F_monster_first_attack/`: monster shatters a small iceberg with its first blizzard attack.

## Earlier Segment 01 Folders

- `_discarded_legacy/old_segment01_folders/KF01A_calm_antarctica/`: old calm Antarctica candidate.
- `_discarded_legacy/old_segment01_folders/KF01B_monster_birth/`: old monster birth candidate; background continuity was not reliable.
- `_discarded_legacy/old_segment01_folders/KF01C_monster_first_attack/`: old first attack candidate; background continuity was not reliable.
- `_discarded_legacy/misfiled_or_superseded/`: individual misfiled or superseded keyframe files preserved for traceability.

## Later Episode Keyframe Output Folders

- `KF02A_gugugaga_appears/`: Gugugaga appears with innocent expression.
- `KF02B_gugugaga_charge_ready/`: Gugugaga becomes serious and prepares to charge.
- `KF03A_hero_first_step/`: Gugugaga takes the heroic first step.
- `KF03B_first_slip/`: Gugugaga slips immediately.
- `KF04A_bucket_impact/`: Gugugaga hits the fish bucket.
- `KF04B_ice_pillar_to_gong/`: ice pillar falls toward the ice gongs.
- `KF05A_gong_avalanche/`: ice gongs trigger the avalanche.
- `KF05B_snowball_to_monster/`: rolling snowball rushes toward the monster.
- `KF06A_snowball_hits_monster/`: snowball hits and wraps the monster.
- `KF06B_final_snowman/`: final harmless giant snowman reveal.

## Naming

- Candidate image: `ep001_<keyframe_id>_candidate_v001.png`
- Revised candidate: `ep001_<keyframe_id>_candidate_v002.png`
- Selected image: `ep001_<keyframe_id>_selected.png`
- Composition or rejected reference image: `ep001_<keyframe_id>_reference_<reason>_v001.png`

Example:

```text
ep001_KF03B_candidate_v001.png
ep001_KF03B_selected.png
```

## Selection Rule

Keep all generated candidates in the matching keyframe folder. When a candidate is accepted, copy or rename it to the selected filename in the same folder.

## Video Input Rule

For video generation, do not upload these keyframes as separate direct references for the same clip. Use them to create a single storyboard image, then upload the character/monster design reference plus that storyboard image. The video prompt must convert the storyboard into one smooth continuous shot and must forbid visible panels, captions, gutters, hard cuts, fades, dissolves, and slideshow transitions.

The storyboard is only a stage, composition, and state reference. Do not rely on the video model to infer motion, VFX, or cause and effect from storyboard panels. All motion, VFX timing, energy flow, object movement, character reactions, and continuity rules must be written explicitly in the video prompt. Future video prompts should be Chinese by default unless the user asks otherwise.

## Current Segment 01 Selection

- Shot A: `03_keyframes/episode_001/KF01A_master_calm_antarctica/ep001_KF01A_selected.png`
- Shot B: `03_keyframes/episode_001/KF01B_crisis_start/ep001_KF01B_from_selected_A_candidate_v001.png`
- Shot C: `03_keyframes/episode_001/KF01C_monster_forming/ep001_KF01C_selected.png`
- Shot D latest candidate: `03_keyframes/episode_001/KF01D_monster_half_formed/ep001_KF01D_eyes_lit_body_forming_candidate_v001.png`
- Shot E latest candidate: `03_keyframes/episode_001/KF01E_monster_reveal_attack_ready/ep001_KF01E_full_body_animals_flee_candidate_v001.png`
- Shot F latest candidate: `03_keyframes/episode_001/KF01F_monster_first_attack/ep001_KF01F_sweeping_ice_ray_candidate_v001.png`
- Shot F attack sequence v001:
  - `03_keyframes/episode_001/KF01F_monster_first_attack/ep001_KF01F_01_vortex_charge_candidate_v001.png`
  - `03_keyframes/episode_001/KF01F_monster_first_attack/ep001_KF01F_02_mouth_charge_candidate_v001.png`
  - `03_keyframes/episode_001/KF01F_monster_first_attack/ep001_KF01F_03_ray_sweep_candidate_v001.png`
  - `03_keyframes/episode_001/KF01F_monster_first_attack/ep001_KF01F_04_after_ray_vortex_fade_candidate_v001.png`

Shot C selected source candidate:

- `03_keyframes/episode_001/KF01C_monster_forming/ep001_KF01C_animals_facing_storm_candidate_v002.png`

The earlier local file at that path was preserved as:

- `03_keyframes/episode_001/KF01C_monster_forming/ep001_KF01C_animals_facing_storm_candidate_v002_previous_local.png`

## Current Storyboards

- Segment 01 attack vortex ray storyboard: `03_keyframes/episode_001/storyboards/ep001_segment01_attack_vortex_ray_storyboard_v001.png`
- Segment 02 Gugugaga entrance storyboard: `03_keyframes/episode_001/storyboards/ep001_segment02_gugugaga_entrance_storyboard_v001.png`
- Storyboard records: `03_keyframes/episode_001/storyboard_records/ep001_storyboard_log.md`

## Current Video Prompts

- Segment 01 attack vortex ray prompt: `02_prompts/segments/ep001_segment01_attack_vortex_ray_prompt_v001_zh.md`
- Segment 01 attack vortex ray no-crystal prompt candidate: `02_prompts/segments/ep001_segment01_attack_vortex_ray_prompt_v002_ice_magic_no_crystals_zh.md`
- Segment 01 progressive birth no-crystal prompt candidate: `02_prompts/segments/ep001_segment01_progressive_birth_video_prompt_v004_ice_magic_no_crystals.md`
- Segment 01 progressive birth Chinese storyboard-first prompt: `02_prompts/segments/ep001_segment01_progressive_birth_video_prompt_v005_zh_storyboard_first_no_crystals.md`
- Segment 01 progressive birth Chinese static-layout no-attack prompt: `02_prompts/segments/ep001_segment01_progressive_birth_video_prompt_v006_zh_static_layout_no_attack.md`
- Segment 01 progressive birth Chinese frontloaded no-attack prompt: `02_prompts/segments/ep001_segment01_progressive_birth_video_prompt_v007_zh_frontloaded_no_attack.md`
- Segment 01 progressive birth Chinese magic VFX slow-retreat prompt: `02_prompts/segments/ep001_segment01_progressive_birth_video_prompt_v008_zh_magic_vfx_slow_retreat.md`
