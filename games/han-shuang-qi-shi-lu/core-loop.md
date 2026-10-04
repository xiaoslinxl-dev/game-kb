---
type: CoreLoop
title: 寒霜启示录 核心循环
description: 解析《寒霜启示录》从前期模拟经营到中后期4X大地图战争的双核循环机制，涵盖资源生产、大熔炉供暖、小队探险与跨服王战。
game_id: han-shuang-qi-shi-lu
confidence: high
timestamp: "2026-10-01T11:00:00Z"
research_schema_version: 1
applies_to: all
---

# 寒霜启示录 核心循环

《寒霜启示录》的核心循环由**内城模拟经营循环**与**外城 4X SLG 大地图扩张循环**双核驱动，并在中后期过渡为**联盟社交与跨服巅峰竞技循环**。

## 核心循环关系台账

| relation_id | 起点 ID | 关系类型 | 终点 ID | 条件 | 来源 | 核验状态 |
|---|---|---|---|---|---|---|
| rel-001 | sys-base-build | 产出 | res-meat | 建造并指派幸存者进驻猎人小屋 | src-0001@r001/ev-01 | unverified |
| rel-002 | sys-base-build | 产出 | res-coal | 建造并指派幸存者进驻煤矿场 | src-0001@r001/ev-01 | unverified |
| rel-003 | res-coal | 消耗 | prog-furnace | 开启大熔炉过载供暖及熔炉升温维护 | src-0001@r001/ev-01 | unverified |
| rel-004 | prog-furnace | 解锁 | prog-fc-age | 大熔炉达到Lv 30且满足王国开服天数 | src-0001@r001/ev-01 | unverified |
| rel-005 | prog-fc-age | 解锁 | res-wish-mark | 熔炉达到FC1开启心愿驿站完成居民心愿 | src-0001@r001/ev-01 | unverified |
| rel-006 | res-wish-mark | 转换 | prog-chief-gear | 在心愿商店兑换娱乐设施建材，设施产出装备图纸与材料 | src-0001@r001/ev-01 | unverified |
| rel-007 | sys-exploration | 产出 | res-iron | 5人小队推关与挂机探险宝箱 | src-0002@r001/ev-01 | unverified |
| rel-008 | res-iron | 消耗 | prog-troop-tier | 兵营训练与升级士兵（T1-T10） | src-0001@r001/ev-01 | unverified |
| rel-009 | sys-content-modes | 产出 | res-arena-coin | 参与每日竞技场挑战防守镜像 | src-0002@r001/ev-02 | unverified |
| rel-010 | res-arena-coin | 转换 | prog-hero-star | 在竞技场商店兑换特定英雄碎片提升星级 | src-0002@r001/ev-02 | unverified |
| rel-011 | res-fire-crystal | 强化 | prog-troop-t12 | 熔炉FC8后在炽炎科技所进阶T12煌耀兵种 | src-0002@r001/ev-03 | unverified |
| rel-012 | prog-troop-t12 | 强化 | sys-territory-war | 提升太阳城王战争夺与SvS跨服集结战斗力 | src-0002@r001/ev-03 | unverified |
| rel-013 | sys-territory-war | 产出 | res-gems | 赢得堡垒要塞争夺战与最强王国跨服战排名奖励 | src-0005@r001/ev-02 | unverified |
| rel-014 | res-gems | 消耗 | prog-hero-star | 幸运大转盘消耗宝石抽取世代核心英雄碎片 | src-0001@r001/ev-04 | unverified |

## 1. 基础内城模拟经营循环

1. **资源收集**：通过猎人小屋（生肉）、伐木场（木材）、煤矿场（煤炭）、铁矿场（铁矿）获取基础四大资源。
2. **大熔炉与设施升级**：消耗资源升级核心**大熔炉**（Furnace），提升定居点抗寒温度，同时解锁更高的民宅与兵营等级。
3. **幸存者生存维护**：在暴风雪（Blizzard）或夜晚阶段启动大熔炉“过载”增温，维持幸存者满意度与健康值，防止幸存者生病停工。
4. **火晶心愿与日常产出**：熔炉突破 30 级后进入火晶时代，通过[心愿驿站](systems/base-build.md)完成幸存者心愿换取印记，建造 9 大娱乐设施持续产出高级养成材料。

## 2. 探索、日常聚合与英雄养成循环

1. **“日常”总览一站式驱动**：通过主界面“日常（Daily Tab）”整合入口，统一清空竞技场、苔原历险（Treks）、迷宫（Labyrinth）、灯塔情报与英雄免费招募进度。
2. **挂机探险（Exploration）**：通过5人小队推关，解锁离线挂机收益（主要产出铁矿、英雄经验与装备材料）。
3. **英雄招募与星级突破**：在英雄大厅（Hero Hall）与世代轮盘进行招募，通过碎片提升英雄星级、解锁专属武器技能，反哺SLG行军集结与小队战力。

## 3. 大地图 SLG 与联盟扩张循环

1. **野外资源采集与野兽猎杀**：派遣军队采集地图大矿，猎杀冰原野兽与冰原巨兽（Bear / Beast），获得领主装备材料与宝石。
2. **联盟集结与领地建造**：加入活跃联盟，建造联盟旗帜与工程站，瓜分要塞（Fortress）与枢纽设施。
3. **王城争霸、跨服对抗与巅峰战**：参与日光城（Sunfire Castle）争夺战、跨服最强王国（State vs State）、[霜龙霸主](systems/territory-war.md)多王国巅峰对决与[冰火战歌联赛](systems/content-modes.md)，争夺执政官特权、霸主王座与全服排名奖励。

相关文档链接：
- [游戏概览](overview.md)
- [数值与长线养成](progression.md)
- [基地建造与模拟经营](systems/base-build.md)
- [战斗系统与小队/SLG机制](systems/session-combat.md)
