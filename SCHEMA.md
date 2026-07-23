# Game KB Schema（竞品 LLM-Wiki 文档定义）

一游戏一目录。Git 为变更权威源（无 `log.md`）。正文默认简体中文。

## 三层结构

```text
games/<game_id>/
├── index.md
├── manifest.md              # 启用哪些模块
├── overview.md              # 核心
├── core-loop.md
├── progression.md
├── monetization.md
├── economy.md
├── social-liveops.md
├── market-position.md
├── risks-unknowns.md
├── sources.md
├── systems/                 # 按品类启用
│   ├── session-combat.md
│   ├── base-build.md
│   ├── territory-war.md
│   ├── matchmaking.md
│   ├── exploration.md
│   └── content-modes.md
└── entities/                # 按需
    ├── index.md
    └── units/               # 角色/武将/英雄（representative 抽样）
        ├── _index.md
        └── <unit-slug>.md
```

## 默认策略

- `unit_policy: representative`（8–15 个关键实体，不做全图鉴）
- 生成 Agent 必须使用 `google_search` + `url_context`
- 校验：对该游戏目录跑 OKF `--strict --check-links`
