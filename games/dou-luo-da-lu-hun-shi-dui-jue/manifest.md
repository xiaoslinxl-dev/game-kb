---
type: Manifest
title: 斗罗大陆：魂师对决 模块清单
description: 《斗罗大陆：魂师对决》知识库结构配置与模块规划
game_id: dou-luo-da-lu-hun-shi-dui-jue
genre_tags:
  - turn-based-rpg
  - card-battle
  - ip-adaptation
language: zh-CN
timestamp: 2026-08-03T00:00:00Z
confidence: high
modules:
  - core: [overview, core-loop, progression, monetization, economy, social-liveops, versions, live-events, market-position, risks-unknowns, sources]
  - systems: [session-combat, content-modes]
  - entities: [units]
unit_policy: representative
---

# 模块启用说明

- **核心模块 (Core)**：全部 11 个核心文件均已建立，全面涵盖游戏概貌、核心循环、长线养成、商业化、代币经济、运营策略、版本时间线、活动台账、市场定位、风险与来源。
- **系统模块 (Systems)**：
  - `session-combat.md`：游戏核心战斗为 6v6 回合制卡牌战斗，包含行动条、魂力管理、阵营/职业羁绊与武魂融合技。
  - `content-modes.md`：游戏包含 PVE 主线/猎魂森林、PVP 斗魂场/全民对决、GvG 宗门争霸以及跨服星斗大森林等丰富玩法。
- **实体模块 (Entities)**：
  - `entities/units/`：收录 10 位代表性核心魂师（如 SP+ 太初食神·奥斯卡、SP+ 月神·小舞、SP+ 极致剑道·尘心、SP 修罗·唐三等），体现版本 Meta 与商业化锚点。
