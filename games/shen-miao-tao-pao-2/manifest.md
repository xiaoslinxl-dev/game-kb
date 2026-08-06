---
type: Manifest
title: 神庙逃亡2 知识库 Manifest
description: 神庙逃亡2（Temple Run 2 中文版）知识库 Bundle 的模块规划与构成说明。
game_id: shen-miao-tao-pao-2
genre_tags:
- endless-runner
- casual
- pvp-runner
- action
language: zh-CN
timestamp: '2026-08-06T11:00:00Z'
confidence: high
modules_core:
- overview
- core-loop
- progression
- monetization
- economy
- social-liveops
- market-position
- risks-unknowns
- sources
modules_systems:
- session-combat
- content-modes
modules_entities:
- units
unit_policy: representative
---


# 模块选择说明

《神庙逃亡2》（Temple Run 2 中文版）由 Imangi Studios 开发、创梦天地（乐逗游戏）在中国大陆本土化代理与二次开发运营。作为一款经典的 3D 悬崖跑酷手游，其中国版本加入了大量的本土化系统、多套主题赛道与长线运营机制。

## 启用模块说明

- **Core (核心模块)**：全量包含 Overview、Core Loop、Progression、Monetization、Economy、Social/LiveOps、Market Position、Risks/Unknowns 和 Sources。
- **Systems (系统模块)**：
  - `session-combat`：涵盖单局跑酷、障碍避让、重力感应/滑屏操作、道具拾取以及 2v2 竞技场对战干扰/技能对抗机制。
  - `content-modes`：涵盖无尽跑酷模式、竞技场/排位赛（单人/双人）、主题地图副本（如玩具王国、幽灵穹顶、迷失丛林等）、黄金矿山挂机及限时收集赛等多重玩法。
- **Entities (实体模块)**：采用 `representative`（代表性实体）策略，挑选了 10 个具有代表性的角色、坐骑、宠物与羽翼/装备（如盖伊、莉莉丝、赵云、比奥斯博士、安妮、年兽、傲狠、仙灵鹤、小香猪、花蝶梦翅膀），覆盖新手引导、版本付费锚点、竞技 PvP Meta 与长线福利展示。
