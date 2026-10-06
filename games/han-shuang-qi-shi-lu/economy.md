---
type: Economy
title: 寒霜启示录 经济系统
description: 基础生产资源（肉/木/煤/铁）、高级货币（宝石/霜星）与特殊代币的双轨经济模型分析。
game_id: han-shuang-qi-shi-lu
confidence: high
timestamp: "2026-10-06T11:00:00Z"
research_schema_version: 1
applies_to: all
---

# 寒霜启示录 经济系统

《寒霜启示录》采用典型的双轨制（基础生产资源 + 高级充值货币）经济结构，配合多层级的活动代币商店与回收流转机制，实现资源自给与长线养成循环。

## 资源台账

| resource_id | 名称 | 产出系统 | 消耗用途 | 获取/存储限制 | 刷新周期 | 转换 | 有效期与跨期保留 | 来源 | 核验状态 |
|---|---|---|---|---|---|---|---|---|---|
| res-meat | 生肉 (Meat) | sys-base-build, sys-exploration | 建筑升级、暴风雪幸存者口粮、训练士兵 | 仓库保护容量受仓库等级限制 | 即时持续产出 | not_applicable（基础物资不可直转外币） | not_applicable（永久保留无过期限制） | src-0001@r001/ev-01 | unverified |
| res-wood | 木材 (Wood) | sys-base-build, sys-exploration | 建筑升级、科技研发、兵种训练 | 仓库保护容量受仓库等级限制 | 即时持续产出 | not_applicable（基础物资不可直转外币） | not_applicable（永久保留无过期限制） | src-0001@r001/ev-01 | unverified |
| res-coal | 煤炭 (Coal) | sys-base-build, sys-exploration | 大熔炉日常供暖、暴风雪过载升温、高级城建 | 仓库保护容量受仓库等级限制 | 即时持续产出 | not_applicable（基础物资不可直转外币） | not_applicable（永久保留无过期限制） | src-0001@r001/ev-01 | unverified |
| res-iron | 铁矿 (Iron) | sys-base-build, sys-exploration | 高阶兵种训练、火晶建筑前置、高等科技 | 仓库保护容量受仓库等级限制 | 即时持续产出 | not_applicable（基础物资不可直转外币） | not_applicable（永久保留无过期限制） | src-0001@r001/ev-01 | unverified |
| res-gems | 宝石 (Gems) | sys-content-modes, sys-territory-war | 幸运轮盘抽卡、VIP商店购买加速、应急资源补足 | not_applicable（无获取与存储上限） | 活动结算与每日任务刷新 | 可1:1抵扣多种日常代币缺口 | not_applicable（永久保留可跨赛季跨期使用） | src-0001@r001/ev-04 | unverified |
| res-frost-star | 霜星 (Frost Stars) | Web Store直充购买 | 网页商城购买游戏内同等价值礼包与周月卡 | not_applicable（充值代币无存储上限） | not_applicable（即时充值获得） | 1:1等额替代游戏内现金内购计费 | not_applicable（永久保留跨期不过期） | src-0009@r001/ev-01 | unverified |
| res-fire-crystal | 火晶 (Fire Crystals) | sys-content-modes, sys-territory-war | 大熔炉FC1-FC10突破、核心火晶建筑升级 | 每日获取受活动与礼包配额限制 | 每日00:00 UTC刷新 | 苔原贸易站溢出兑换 | not_applicable（永久保留随王国世代推进） | src-0001@r001/ev-01 | unverified |
| res-refined-fc | 精炼火晶 (Refined FC) | sys-content-modes, sys-base-build | 大熔炉高阶突破、战争学院炽炎科技研究 | 产出受限于地心探险层数与高难活动 | 每周/活动周期刷新 | 在精炼工坊由基础火晶合成 | not_applicable（永久保留不过期） | src-0001@r001/ev-01 | unverified |
| res-wish-mark | 心愿印记 (Wish Marks) | sys-base-build | 在心愿商店兑换9座娱乐设施专属建筑材料 | 每日居民心愿数量上限为固定配额 | 每日00:00 UTC刷新 | 心愿商店兑换专属建材 | not_applicable（火晶时代内永久保留） | src-0001@r002/ev-02 | confirmed |
| res-arena-coin | 竞技场代币 (Arena Coins) | sys-content-modes | 竞技场商店兑换特定SSR英雄碎片与专武材料 | 每日免费挑战5次，购买次数有每日上限 | 每日00:00 UTC刷新 | 商店定向兑换英雄碎片 | not_applicable（永久保留随赛季跨期） | src-0002@r001/ev-02 | unverified |
| res-stamina | 领主体力 (Stamina) | 自然恢复, 任务礼包 | 野外猎杀野兽、巨熊集结、情报任务 | 上限120点（可溢出存储通过药水获得） | 每5分钟恢复1点 | not_applicable（不可逆向转换代币） | 自然恢复部分满120即止，背包药水永久有效 | src-0007@r001/ev-01 | unverified |
| res-speedup | 通用加速 (Speedup) | sys-base-build, sys-content-modes | 建筑建造加速、科研加速、练兵与治疗加速 | not_applicable（背包无限堆叠存储） | not_applicable（即时消耗型资产） | 联盟帮助每次减少1%或固定分钟 | not_applicable（永久保留随时可使用） | src-0007@r001/ev-01 | unverified |

## 1. 基础生产资源（内城与采集）

游戏内有四大基础资源，用于建筑升级、士兵训练与科技研发：

| 资源类型 | 主要产出建筑 | 解锁与配比建议 | 消耗用途 |
| :--- | :--- | :--- | :--- |
| **生肉 (Meat)** | 猎人小屋 | 前期核心资源 | 建筑建设、暴风雪食物供给、爆兵 |
| **木材 (Wood)** | 伐木场 | 前期核心资源 | 建筑建设、科技研发、爆兵 |
| **煤矿 (Coal)** | 煤矿场 | 中期核心（熔炉供暖消耗） | 大熔炉过载与升温、高级建筑 |
| **铁矿 (Iron)** | 铁矿场 / 挂机探险 | 中后期核心 | 高级建筑、高阶兵种训练与科研 |

*注：玩家日常采集建议配比一般保持在 肉20 : 木20 : 煤4 : 铁1。在向苔原核心区搬迁时，各资源储备需求往往达到数十万乃至百万级。*

## 2. 高级货币系统

1. **宝石（Gems）**：
   - 游戏内核心高价值通用货币。
   - **获取途径**：充值、每日任务、探险关卡首通、联盟礼包、SVS/最强领主活动积分奖励（活跃玩家月均可积累数万宝石）。
   - **最优消费策略**：积攒宝石用于**幸运轮盘保底抽取世代核心英雄**，或在备战活动期间购买VIP经验与高价值加速，切忌直接用于普通基础资源购买。
2. **霜星（Frost Stars）**：
   - 官方网页商城（Century Games Store）与授权三方平台直充高级代币，具备比端内直接购买更优惠的费率（如额外返利与免税优惠），1:1 等价兑换游戏内礼包并激活运营累充活动。

## 3. 专属代币与多元循环体系

- **心愿印记 (Wish Marks)**：
  - 熔炉 FC1 后通过[心愿驿站](systems/base-build.md)完成幸存者诉求获得，用于兑换 9 大娱乐建筑专属建材（来源：[src-0001](sources/src-0001.md)，证据：r002/ev-02，状态：confirmed）。
- **雪原贸易站 (Tundra Trading Station)**：
  - 王国进程达到指定天数后解锁，领主可一键售出溢出的英雄碎片与专属装备零件，实现溢出资产向实用养成资源的平滑回收置换（来源：[src-0004](sources/src-0004.md)，证据：r004/ev-04，状态：confirmed）。
- **复苏之印 (Revitalization Seals)**：
  - 跨服最强王国（SvS）阶段战损阵亡士兵的复活代币，保障大战争损可控回收。
