---
type: Manifest
title: 疯狂水世界 知识库架构配置
description: 疯狂水世界（feng-kuang-shui-shi-jie）知识库 Bundle 的模块架构、元数据配置与收录范围。
game_id: feng-kuang-shui-shi-jie
genre_tags: [survival, simulation, slg, nautical, card-rpg]
language: zh-CN
timestamp: "2026-09-16T11:00:00Z"
confidence: high
modules_core: [overview, core-loop, progression, monetization, economy, social-liveops, market-position, risks-unknowns, sources]
modules_systems: [base-build, content-modes, exploration, session-combat, territory-war]
modules_entities: [ao-xie, bei-jing-da-di, da-zui-shan-mu, dian-yu-zhang-sai-si, guo-jiang-long, hai-tun, ji-qi-tu-fu, lan-bo, mi-xue-er, qian-dai, tan-an-shuang-zi-xing, tie-tui-hong-mo, wu-shi-lao-kan, xiao-chou-jie-ke, yi-long]
unit_policy: representative
---

# 疯狂水世界 知识库架构配置

本文档定义《疯狂水世界》（海外发行定名：*Wild Water World* / 日本定名《波乱水世界》 / 韩国定名《아쿠아랜드: 크레이지 서바이벌》 / 原开发用名 *Flot Shelter*）OKF v0.1 知识库 Bundle 的顶层架构元数据、模块收录策略与最新运营实况。

根据 2026 年 8 月行业权威收入大盘统计，该作勇夺微信小游戏与抖音小游戏月度收入“双榜眼”（第 2 名），并于 9 月 7 日被七麦数据与 36氪评为 8 月热门游戏榜单新晋 Top 30 核心黑马。

截至 2026 年 9 月 16 日最新运营动向：
1. **Enjoy出海深度报道：拆解益世界“模拟经营+SLG”演化与四层融合机制**：2026 年 9 月 16 日，权威出海媒体（Enjoy出海）刊发深度报道《广州厂商再拿爆款：模拟经营+SLG，正在小游戏出海里放大》，系统梳理了益世界从《金币大富翁》《商道高手》到《这城有良田》《Lands of Jail》再到《疯狂水世界》的架构演化路径。剖析了其洋葱式四层模型（Survival 起手吸量 -> Simulation 生产链撑住日常与 12 元自动生产变现 -> Card Battle 承接中期数值并反哺生产 -> Light SLG 16 级压后开放减负城战）；
2. **官方正式下发停服更新公告：S6+ 征服赛季与全新世界剧本「黑潮」定档**：官方定于 9 月 17 日凌晨停服维护，全面升级 S6 及后续高阶赛季为“征服赛季”，首个世界剧本「黑潮」于 9 月 21 日正式开打（8 联盟争夺核心“水之都”、八向城池站位、遭遇黑潮全域禁战）；上线自由组队 2.0 系统（战队战力自动系统排序、50人满编规则）；远征商店 51 级解锁超凡英雄万能碎片兑换；联盟商船半数以上船员参与后倒计时结束即自动启航；狂浪节剩余道具支持批量兑换钻石；
3. **“净海行动”与玩家专场净滩公益深入推进（第 3 天）**：广州南沙线下净滩专场（与广州市海洋双碳研究会联合）报名持续火爆，游戏内“净海行动”主题活动深入推进，将虚拟海面拾荒与现实海洋生态保护长效呼应；
4. **9 月 16 日全网最新有效礼包码实测发布**：各大渠道（7724、JISU极速手游、巴哈姆特等）今日最新实测下发新一批专属礼包兑换码（包括通用码与微信抖音码 `VIP666`、`VIP777`、`VIP888`、中秋限定码、通用码与 KOL 专属码等），确认限时码 `SJJ72915` 彻底失效，iOS 用户需通过官方 Web 兑换中心绑定 UID 领取；
5. **官方安卓客户端 v1.10.7 (463) 持续铺开与跨端账号迁移常态化**：官方最新安卓客户端 `v1.10.7`（安装包约 442MB）在各渠道稳定分发，多端内存调度与跨服巅峰赛场景优化效果显著；微信小程序（海港服）、抖音小游戏（海岛服）向官服原生 APP 迁移申请常态化高效运转。

## 模块选择说明

- **Core (核心模块)**：全量包含 Overview（概述）、Core Loop（核心循环）、Progression（数值与养成）、Monetization（商业化变现）、Economy（经济系统）、Social/LiveOps（社交与长线运营）、Market Position（市场定位与竞品分析）、Risks/Unknowns（风险与未知项）和 Sources（资料来源）。
- **Systems (系统模块)**：
  - `base-build`：涵盖木筏扩展、民居与发电站突破人口上限、切鱼厂/材料厂/建材厂生产线、51 级兵工厂、指挥中心英雄委派加速及基地建筑皮肤机制。
  - `exploration`：涵盖海面物资打捞/自动拾荒（及净海行动现实呼应）、深海潜水探险搜寻高阶蓝图与藏品、钓鱼捕捞、古物修复及动态天气系统。
  - `session-combat`：涵盖 5v5 阵型卡牌战斗、前后排站位、战术飞钩拉人机制、海兽技能辅助（如鳌蟹、海豚、铁甲人鱼）、控制抗性属性、登峰核芯、PVP 战斗超时机制、装备海兽洗练工具“洗刷锁”与 S6/S7 赛季最新国家队及主流实战阵容 Meta。
  - `content-modes`：涵盖关卡挂机推图（70层蓝图分水岭与800关双博士卡关点）、日常试炼副本、竞技场、世界 BOSS、联盟商船协作、海商王贸易与巅峰擂台赛。
  - `territory-war`：涵盖联盟领地大本营、战略硅矿采集（每日30次抢占管控）与巨轮打捞、城市要塞攻防与工事布设、S6+ 征服赛季全新世界剧本「黑潮」（8 联盟争夺水之都与黑潮禁战天候）、自由组队 2.0 系统及联盟科技与战利品分配机制。
- **Entities (实体模块)**：
  - 遵循 `representative` 选育策略，精选 15 个影响不同成长周期与阵容体系的核心代表性实体（涵盖 T0 国家队核心、狂浪节及 S7 超凡限定英雄、跨界联动限定英雄及代表性海兽）。
