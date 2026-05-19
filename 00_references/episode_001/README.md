# Episode 001 Reference Assets

## Purpose

Stores episode-specific reference assets that are not owned by a single character or monster.

Character-specific assets should stay under:

- `00_references/character/images/model_sheets/`
- `00_references/character/images/pose_sheets/`

Monster-specific assets should stay under:

- `00_references/monster/images/model_sheets/`
- `00_references/monster/images/pose_sheets/`

## Folder Map

| Folder | Purpose |
| --- | --- |
| `scale_lineup/` | Scale comparison sheets for Gugugaga, monster, animals and props |
| `props/` | Fish bucket, fish, ice gong, ice pillar, snowball and final snowman props |
| `environments/` | Antarctic ice field, icebergs, snow mountain, ice gong area and sky states |
| `vfx/` | Blizzard, snow particles, blue glow, avalanche, sound waves and snow wipe effects |
| `final_selected/` | Selected episode-level reference assets ready for keyframes and video generation |
| `rejected/` | Rejected or failed episode-level generations kept for review |

## Naming Rules

- Scale lineup: `ep001_scale_lineup_v001.png`
- Props: `ep001_props_<description>_v001.png`
- Environments: `ep001_env_<description>_v001.png`
- VFX: `ep001_vfx_<description>_v001.png`

## Selection Rule

Only copy assets into `final_selected/` after they pass consistency checks against the confirmed reference images and episode story.
