# Contributing

Languages: [繁體中文](../CONTRIBUTING.md) · [English](CONTRIBUTING.en.md)

This repository is an archived 2023 coursework showcase. Documentation fixes and notes on opening the project on JDK 8 in 2026 are welcome. Treat the game as an artefact first.

## Before you start

1. Read [`../README.md`](../README.md) and [`README.md`](README.md).
2. Rule or parameter changes must land in [`gameplay.md`](gameplay.md) and the matching Java together.
3. When they disagree: **2023 submitted behaviour wins**. Fix the docs. Gameplay edits are allowed only when the original sources do not compile or start, and the drift must be recorded under [`docs/`](./).

## Conventions

| Item | Rule |
| --- | --- |
| Public copy | Traditional Chinese in `README.md`; English in `docs/README.en.md` — edit both |
| Dates | `YYYY-MM-DD`, Taipei |
| Changelog | `## [Unreleased]` in `CHANGELOG.md` (Keep a Changelog 2.0.0) |
| Line endings | LF (`.gitattributes`) |

## Please do not

- Commit `local/`, `*.docx`, student numbers, `build/`, `dist/`, `nbproject/private/`, `jfx-impl_backup*`, or the unused GIF
- Hard-code absolute machine paths, accounts or student identifiers
- Describe this as an official Shimen Reservoir model or a Water Resources Agency product
- Rewrite the tree as Maven / JDK 21 and present it as the 2023 hand-in
- Replace the drawings with official reservoir photographs or agency marks

Ask first before irreversible git history changes.

## After a change

1. Note it under `## [Unreleased]` in `CHANGELOG.md`
2. Keep the two README tours in step if you touch the hero, install steps or tree
3. If `src/` behaviour changes, record the drift from the submitted files in [`gameplay.md`](gameplay.md)
