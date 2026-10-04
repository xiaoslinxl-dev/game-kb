---
type: Monetization
title: 寒霜启示录 商业化设计
description: 极高ARPU的4X SLG商业化策略，涵盖永久功能礼包、VIP特权、幸运轮盘、火晶礼包与世代英雄抽卡。
game_id: han-shuang-qi-shi-lu
confidence: high
timestamp: "2026-10-04T11:00:00Z"
research_schema_version: 1
applies_to: all
---

# 寒霜启示录 商业化设计

《寒霜启示录》实现了极高的商业化变现效率，其商业化结构既保留了传统 4X SLG 的大氪高 ARPU 池，又通过高性价比的基建礼包大幅提升了首充与中氪转化率。

## 商业化产品与权益台账

| product_id | 产品/权益 | 价格与币种 | 地区/平台 | 适用条件 | 来源 | 核验状态 |
|---|---|---|---|---|---|---|
| prod-sprint-pack | 新手冲刺礼包 (永久第二建造队列+初始资源) | 4.99 USD | US / iOS & Android | 账号创建前7天内限购1次 | src-0001@r001/ev-01 | unverified |
| prod-march-queue | 第二行军队列礼包 (永久增加大地图行军队伍) | 9.99 USD | US / iOS & Android | 大熔炉Lv 7以上常驻限购1次 | src-0001@r001/ev-01 | unverified |
| prod-first-recharge | 首充礼包 (SSR步兵英雄娜塔莉亚+专属武器) | 0.99 USD | US / iOS & Android | 首次任意金额现金内购 | src-0001@r001/ev-01 | unverified |
| prod-monthly-pass | 极地月卡 (每日领取1,000钻石+体力药水+行军增益) | 9.99 USD | US / iOS & Android | 常驻可续期购买，有效期30天 | src-0001@r001/ev-01 | unverified |
| prod-weekly-pass | 至尊周卡 (每日高额通用加速+基础建材) | 4.99 USD | US / iOS & Android | 常驻可按周循环购买，有效期7天 | src-0001@r001/ev-01 | unverified |
| prod-survivor-pass | 幸存者通行证 (Battle Pass 赛季高级战令) | 19.99 USD | US / iOS & Android | 赛季战令开放期间（每期约28天） | src-0001@r001/ev-01 | unverified |
| prod-lucky-wheel | 幸运轮盘代币礼包 (世代SSR英雄碎片与专武原石) | 4.99 ~ 99.99 USD | US / iOS & Android | 当期世代轮盘活动开放期间 | src-0001@r001/ev-04 | unverified |
| prod-fire-crystal | 火晶强化专属礼包 (火晶+精炼火晶+加速) | 4.99 ~ 99.99 USD | US / iOS & Android | 大熔炉达到Lv 30火晶时代开启后 | src-0001@r001/ev-01 | unverified |
| prod-chief-gear | 领主装备图纸与抛光液礼包 (高阶装备图纸) | 19.99 ~ 99.99 USD | US / iOS & Android | 王国进入Gen 6以上解锁传奇T6前置 | src-0003@r001/ev-01 | unverified |
| prod-12h-barrier | 12小时领地防护罩 (免受敌方侦察与攻击掠夺) | 500 钻石 或 0.99 USD | US / iOS & Android | 全阶段常驻（城市增益与联盟商店） | src-0001@r001/ev-03 | unverified |

## 1. 入门与必买核心礼包（低门槛变现）

1. **新手冲刺礼包（Beginner Sprint Pack / 原建造队列礼包升级）**：
   - 永久解锁第二个建造队列（500 霜星/钻石档位），并附赠大量初始发展资源与加速。由于建筑升级时间随等级指数增长，该礼包为付费玩家的核心必买项。
2. **第二行军队列礼包（Marching Queue Pack）**：
   - 永久增加一个大地图行军队列，极大地提升野外采集与打怪清情报效率。
3. **首充礼包与 VIP 礼包**：
   - 首充任意金额送 SSR 步兵英雄[娜塔莉亚](entities/units/natalia.md)。
   - 购买专属 VIP 礼包获得核心 SSR 步兵英雄[杰罗尼莫](entities/units/jeronimo.md)。

## 2. 订阅与常驻收益（中氪留存）

- **月卡与至尊周卡 (Monthly & Weekly Passes)**：
  - 每日提供稳定宝石（Gems）、领主体力药水与通用加速道具，两周内即可完全收回基础投入价值。
- **幸存者通行证 (Battle Pass / Survivor Pass)**：
  - 结合每期赛季主题（如极地狂欢、凛冬庆典）的活跃战令，解锁专属行军皮肤、铭牌与高阶通用橙色碎片。
- **平民防护兜底设计**：
  - 在城市增益与联盟商店全面引入【12小时防护罩】，为非全天在线的中小氪与平民领主提供高性价比战力保全手段。

## 3. 核心抽卡与大额付费点（长线高ARPU）

1. **幸运大转盘 (Lucky Wheel)**：
   - 游戏内性价比最高的世代英雄获取途径。每代新英雄轮盘上线时，中大氪玩家通过消耗钻石或购买轮盘币直接将当期核心英雄（如[弗林特](entities/units/flint.md)、[米娅](entities/units/mia.md)、[艾登](entities/units/aiden.md)）拉满星级。
2. **火晶礼包与精炼火晶 (Fire Crystals)**：
   - 熔炉 Lv 30 之后的核心付费卡点。火晶用于 FC1 至 FC10 大熔炉与核心建筑突破，属于跨服战车头玩家的硬性数值门槛。
3. **领主装备、宝符与晨曦学堂专家**：
   - 传奇 T6 装备图纸、抛光液与 17-18 级宝符设计图属于顶氪长线池。VIP 商店已下调部分兑换门槛并增补抛光液与图纸兑换。

## 4. 商业化效果与留存表现推论

<!-- statement_kind: inference -->
根据 Sensor Tower 与 AppMagic 的历史收入走势研判，《寒霜启示录》通过前期 0.99 美元首充、4.99 美元二建队列以及 9.99 美元月卡构筑了极宽的泛用户付费转化漏斗，使得早期转化率明显高于同类重度 4X SLG。随着服务器进入火晶时代与跨服最强王国阶段，中长线付费向高 ARPU 的火晶礼包、轮盘抽卡与领主装备集中，形成长尾收入极其稳定的高变现模型。
