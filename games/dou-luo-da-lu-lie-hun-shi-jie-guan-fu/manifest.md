---
type: Manifest
title: 斗罗大陆：猎魂世界(官服) 知识库 Manifest
description: 斗罗大陆：猎魂世界(官服) 游戏知识库 Bundle 结构与模块配置
game_id: dou-luo-da-lu-lie-hun-shi-jie-guan-fu
genre_tags: [MMORPG, 开放世界, 动作RPG, 3D写实, 斗罗IP]
language: zh-CN
timestamp: 2026-07-28T00:00:00Z
confidence: high
modules: [overview, core-loop, progression, monetization, economy, social-liveops, versions, live-events, market-position, risks-unknowns, sources]
systems: [session-combat, exploration, content-modes, matchmaking]
entities: [units]
unit_policy: representative
---

# 模块选择与架构说明

《斗罗大陆：猎魂世界》是由三七互娱（安徽三七/广州三七极梦）研发发行的 3D 写实大世界 MMORPG 手游（腾讯动画与阅文集团双授权）。

## 系统模块启用说明

1. **`systems/session-combat.md`**：游戏采用无锁定实时动作战斗系统，支持 4 武魂无缝轮切、闪避浮空与魂技奥义组合，因此启用战斗系统模块。
2. **`systems/exploration.md`**：游戏包含诺丁城、星斗大森林、天斗城、杀戮之都、七宝山脉等开放世界地图，支持宝箱搜集、奇遇、拟态与魂兽猎杀，因此启用大世界探索模块。
3. **`systems/content-modes.md`**：游戏包含猎魂悬赏、邪化兽王、深渊巨兽、演武·元素掌控、邪魇入侵等多丰富常驻与周常副本，因此启用多模式内容模块。
4. **`systems/matchmaking.md`**：游戏包含斗魂对决（跨服 PvP 赛季竞技）等竞技匹配系统，因此启用竞技匹配模块。

## 实体选择说明

采用 `representative`（代表性实体）策略，精选 10 位涵盖强攻、敏攻、控制、防御、辅助不同定位与热度核心的 SSR 代表性武魂/魂师进行深度建档，避免全量数据堆砌。
