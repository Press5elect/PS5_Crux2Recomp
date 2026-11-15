# PS5_Crux2Recomp

Crux2 Recomp's files that Crux2 (https://github.com/Press5elect/Crux2) builds with: its recomp kit
(`ps5/tools/make-recomp-kit.sh`, released with every Crux2 version) and its paraLLEl-GS renderer
(`ps5/tools/build-parallel-gs.sh`) take them from a checkout of this repository beside Crux2's
(`../PS5_Crux2Recomp`, or the folder `CRUX2_RECOMP_DIR` names).

| Path | What |
| --- | --- |
| `ps5/runner/crux2_recomp_config.h` | The settings PS2Recomp's runtime and every game module are compiled with |
| `ps5/runner/tools/build-runner-module.py` | Builds a game's `.crux2recomp` module from PS2Recomp's output, for the console |
| `ps5/runner/tools/vu1_recomp.py` | The VU1 recompiler: a game's VU1 microprograms to C++ (from def-jam-vendetta-recomp, jcsix694, GPL-3.0) |
| `ps5/patches/ps2recomp/` | PS2Recomp's runtime: def-jam-vendetta-recomp's work and Crux2 Recomp's changes (`runner.patch`), on PS2Recomp `e563698` |
| `ps5/patches/parallel-gs/` | paraLLEl-GS: def-jam-vendetta-recomp's changes and the PS5 build |
| `ps5/tools/fetch-ps2recomp.sh`, `fetch-parallel-gs.sh` | Fetch PS2Recomp and paraLLEl-GS (with Granite and volk) at their pins into `vendor/` and apply the patches |

The three runner files are as in recomp kit v1.6.4; the patches and fetch scripts as in Crux2's
`crux2recomp/` (2026-11-15). The Crux2 Recomp title's own source (its PS5 host) is not in this
repository yet.

Copyright (C) 2026 Press5elect, GPL-3.0-or-later (`LICENSE`), under the licences of the files the
patches change, with the additional term in `NOTICE`: keep the credit "Crux2 by Press5elect".
