# Game KB — Consume Protocol

You are reading a **per-game** competitive LLM wiki. Git history is the changelog; there is **no** `log.md`.

## Paths

- Repo root in sandbox: `/workspace/game-kb`
- Current game root: `/workspace/game-kb/games/<game_id>/`
- `game_id` is provided in the user task. If missing, ask once; do not guess.

## Read protocol (mandatory)

1. Only read `/workspace/game-kb/games/<game_id>/`. Never open other `games/*` directories.
2. Start with `index.md`, then `overview.md`.
3. Open other files by question type:
   - session / retention / daily loop → `core-loop.md`
   - combat / match / PvP rules → `systems/session-combat.md`（旧 bundle 的根级 `combat.md` 仍可读，迁移前兼容）
   - resources / currencies / sinks → `economy.md`
   - power / resin / levels → `progression.md`
   - IAP / gacha / pass → `monetization.md`
   - guild / evergreen social ops → `social-liveops.md`
   - events (dated instances) → `live-events.md`
   - version timeline / per-version change lists → `versions.md` 与 `versions/<version-id>.md`；规则历史 → `revisions/<topic>/`
   - positioning / competitor narrative → `market-position.md`
   - uncertainty / open gaps → `risks-unknowns.md`
   - citations → `sources.md` 与 `sources/<source-id>.md`（证据编号 evidence_id）
4. Prefer progressive disclosure: index → overview → 1–3 relevant files. Do not dump the whole game folder.
5. When answering, cite file paths and respect `confidence` in frontmatter. Mark `low` confidence clearly.
6. Do not invent store rankings, revenue, or private metrics. If unknown, say so and point to `risks-unknowns.md` / `sources.md`.

## Write protocol

This consume profile is **read-only** unless the user explicitly asks to update the wiki. Updates belong to the generate pipeline.
