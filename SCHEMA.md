# Game KB Schema（竞品 LLM-Wiki 文档定义）

一游戏一目录。Git 为变更权威源（无 `log.md`）。正文默认简体中文。

研究格式版本：`research_schema_version: 1`（manifest 声明；它研究记录格式，与 OKF 标准版本、游戏版本是三件事）。

## 结构

```text
games/<game_id>/
├── index.md
├── manifest.md              # 启用哪些模块 + research_schema_version
├── overview.md              # 核心
├── core-loop.md
├── progression.md
├── monetization.md
├── economy.md
├── social-liveops.md
├── market-position.md
├── risks-unknowns.md
├── sources.md               # 来源总索引（只放入口与概览）
├── sources/                 # 来源详情（research_schema_version: 1 起）
│   └── <source-id>.md       #   一份独立来源，按修订分章节（## r001 …），每章节含检查时间与编号证据
├── systems/                 # 按品类启用
│   ├── session-combat.md
│   ├── base-build.md
│   ├── territory-war.md
│   ├── matchmaking.md
│   ├── exploration.md
│   └── content-modes.md
├── versions.md              # 版本总索引
├── versions/                # 单版本清单（同版本跨地区/平台 = 不同清单）
│   └── <version-id>.md
├── revisions/               # 规则修订正文（topic 内编号，非游戏版本号）
│   └── <topic>/<revision-id>.md
├── live-events.md           # 活动实例台账
└── entities/                # 按需
    ├── index.md
    └── units/               # 角色/武将/英雄（representative 抽样）
        ├── _index.md
        └── <unit-slug>.md
```

事实写在所属模块；版本清单只做映射、修订保存规则历史、来源保存证据，用稳定 ID 关联，
不在多份文档维护同一事实。主题文件（systems/economy/…）是选定修订组装的当前视图。

## 最小字段契约（摘要）

逐类型字段表、模板与完整规则以生成侧契约为准：
GameplayGraph `backend/app/agents/llm_wiki/skills/game-mechanics-research/references/OUTPUT_SCHEMA.md`。

- 稳定 ID：`rule_id` / `resource_id` / `progression_id` / `relation_id` / `system_id` /
  `version_id` / `change_id` / `source_id` / `evidence_id` / `(topic_id, revision_id)`。
  定义唯一、引用可重复；改名不换 ID；`rule_id` 跨修订稳定。
- 来源引用：`source_id@source_revision/evidence_id`（如 `src-0001@r001/ev-01`），
  必须能在 `sources/<source-id>.md` 中回查。
- 核验状态：`confirmed` / `unverified` / `conflicted` / `deprecated`；商业效果推断标
  `statement_kind: inference`。文件级 `confidence` 仅为概览。
- 未知与不适用：必填项不得空白——`unknown（原因）` / `not_applicable（原因）`。
- 无活动/无资料是合法结果：保留空表 + not_found 记录 + `risks-unknowns.md` 缺口，不得编造。

## 默认策略

- `unit_policy: representative`（8–15 个关键实体，不做全图鉴）
- 生成 Agent 必须使用 `google_search` + `url_context`
- 校验：对该游戏目录跑 OKF `--strict --check-links` + liveops 表校验；
  逐类型领域校验（`validate_game_mechanics.py`）由后续阶段接入，届时新/已迁移 bundle 走严格发布校验。
- 旧格式 bundle（无 `research_schema_version`）仍可读取；审计报告列出迁移缺口，不阻塞阅读。
