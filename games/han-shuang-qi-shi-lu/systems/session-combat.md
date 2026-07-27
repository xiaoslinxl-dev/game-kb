---
type: SessionCombat
title: 战斗系统与小队/SLG机制 (Session Combat)
description: 解析小队RPG 5v5战斗（探险/竞技场）与4X大地图SLG行军集结双重战斗机制及兵种克制。
game_id: han-shuang-qi-shi-lu
confidence: high
---

# 战斗系统与小队/SLG机制 (Session Combat)

《寒霜启示录》具备两套完全不同的战斗展现与结算逻辑：**小队RPG战斗**与**4X SLG大地图战斗**。

## 1. 小队RPG战斗（探险 / 竞技场）

- **阵型规则**：采用5人九宫格阵型（通常前排2人，后排3人）。
  - **前排**：推荐放置盾兵/步兵英雄（如[杰罗尼莫](/entities/units/jeronimo.md)、[娜塔莉亚](/entities/units/natalia.md)、[弗林特](/entities/units/flint.md)），吸收伤害并提供控制。
  - **后排**：放置射手/枪兵与辅助英雄（如[茉莉](/entities/units/molly.md)、[巴林](/entities/units/bahiti.md)、[菲利](/entities/units/philly.md)），进行主输出与治疗。
- **技能释放与怒气/能量**：英雄普通攻击与受击积累能量，满能量后释放大招（探索技能）。大招具备范围伤害、眩晕、冰冻、治疗或破甲效果。

## 2. 4X SLG大地图战斗（采集/打怪/城战/集结）

- **部队构成**：由1-3名指挥官（英雄）带领三大兵种（步兵、枪兵、弓兵）组成行军队列。
- **兵种克制公式**：
  - **步兵（Infantry）**：高防御/高生命，克制枪兵（+10%伤害）。
  - **枪兵（Lancer）**：高穿透/中等攻防，克制弓兵（+10%伤害）。
  - **弓兵（Marksman）**：高爆发/高暴击，克制步兵（+10%伤害）。
- **远征技能（Expedition Skills）**：在SLG战斗中，英雄不释放小队大招，而是触发其“远征技能”，为随行部队提供全局百分比攻击、防御、减伤或集结伤害加成（如[西里尔](/entities/units/cyril.md)的打熊集结加成）。
- **战损结算**：分为轻伤、重伤（进入军医所 Clinic 治疗）与死亡（超出军医所容量部分）。

相关文档链接：
- [数值与长线养成](/progression.md)
- [内容模式与玩法大纲](/systems/content-modes.md)
- [英雄/单位大纲](/entities/units/_index.md)
