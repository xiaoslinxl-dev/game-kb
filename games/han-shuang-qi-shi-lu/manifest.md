---
type: Manifest
title: 寒霜启示录 (Whiteout Survival) 知识库 Manifest
description: 点点互动（Century Games）冰雪末日SLG《寒霜启示录》的OKF v0.1知识库清单与模块配置 rationale。
game_id: han-shuang-qi-shi-lu
genre_tags: [4X SLG, 冰雪末日生存, 模拟经营, 放置挂机, 策略RPG]
language: zh-CN
timestamp: "2026-09-22T11:00:00Z"
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
   - `content-modes`：包含探险挂机副本、竞技场、日常整合分页、无尽试炼（Endless Trial - 蛮族首领风吼者·乌尔夫加 Wulfgar）、地心探险（大地之心新增50层）、燃霜矿区、霜龙霸主（跨王国巅峰王座争夺与随时竞猜修改）、王城争霸、冰火战歌联赛（Icefire Warhymn League，预选赛阵型锁定新规）、联盟凛冬围城（Winter Siege）、中秋明月盛典（进入第2日，瑤池月色裝飾包正式发售，妙解千機数阵解谜与壺納千祥投壶小游戏）、巴哈姆特30周年线上问答与九宫格联动，以及“双星同行”（Kingshot 联动）与诚品“熊先生书屋”活动。
   - `exploration`：冰原迷雾探索、野外资源点采集、苔原商路（Frost Wind Track）、灯塔情报任务（含军情处理指引）与野兽猎杀。
   - `matchmaking`：竞技场积分匹配、跨服/跨王国战（KvK / SvS）、王国转移（State Transfer，2026年9月13–19日第20组分组，涵盖States 4–4326，第三阶段全员自由转服期 Phase III 圆满闭幕，转服通道闭合，全服进入战后重整与 25 天冷却期，下期周期预计 10 月中旬开启）、领航荣耀体系（Leading Glory System）、霜龙争霸赛区匹配池与跨服矿区/联赛匹配机制。
   - `session-combat`：包含单局放置回合/小队RPG战斗（探险/竞技场）以及4X大地图部队行军/集结SLG战斗模式，融入T12煌耀兵种战术与第18代新英雄战术协同。
   - `territory-war`：联盟领地大本营与旗帜铺路扩张、堡垒/要塞争夺、太阳城争霸（决战王城）、SvS 最强王国跨服攻防战机制，以及跨赛区巅峰王座争霸“霜龙霸主”（Frostdragon Tyrant）机制。
3. **实体模块（Entities Modules）**：精选 15 名具有新手引导、付费锚定、战斗/内城核心地位与最新第18世代的代表性英雄及专家（Units）。

## 2026年9月22日知识库最新状态说明

- **中秋节「明月盛典」进入第 2 日与「瑤池月色裝飾包」正式开售（Moonlit Celebration, 2026-09-21 ~ 09-27）**：
  官方中秋限时盛典于今日（9 月 22 日）迎来第 2 日高潮推进：
  1. **瑤池月色裝飾包（Moonlit Paradise Decoration Pack）今日正式开售**：今日（9 月 22 日 00:00:00 UTC）至 9 月 26 日 23:59:59 UTC 限时发售，上架节日绝版东方仙境主题城堡外观、专属行军特效及限定头像框/铭牌装扮；
  2. **妙解千機（5x5 数字数阵解谜）进入第 2 轮**：消耗「祝福明燈」放飞抽取数字点亮数阵，连通 3 条横线或纵线即可解锁大奖并获取「盈月之章」；
  3. **壺納千祥（传统投壶宴饮小游戏）**：游侠无名带来东方古代投壶玩法，操控角度力度投壶争夺每日挑战排行积分与节日好礼；
  4. **流光的樂章 & 燈彩映月華**：行列式战备任务持续开放，全服点灯与幸存者团圆；
  5. **望月商舖 & 累儲好禮**：【望月商舖】支持兑换永久主城外观「月上仙宮」（Moon Pavilion）与专属铭牌「玉兔迎月」（Lunar Rabbit）；
  6. **最新专属礼包兑换码动态与到期告警**：
     - 秋分/日本白银周特辑礼包码 `JPsilverweek26`（含 1,000 宝石、2 把黄金钥匙、200 强化经验组件及海量物资）稳定有效；
     - 国内客户端预热码 `中秋节活动预告` 今日迎来最后兑换期限（有效至 2026-09-22 23:59，需熔炉 Lv.9，今日最后兑换机会）；
     - 官方全球特辑礼包码 `WOS0919` 已于昨日（9 月 21 日 23:59:00 UTC）正式到期失效闭合，移入失效列表。
- **跨服王国转移（State Transfer Group 20）战后整编第 3 日推进**：
  第 20 组（涵盖 States 4–4326）跨服移民已于 9 月 19 日 23:59 UTC 正式圆满收官。今日（9 月 22 日），全服处于战后整编第 3 日：
  1. **“解雇士兵（Dismiss Troops）”专属入口已下线**：兵力变动恢复为常规战斗与战损模式；
  2. **战后阵型重组与战备期深度推进**：各大主力联盟完成人员收口与内部分组，各大公会展开主战盟与农场盟的人员整编，清点高阶兵力与煌耀兵种储备，全力备战接下来的太阳城争霸与跨服 SvS 最强王国战；
  3. **冷却期激活与下期周期前瞻**：迁移领主处于 25 天转服冷却期第 3 日；依据官方每 28 天一次的固定周期规律，下一轮转服窗口（Group 21）预计将于 2026 年 10 月中旬如期启动。
- **巴哈姆特 30 週年线上双重合作活动进入第 7 日**：
  2026 年 9 月 16 日 10:00 至 10 月 15 日 23:59 (UTC+8)，官方台湾代理商杰游有限公司携手巴哈姆特 30 週年庆开启全月线上合作：
  1. **线上问答挑战赛（30 题达人试炼）**：今日迎来第 7 题专业问答，连续 30 天采用双重保底机制，答题必得“每日保底金币”，答对额外送虚宝序号；
  2. **每日九宫格转盘**：今日转盘机会已重置，光圈定格格位直接派发专属虚宝序号或实体周边，双重保底金币全量派发；
  3. **勇者嘉年华联动**：累积金币可直接投入勇者嘉年华主会场大抽奖，兑换序号有效期长达至 2026 年 11 月 30 日 23:59。
- **Sensor Tower 8月出海榜单确认点点互动全球第 2**：
  Sensor Tower 最新发布的 2026 年 8 月中国手游发行商全球收入榜显示，腾讯、点点互动、柠檬微趣稳居全国前三；《寒霜启示录》以单月近 1 亿美元预估流水高居全球移动游戏第 3 位，全生态总流水逼近 50 亿美元大关；点点互动旗下三支柱矩阵巩固全球领先地位。
- **火晶纪元（v1.33.9）机制全量运转与礼包码状态核验**：
  心愿驿站、9 座免费娱乐设施每日随机掉落材料机制平稳运行；成长专家贾斯图斯确认将于 10 月上线；礼包码 `JPsilverweek26`、`中秋节活动预告`（今日到期）、`GuDokYTKOR`、`2ndYoutubeKR`、`1stYoutubeKR`、`gogoWOS`、`OFFICIALSTORE`、`wm6B7MM4u`、`K6ZbjAXK6` 全量有效；已失效码 `WOS0919`、`K5aM8vzKq`、`WOS0909`、`4dp5ZGM4c` 持续标红预警。
