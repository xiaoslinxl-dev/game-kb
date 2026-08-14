---
type: Manifest
title: 斗罗大陆：魂师对决 模块清单
description: 《斗罗大陆：魂师对决》知识库结构配置与模块规划
game_id: dou-luo-da-lu-hun-shi-dui-jue
genre_tags: [turn-based-rpg, card-battle, ip-adaptation]
language: zh-CN
timestamp: 2026-08-14T11:00:00Z
confidence: high
unit_policy: representative
modules: [core, systems, entities]
---

# 模块启用说明

- **核心模块 (Core)**：全部 11 个核心文件均已建立，全面涵盖游戏概貌、核心循环、长线养成、商业化、代币经济、运营策略、版本时间线、活动台账、市场定位、风险与来源。
- **系统模块 (Systems)**：
  - `session-combat.md`：游戏核心战斗为 6v6 回合制卡牌战斗，包含行动条、魂力管理、阵营/职业羁绊、武魂融合技以及第 7 人神祇机制。
  - `content-modes.md`：游戏包含 PVE 主线/猎魂森林、PVP 斗魂场/全民对决、GvG 宗门争霸以及跨服百级成神（登神长阶/神殿之争）等丰富玩法。
- **实体模块 (Entities)**：
  - `entities/units/`：收录 11 位代表性核心魂师（如双神·唐三、SP+ 月神·小舞、SP+ 太初食神·奥斯卡、SP+ 极致剑道·尘心、SP 修罗·唐三等），体现版本 Meta 与商业化锚点。
