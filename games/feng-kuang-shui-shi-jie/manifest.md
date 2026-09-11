---
type: Manifest
title: 疯狂水世界 知识库 Manifest
description: 疯狂水世界（feng-kuang-shui-shi-jie）知识库 Bundle 的模块规划与构成说明。
game_id: feng-kuang-shui-shi-jie
genre_tags: [survival, simulation, slg, nautical, card-rpg]
language: zh-CN
timestamp: "2026-09-11T11:00:00Z"
confidence: high
modules_core: [overview, core-loop, progression, monetization, economy, social-liveops, market-position, risks-unknowns, sources]
modules_systems: [base-build, content-modes, exploration, session-combat]
modules_entities: [units]
modules: [overview, core-loop, progression, monetization, economy, social-liveops, market-position, risks-unknowns, sources, base-build, content-modes, exploration, session-combat, units]
unit_policy: representative
---

# 疯狂水世界 知识库 Manifest

《疯狂水世界》（英文名及海外版本名：*Wild Water World* / 日本定名：*波乱水世界* / 韩国定名：*아쿠아랜드: 크레이지 서바이벌* / 原测试名 *Flot Shelter*）由益世界（广州益玩网络科技有限公司 / Hong Kong Just Game Technology Limited / IYAGAMES / 香港商阿爾發遊戲）发行，是一款融合了末日海洋生存、模拟经营建设、放置卡牌养成与 SLG 联盟大地图城战的微信小游戏及双端手游。

根据 2026 年 8 月行业权威收入大盘统计，该作勇夺微信小游戏与抖音小游戏月度收入“双榜眼”（第 2 名），并于 9 月 7 日被七麦数据与 36氪评为 8 月热门游戏榜单新晋 Top 30 核心黑马。

截至 2026 年 9 月 11 日最新运营动向：
1. **全球首发登顶日韩台三地 App Store 免费榜 TOP1**：2026 年 9 月 11 日行业最新战报披露，益世界旗下《疯狂水世界》全球版本在首发阶段表现极为强劲，一举**登顶日本、韩国及中国台湾地区 App Store 免费榜 TOP1**！益世界在全球化发行中坚持“先换一片海”（海上末日生存差异化）与“先经营、再探索”的轻量化路径，大幅降低了海外 SLG 用户的理解门槛；在营销层面从“产品本地化”延伸至“营销本地化”，韩国市场力邀影视实力派演员**朴智焕**（以鲜明“小人物生存感”与喜剧特质切入）与超人气啦啦队女神**李珠珢**（面向年轻群体）形成双星协同推广，日本与台湾市场亦精准引爆，阶段性验证了益世界的全球化发行能力；
2. **海外公测稳健推进与首期社群创作截稿评审**：海外版客户端（v1.2.2）运行平稳，Google Play 下载量稳定突破 10 万+（评分稳居 4.3~4.4），李珠珢专属兑换码 `JUEUN777` 持续发挥长尾获客效应；全球首期社群有奖创作大赛“漂流者的海上派对”（Drifting Sea Party）于 9 月 10 日 23:59 UTC+8 正式截稿，今日全面转入作品评审与大奖发放阶段；
3. **金秋双节运营持续深化与礼包码时效刷新**：国内金秋双节（中秋、国庆）前置备战指引与资源囤积规划稳步展开；9 月上旬核心限时兑换码 `SJJ72915` / `SSJJ72915` 已于昨日（9 月 10 日 23:59）正式到期失效；今日继续派发并实测中秋系列限定礼包码（`ASSGMSDAGW`、`TEIQ9QE`、`3RYMWQY`、`DHNDIS9HDS` 等）与 9 月中旬最新批次限时码（`APBG6O46`、`64SJJ72`、`9MPZQHNQ`、`SJJ35190`、`X2U0Y1GE`、`18SJJ53`、`SSJ9A8D`、`W3SSJ5K` 等）；
4. **多端生态数据迁移常态化与公平竞技治理**：微信小程序、抖音小游戏（海岛服/海港服等）及番茄小说等轻端高战玩家向官方原生 APP 迁移角色的申请通道步入标准化日常审批流，保障核心大 R 玩家资产无损迁移；小米游戏中心 9 月好评宠粉活动稳健进行，官方论坛与社区针对 S7 赛季跨区服竞技与大地图城战持续开展防脚本外挂专项治理，维护公平健康的竞技生态。

## 模块选择说明

- **Core (核心模块)**：全量包含 Overview（概述）、Core Loop（核心循环）、Progression（数值与养成）、Monetization（商业化变现）、Economy（经济系统）、Social/LiveOps（社交与长线运营）、Market Position（市场定位与竞品分析）、Risks/Unknowns（风险与未知项）和 Sources（资料来源）。
- **Systems (系统模块)**：
  - `base-build`：涵盖木筏扩展、民居与发电站突破人口上限、切鱼厂/材料厂/建材厂生产线、指挥中心英雄委派加速及基地建筑皮肤机制。
  - `exploration`：涵盖海面物资打捞/自动拾荒、深海潜水探险搜寻高阶蓝图与藏品、钓鱼捕捞、古物修复及动态天气系统。
  - `session-combat`：涵盖 5v5 阵型卡牌战斗、前后排站位、战术飞钩拉人机制、海兽技能辅助（如鳌蟹、海豚、铁甲人鱼）、控制抗性属性、登峰核芯、PVP 战斗超时机制、装备海兽洗练工具“洗刷锁”与 S6/S7 赛季最新国家队及主流实战阵容 Meta。
  - `content-modes`：涵盖关卡挂机推图（70层蓝图分水岭与800关双博士卡关点）、日常试炼副本、竞技场、世界 BOSS、美人鱼联动副本、联盟商船、巅峰擂台赛与大地图联盟城战。
- **Entities (实体模块)**：
  - `units`：遵循 `unit_policy: representative`，精选 15 个影响版本 Meta、S7 赛季与开荒节奏的关键英雄与海兽实体。
