---
type: Manifest
title: 疯狂水世界 知识库 Manifest
description: 疯狂水世界（feng-kuang-shui-shi-jie）知识库 Bundle 的模块规划与构成说明。
game_id: feng-kuang-shui-shi-jie
genre_tags: [survival, simulation, slg, nautical, card-rpg]
language: zh-CN
timestamp: "2026-09-12T11:00:00Z"
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

截至 2026 年 9 月 12 日最新运营动向：
1. **全球首发登顶日韩台 App Store 免费榜 TOP1 势头巩固与海外本地化纵深**：益世界《疯狂水世界》（海外版 *Wild Water World* / 日本《波乱水世界》 / 韩国《아쿠아랜드: 크레이지 서바이벌》）全球版本在首发阶段强势登顶日本、韩国及中国台湾地区 App Store 免费榜 TOP1 后，全球多地媒体（新浪、网易、CSDN、手游那点事）深度评析其“先换一片海”（末日海洋生存题材）与“先经营、再探索”的轻量化破局逻辑。在营销上实现“营销本地化”跃升，韩国市场力邀影视实力派演员**朴智焕**（以鲜明“小人物生存感”与喜剧特质切入）推出喜剧求生 webCM 并派发专属码 `CRAZY777`，与台湾市场超人气啦啦队女神**李珠珢**（`JUEUN777`）形成双星协同推广；日本市场《波乱水世界》由 EWORLDGAME 发行，Gamerch 等主流攻略站力荐其 10 分钟解锁无线电台、无须繁琐刷初始（リセマラ不要）的放置建造特色；
2. **海外社群创作大赛截稿评审与大奖定档**：首期全球社群创作大赛“漂流者的海上派对”（Drifting Sea Party / 표류자들의 해상 파티）已于 9 月 11 日凌晨全面截稿，正式转入评审阶段，最终评选结果将于 9 月 25 日 13:00 KST 揭晓，提供 iPhone 17 Pro、PS5 Pro、Nintendo Switch 2 等重磅大奖；Google Play 评分稳居 4.3~4.4，下载量超 10 万+；
3. **金秋双节运营深化与 9 月 12 日最新批次礼包码实测发布**：国内金秋双节（中秋、国庆）前置备战指引与资源囤积规划稳步展开；9 月上旬限时码 `SJJ72915` 确认过期后，今日（9 月 12 日）各大渠道最新验证并下发全新一批 15 个有效兑换码（`DSFMFDSKHDSF`、`WETEIWQ9T`、`FSJSWATER`、`FSJSVIPGIFT`、`FSJSYUE08`、`FSJSLUCK`、`RQHRIQW9H`、`DGDSGMK`、`SDHFI9HS`、`ADGDSAGMK`、`ETMWKYQW`、`3WETIEW9T`、`ADSGMDSKG`、`RQHIQ9H`、`afmskg`）及活跃码；
4. **赛季节奏与超凡英雄培养模型明确**：玩家社区与攻略组验证全区服标准 18 天一个赛季周期（S1 结束 2 服合服进 S2，后续 4 服合服并提供 72 小时自由组盟窗口）。核心超凡英雄（S1 北境大帝、S2 雾隐千代）高阶培养资源门槛明确为 1400 碎片与 1120 本技能书，4 星解锁 5 级技能，专武升至 50 级需中级 725、高级 900、特级 350 合金；
5. **跨端迁移常态化与公平竞技反脚本外挂**：微信小程序、抖音小游戏向官方原生 APP 的角色迁移申请步入标准化日常审批流；官方论坛持续发布反外挂脚本治理通告，保障跨服竞技与大地图攻城的生态公平。

## 模块选择说明

- **Core (核心模块)**：全量包含 Overview（概述）、Core Loop（核心循环）、Progression（数值与养成）、Monetization（商业化变现）、Economy（经济系统）、Social/LiveOps（社交与长线运营）、Market Position（市场定位与竞品分析）、Risks/Unknowns（风险与未知项）和 Sources（资料来源）。
- **Systems (系统模块)**：
  - `base-build`：涵盖木筏扩展、民居与发电站突破人口上限、切鱼厂/材料厂/建材厂生产线、指挥中心英雄委派加速及基地建筑皮肤机制。
  - `exploration`：涵盖海面物资打捞/自动拾荒、深海潜水探险搜寻高阶蓝图与藏品、钓鱼捕捞、古物修复及动态天气系统。
  - `session-combat`：涵盖 5v5 阵型卡牌战斗、前后排站位、战术飞钩拉人机制、海兽技能辅助（如鳌蟹、海豚、铁甲人鱼）、控制抗性属性、登峰核芯、PVP 战斗超时机制、装备海兽洗练工具“洗刷锁”与 S6/S7 赛季最新国家队及主流实战阵容 Meta。
  - `content-modes`：涵盖关卡挂机推图（70层蓝图分水岭与800关双博士卡关点）、日常试炼副本、竞技场、世界 BOSS、美人鱼联动副本、联盟商船、巅峰擂台赛与大地图联盟城战。
- **Entities (实体模块)**：
  - `units`：遵循 `unit_policy: representative`，精选 15 个影响版本 Meta、S7 赛季与开荒节奏的关键英雄与海兽实体。
