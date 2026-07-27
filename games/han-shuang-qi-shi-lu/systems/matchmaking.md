---
type: Matchmaking
title: 匹配与跨服机制 (Matchmaking & Transfer)
description: 竞技场积分匹配、燃霜矿区跨服分组、王国移民（State Transfer）与SvS跨服对决匹配算法。
game_id: han-shuang-qi-shi-lu
confidence: high
---

# 匹配与跨服机制 (Matchmaking & Transfer)

为了保持服务器活力与跨服竞技的公平性，《寒霜启示录》建立了多层级的匹配与王国迁移规则。

## 1. 竞技场（Arena）匹配

- 基于玩家当前的**积分段位（Rank/Rating）**进行异步匹配。
- 刷新列表展示3位战力相近或稍高/稍低的对手。胜者提升积分，降者扣分。

## 2. 跨服战（SvS）匹配算法

- **历史战力与活跃度评估**：系统在SvS开启前，根据两个王国的顶级战力总和（Top 100领主战力）、历史胜率以及充值活跃度进行匹配。
- **开服天数相近**：通常匹配开服时间在同一区间（同一个Generation世代）的服务器，避免老服对新服的绝对数值碾压。

## 3. 燃霜矿区与活动跨服分组

- 跨服活动（如燃霜矿区、兵工厂争夺战）会将若干邻近战区/王国划入同一个匹配池，再根据联盟战力或个人战力分档（Tier），确保各梯队玩家都能获得相对公平的竞技体验。

## 4. 王国移民系统（State Transfer）

- 当服务器运营到一定阶段后开启移民。
- **移民规则**：
  - 玩家需要消耗**移民卷轴（State Transfer Pass）**，数量取决于玩家战力排名。
  - 目标王国设有最高战力上限与人数配额（普通领主与顶尖领主配额分开），防止单一服务器战力极度失衡。

相关文档链接：
- [内容模式与玩法大纲](/systems/content-modes.md)
- [社交与LiveOps运营](/social-liveops.md)
- [风险与未知项](/risks-unknowns.md)
