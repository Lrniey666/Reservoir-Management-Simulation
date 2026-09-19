# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

## [Unreleased]

### Added

- GitHub showcase tree: bilingual README (zh-Hant / en), gameplay and installation notes, MIT licence, contributing guide, and 2023 in-game screenshots under `docs/assets/`.
- `.gitignore` for the marked course report, `local/`, `build/`, `dist/`, `nbproject/private/`, `jfx-impl` backups, and the unused GIF.

### Changed

- Unused `ImpureDimwittedCottonmouth-max-1mb.gif` and the 2023 Word report moved to `local/` (still on disk, not in the public tree).
- README demo images are 2023 in-game screenshots taken from the course report (no student number in the public filenames). The previous hero SVG and loose art plates under `docs/assets/` are gone.
- Gameplay source is unchanged from the 2023 hand-in.

### Removed

- Build products, WebStart bundles, NetBeans private paths and `jfx-impl` auto-update backups are gitignored. They may still exist locally after a NetBeans open.

## [1.0.0] - 2023-04-13

### Added

- Coursework hand-in: JavaFX control-room game 「水庫模擬器Beta」.
- Day-step loop for supply, generation, gates, flood alarm and artificial rain.
- `Rock_Door_reservoir` parameter bands sized against public Shimen Reservoir figures.
- Hand-drawn weather, pool, console and monitor plates.
