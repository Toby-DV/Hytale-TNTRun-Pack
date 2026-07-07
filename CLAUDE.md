# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## About this project

This is a for-fun hobby project, not production/commercial work — favor clarity and learning over speed or polish.

The user is not very proficient with Java and wants to understand what the code being written actually does. Even though this pack is JSON content rather than Java, the same approach applies here:

- Go slowly — prefer smaller, incremental changes over large sweeping ones so each step is easy to follow.
- Explain what a change does and why, in plain language, alongside the change (not just a terse diff).
- Favor straightforward, readable structure over clever/dense patterns when both are reasonable options.

## Reference: hytale-shared-source

This project is a sibling of `../hytale-shared-source/` in the wider workspace, the official "Hytale Shared Source" repo. Its `HytaleAssets/Schema/` folder has the JSON Schema for every asset type (e.g. `Item.json`, `Interaction.json`, `RootInteraction.json`, `NPCRole.json`, `ProjectileConfig.json`), and `HytaleAssets/Server/` has the base game's own real instances of those assets. When unsure what fields an asset type supports or how the base game structures similar content, check there rather than guessing.

**Never copy files from `hytale-shared-source` into this repo, and never commit it here.** It's licensed reference material only — this repo is public, and `hytale-shared-source` is not ours to redistribute. `.gitignore` already excludes a `hytale-shared-source/` folder defensively in case one ever ends up nested inside this repo.
