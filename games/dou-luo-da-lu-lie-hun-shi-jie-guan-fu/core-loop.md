---
type: CoreLoop
title: 斗罗大陆：猎魂世界(官服) 核心循环
description: 游戏的核心玩法循环、日常/周常玩法路径与战力成长反馈（research_schema_version: 1）
game_id: dou-luo-da-lu-lie-hun-shi-jie-guan-fu
confidence: high
timestamp: "2026-10-01T20:45:00Z"
applies_to: all
research_schema_version: 1
---

# 斗罗大陆：猎魂世界(官服) 核心循环

《斗罗大陆：猎魂世界》的核心循环建立在“开放世界探索/副本挑战 → 资源获取（魂环/魂核/觉醒券/材料） → 武魂抽卡与魂环/魂核/魂骨养成 → 战力提升 → 挑战高阶副本/跨服 PvP”的经典 MMORPG + Gacha 循环链上。

---

## 核心循环流转关系表

| relation_id | 起点 ID | 关系类型 | 终点 ID | 条件 | 来源 | 核验状态 |
|---|---|---|---|---|---|---|
| rel-001 | sys-exploration | 产出 | res-diamond | 大世界开宝箱、达成区域探索度与成就 | src-0002@r001/ev-03 | confirmed |
| rel-002 | sys-exploration | 产出 | res-xiancao | 野外仙草采集与奇遇任务奖励 | src-0002@r001/ev-03 | confirmed |
| rel-003 | res-diamond | 消耗 | res-wuhun-ticket | 以160钻石:1张比例兑换限定觉醒券 | src-0001@r001/ev-01 | confirmed |
| rel-004 | res-diamond | 消耗 | res-stamina | 每日限次购买体力用于副本推进 | src-0005@r001/ev-01 | confirmed |
| rel-005 | res-stamina | 消耗 | sys-content-modes | 消耗体力进行拟态训练与猎魂魂兽 | src-0005@r001/ev-01 | confirmed |
| rel-006 | sys-content-modes | 产出 | res-gold | 拟态关卡通关与日常副本结算 | src-0005@r001/ev-01 | confirmed |
| rel-007 | sys-content-modes | 产出 | prog-hunhuan-slot | 猎杀魂兽掉落各年份专属魂环 | src-0005@r001/ev-01 | confirmed |
| rel-008 | res-wuhun-ticket | 消耗 | prog-wuhun-star | 限定卡池抽取获得武魂本体与碎片觉醒升星 | src-0001@r001/ev-01 | confirmed |
| rel-009 | res-wuhun-ticket | 转换 | res-xingshen-yu | 限定卡池每抽附赠随机数量星神玉代币 | src-0001@r001/ev-01 | confirmed |
| rel-010 | res-xingshen-yu | 消耗 | prog-hunhe-center | 星神玉商店兑换专属魂技/奥义与十万年灵核 | src-0001@r001/ev-01 | confirmed |
| rel-011 | prog-wuhun-star | 强化 | sys-session-combat | 提升武魂四维面板、解锁新机制与登场技 | src-0002@r001/ev-03 | confirmed |
| rel-012 | prog-waifu-hungu | 强化 | sys-session-combat | 外附魂骨三维年份星级提供全时段全局免伤与属性 | src-0005@r001/ev-01 | confirmed |
| rel-013 | sys-session-combat | 解锁 | sys-matchmaking | 战力达标进入斗魂对决跨服天梯排位 | src-0001@r001/ev-05 | confirmed |
| rel-014 | sys-matchmaking | 产出 | res-honor-coin | 斗魂对决获胜、段位晋阶与赛季结算 | src-0001@r001/ev-05 | confirmed |
| rel-015 | sys-content-modes | 产出 | res-yuanzheng-coin | 远征计划单队通关与双队讨伐伤害排行结算 | src-0005@r001/ev-02 | confirmed |
| rel-016 | res-yuanzheng-coin | 消耗 | prog-waifu-hungu | 远征商店兑换骨华凝晶用于外附魂骨升星 | src-0005@r001/ev-02 | confirmed |
| rel-017 | sys-content-modes | 产出 | res-moon-coins | 参与秋宵同欢双节日常与谲影牌对战 | src-0004@r001/ev-01 | confirmed |
| rel-018 | res-moon-coins | 转换 | res-play-value | 参与斗罗谲影牌4人博弈赢取名次与玩心值 | src-0001@r001/ev-02 | confirmed |
