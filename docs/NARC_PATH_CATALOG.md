# NARC / NitroFS Path Catalog — Pokémon White 2

## Purpose

This document records publicly documented NitroFS/NARC paths for Pokémon White 2 under the project's no-local-ROM policy. B2W2 research that explicitly covers both paired sequels can establish a path/role lead, but Black 2 archive counts are not copied into White 2 without White 2-specific evidence.

The machine-readable companion is `../manifests/narc-paths.csv`.

## Evidence rule

- B2W2 General ROM Info and tools that explicitly support both sequels provide path-role evidence for White 2.
- Black 2 Raw DB counts are **not** White 2 counts.
- `Observed` remains unavailable unless the exact White 2 target build or extracted material is directly examined under `VERIFICATION.md`.
- Known legacy-tool conflicts remain recorded.

## Initial path catalog

| Path | Reported role | White 2 member count | Evidence | Notes |
| --- | --- | ---: | --- | --- |
| `/a/0/0/2` | Main/system text | TBD | Direct technical | PPRE maps White 2 main text here. |
| `/a/0/0/3` | Story text | TBD | Corroborated for B2W2 | PPRE and B2W2 General ROM Info. |
| `/a/0/0/8` | Map resources | TBD | Corroborated for B2W2 | B2W2 General ROM Info + independent ROM-content documentation. |
| `/a/0/1/1` | Battle backgrounds | TBD | Direct technical | B2W2 General ROM Info. |
| `/a/0/1/2` | ZoneData | TBD | Direct technical | B2W2 General ROM Info. |
| `/a/0/1/6` | Pokémon personal data | TBD | Corroborated for B2W2 | B2W2 General ROM Info + PPRE. |
| `/a/0/1/7` | Experience/growth table | TBD | Direct technical | PPRE shared B2W2 mapping. |
| `/a/0/1/8` | Level-up learnsets | TBD | Corroborated for B2W2 | B2W2 General ROM Info + PPRE. |
| `/a/0/1/9` | Evolution data | TBD | Corroborated for B2W2 | B2W2 General ROM Info + PPRE. |
| `/a/0/2/0` | Base-evolution / baby-Pokémon lookup (legacy PPRE terminology) | TBD | Direct technical | Exact semantic format still needs dedicated documentation. |
| `/a/0/2/1` | Move data | TBD | Corroborated for B2W2 | B2W2 General ROM Info + PPRE. |
| `/a/0/2/4` | Item data | TBD | Direct technical | PPRE shared Gen V mapping. |
| `/a/0/2/6` | Title-screen resources | TBD | Direct technical | B2W2 General ROM Info. |
| `/a/0/3/0` | Start-menu sprite/resources | TBD | Direct technical | B2W2 General ROM Info. |
| `/a/0/4/8` | Overworld sprites | TBD | Corroborated for B2W2 | Public B2W2 ROM-content documentation. |
| `/a/0/5/6` | In-game scripts | TBD | Corroborated for B2W2 | B2W2 General ROM Info + concrete B2W2 script research. |
| `/a/0/6/5` | Move animations | TBD | Direct technical | B2W2 General ROM Info. |
| `/a/0/7/1` | Animated trainer sprites (front / VS) | TBD | Direct technical | B2W2 General ROM Info. |
| `/a/0/7/2` | Animated trainer sprites (back / send-out) | TBD | Direct technical | B2W2 General ROM Info. |
| `/a/0/9/1` | Trainer metadata (`trdata`) | TBD | Corroborated | B2W2 General ROM Info, TrainerTyrant, and Triple-Battle-Converter. |
| `/a/0/9/2` | Trainer parties (`trpoke`) | TBD | Corroborated | B2W2 General ROM Info + TrainerTyrant. |
| `/a/1/0/6` | Battle-facility/PWT banlist container | TBD | Single-source technical analysis | Public Gen V facility/PWT research identifies this B2W2 path. |
| `/a/1/2/4` | Egg moves | TBD | Direct technical | B2W2 General ROM Info. |
| `/a/1/2/6` | Overworld/map-event data | TBD | Corroborated | B2W2 General ROM Info + independent hacking reports. |
| `/a/1/2/7` | Wild encounter tables | TBD | Corroborated | B2W2 General ROM Info + independent wild-editing research. |
| `/a/1/6/3` | In-game trades | TBD | Direct technical | B2W2 General ROM Info. |
| `/a/2/6/7` | Trainer mugshots | TBD | Direct technical | B2W2 General ROM Info. |
| `/a/2/7/3` | Hidden Grotto encounter table | TBD | Direct technical | B2W2 General ROM Info. |
| `/a/2/8/2` | Poké Mart data | TBD | Direct technical | B2W2 General ROM Info. |
| `/a/2/9/1` | PWT board trainer sprites | TBD | Direct technical | B2W2 General ROM Info. |
| `/a/2/9/6` | Pokédex in-game location data | TBD | Direct technical | B2W2 General ROM Info. |

## Why counts are `TBD`

Project Pokémon Raw DB currently exposes a Black 2 reference tree, not a White 2 tree. Even if the paired sequels are likely to share many archive shapes, the repository will not promote Black 2 member counts into White 2 facts without White 2-specific preservation or technical evidence.

## Confirmed BW → B2W2 path movement

| Subsystem | Black / White | Black 2 / White 2 |
| --- | --- | --- |
| In-game scripts | `/a/0/5/7` | `/a/0/5/6` |
| Trainer metadata | `/a/0/9/2` | `/a/0/9/1` |
| Trainer parties | `/a/0/9/3` | `/a/0/9/2` |
| Overworld/events | `/a/1/2/5` | `/a/1/2/6` |
| Wild encounters | `/a/1/2/6` | `/a/1/2/7` |

## Source conflict: legacy PPRE B2W2 mappings

Legacy PPRE `nds/files.py` incorrectly/stalely maps Black 2 trainer and encounter paths to the BW-style locations. Because the same codebase groups Black2/White2 mapping patterns, this repository treats its B2W2 trainer/encounter entries as conflicted evidence, not authority.

Later B2W2-specific sources consistently identify:

- `/a/0/9/1` — trainer metadata
- `/a/0/9/2` — trainer parties
- `/a/1/2/6` — overworld/event data
- `/a/1/2/7` — encounter tables

## Source anchors

- B2W2 General ROM Info: https://projectpokemon.org/home/forums/topic/22629-b2w2-general-rom-info/
- PPRE `nds/files.py`: https://github.com/projectpokemon/PPRE/blob/master/nds/files.py
- PPRE `pokeversion.py`: https://github.com/projectpokemon/PPRE/blob/master/pokeversion.py
- TrainerTyrant: https://github.com/ThirdLemon/TrainerTyrant
- Triple-Battle-Converter: https://github.com/mFireworks/Triple-Battle-Converter
- B2W2 script/starter research: https://projectpokemon.org/home/forums/topic/13490-twistedfatal-black-and-white-toolbox/page/15/
- ROM-content cross-reference: https://whackahack.com/foro/threads/guia-nds-informacion-sobre-el-contenido-de-cada-rom-proceso.32504/
- Project Pokémon Raw DB index (shows Black 2 but no White 2 tree): https://projectpokemon.org/rawdb/

## Next work

1. Find White 2-specific file-tree/archive census preservation data.
2. Identify region/revision coverage behind B2W2 tools and research posts.
3. Compare White 2 with Black 2 path-by-path rather than importing counts.
4. Split B2W2-specific systems into dedicated format/data documents as evidence accumulates.
5. Feed version-specific differences into `REGIONAL_SURVEY_MATRIX.md` and manifests.