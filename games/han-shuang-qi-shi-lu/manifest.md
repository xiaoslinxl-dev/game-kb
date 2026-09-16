---
type: Manifest
title: 寒霜启示录 (Whiteout Survival) 知识库 Manifest
description: 点点互动（Century Games）冰雪末日SLG《寒霜启示录》的OKF v0.1知识库清单与模块配置 rationale。
game_id: han-shuang-qi-shi-lu
genre_tags: [4X SLG, 冰雪末日生存, 模拟经营, 放置挂机, 策略RPG]
language: zh-CN
timestamp: "2026-09-16T11:00:00Z"
confidence: high
modules_core: [overview, core-loop, progression, monetization, economy, social-liveops, market-position, risks-unknowns, sources]
modules_systems: [base-build, content-modes, exploration, matchmaking, session-combat, territory-war]
modules_entities: [units]
modules: [overview, core-loop, progression, monetization, economy, social-liveops, market-position, risks-unknowns, sources, base-build, content-modes, exploration, matchmaking, session-combat, territory-war, units]
unit_policy: representative
---

# 寒霜启示录 知识库 Manifest

## 模块启用说明

1. **核心模块（Core Modules）**：包含概览 ([overview.md](/overview.md))、核心循环 ([core-loop.md](/core-loop.md))、数值与长线养成 ([progression.md](/progression.md))、商业化模型 ([monetization.md](/monetization.md))、双轨经济模型 ([economy.md](/economy.md))、社交与LiveOps运营 ([social-liveops.md](/social-liveops.md))、市场定位与竞品对比 ([market-position.md](/market-position.md))、风险与未知项 ([risks-unknowns.md](/risks-unknowns.md))，以及参考文献 ([sources.md](/sources.md))。
2. **系统模块（Systems Modules）**：
   - `base-build`：大熔炉供暖机制、火晶时代（FC1-FC10及火晶纪元/Fire Crystal Age）、心愿驿站、9座免费娱乐设施、破晓岛生态拓展、幸存者满意度与居民宿舍/猎人小屋等模拟经营建设。
   - `content-modes`：包含探险挂机副本、竞技场、日常整合分页、无尽试炼（Endless Trial - 蛮族首领风吼者·乌尔夫加 Wulfgar）、地心探险（大地之心新增50层）、燃霜矿区、霜龙霸主（跨王国巅峰王座争夺与随时竞猜修改）、王城争霸、冰火战歌联赛（Icefire Warhymn League，预选赛阵型锁定新规）、联盟凛冬围城（Winter Siege）、巴哈姆特30周年线上问答与九宫格联动，以及“双星同行”（Kingshot 联动）与诚品“熊先生书屋”活动。
   - `exploration`：冰原迷雾探索、野外资源点采集、苔原商路（Frost Wind Track）、灯塔情报任务（含军情处理指引）与野兽猎杀。
   - `matchmaking`：竞技场积分匹配、跨服/跨王国战（KvK / SvS）、王国转移（State Transfer，2026年9月13–19日第20组分组，涵盖States 4–4326，今日 00:00 UTC 正式开启第二阶段定向邀请期 Phase II，解锁解雇士兵战力微调机制）、领航荣耀体系（Leading Glory System）、霜龙争霸赛区匹配池与跨服矿区/联赛匹配机制。
   - `session-combat`：包含单局放置回合/小队RPG战斗（探险/竞技场）以及4X大地图部队行军/集结SLG战斗模式，融入T12煌耀兵种战术与第18代新英雄战术协同。
   - `territory-war`：联盟领地大本营与旗帜铺路扩张、堡垒/要塞争夺、太阳城争霸（决战王城）、SvS 最强王国跨服攻防战机制，以及跨赛区巅峰王座争霸“霜龙霸主”（Frostdragon Tyrant）机制。
3. **实体模块（Entities Modules）**：精选 15 名具有新手引导、付费锚定、战斗/内城核心地位与最新第18世代的代表性英雄及专家（Units）。

## 2026年9月16日知识库最新状态说明

- **跨服王国转移（State Transfer）第二阶段（Phase II: 定向邀请期）正式拉开帷幕**：
  第 20 组（涵盖 States 4–4326）跨服移民第一阶段（Phase I 准备与预览期）已于 9 月 15 日 23:59 UTC 正式收官，转服战力上限（Power Cap）全面冻结。今日（9 月 16 日 00:00 UTC），**第二阶段定向邀请期（Phase II: Invitational Transfer）全面启动**，持续 48 小时（至 9 月 17 日 23:59 UTC）：
  1. **名额签发实况**：各王国执政官正全力下发 35 个普通邀请（Ordinary Invites）与 3 个特殊邀请（Special Invites，可破格引入超出 Power Cap 的超级车头大氪）；领航王国（Leading States）则严控发放 20 个普通邀请（不可发放特殊邀请）。
  2. **第二阶段专属机制开放——士兵解雇（Dismiss Troops）**：系统在 Phase 2 与 Phase 3 期间正式开放领主头像（Avatar -> Troops -> Dismiss）直接解雇士兵的特有功能，使需要卡进目标服战力门槛或压低转移卷轴（Transfer Passes）消耗阶梯的领主无须再通过撞田或自杀式集结损耗兵力。
  3. **受邀领主秒转入驻**：收到定向邀请的领主已可一键确认移民，提前抢占心仪王国席位，避开 9 月 18 日 00:00 UTC 开启的第三阶段（Phase III 全员自由转服）“手慢无”的拥挤风险。
- **巴哈姆特 30 週年线上双重合作活动重磅上线**：
  2026 年 9 月 16 日 10:00 至 10 月 15 日 23:59 (UTC+8)，官方台湾代理商杰游有限公司携手巴哈姆特 30 週年庆开启全月线上合作：
  1. **线上问答挑战赛（30 题达人试炼）**：每日 1 题《寒霜启示录》游戏知识问答，连续 30 天，采用双重保底机制，答题必得“每日保底金币”，答对额外送虚宝序号；
  2. **每日九宫格转盘**：每日免费转动 1 次，光圈定格格位直接派发专属虚宝序号或实体周边，双重保底金币全量派发；
  3. **勇者嘉年华联动**：累积金币可直接投入勇者嘉年华主会场大抽奖，兑换序号有效期长达至 2026 年 11 月 30 日 23:59。
- **4 亿玩家里程碑与全球市场地位巩固**：
  官方应用商店（App Store & Google Play）更新主打宣传语“4亿人都在玩的原创冰雪手游”，展现出上线三年超强的长线生命力；Sensor Tower 与 AppMagic 最新 8 月数据显示，《寒霜启示录》以单月近 1 亿美元预估流水高居全球移动游戏第 3 位，全生态总流水逼近 50 亿美元大关；母公司点点互动旗下三支柱矩阵稳居全球发行商内购榜第 2 位。
- **火晶纪元（v1.33.9）机制全量运转与礼包码状态核验**：
  心愿驿站、9 座免费娱乐设施每日随机掉落材料机制平稳运行；成长专家贾斯图斯确认将于 10 月上线；礼包码 `WOS0909`、`gogoWOS`、`2ndYoutubeKR`、`1stYoutubeKR`、`GuDokYTKOR`、`wm6B7MM4u`、`K6ZbjAXK6` 与 `OFFICIALSTORE` 全量有效；已失效码 `4dp5ZGM4c` 持续标红预警。
