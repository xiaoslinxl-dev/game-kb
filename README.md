# game-kb

Per-game competitive LLM wiki (OKF-style). One game = one directory. Git is the source of truth for history (no `log.md`).

## Layout

```text
games/
  _template/           # scaffold for a new game
  <game_id>/           # one OKF bundle root per game
    index.md
    overview.md
    core-loop.md
    combat.md
    progression.md
    monetization.md
    social-liveops.md
    market-position.md
    risks-unknowns.md
    sources.md
AGENTS.md              # how Antigravity should read a game wiki
```

## Consume (Antigravity)

Mount this repo into the sandbox, pass `game_id`, and follow `AGENTS.md`.

```text
repository: https://github.com/xiaoslinxl-dev/game-kb.git
target:     /workspace/game-kb
```

## Generate

Use the GameplayGraph `okf-poc` tooling (`run_generate.py`) with okf-skill to write `games/<game_id>/`, then commit + push here.
