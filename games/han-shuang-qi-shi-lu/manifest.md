---
type: Manifest
title: 寒霜启示录 (Whiteout Survival) 知识库 Manifest
description: 点点互动（Century Games）冰雪末日SLG《寒霜启示录》的OKF v0.1知识库清单与模块配置 rationale，已同步2026年10月1日国服无尽冬日国庆黄金周正式开跑与国庆专属兑换码【国庆快乐】上线、巴哈姆特30周年双重线上合作第16日下半程试炼与论坛最新兑换码【4zd7qMQKd】、韩籍啦啦队第二波全家便利商店跨界联动第2天发票虚宝火热兑换、台北诚品生活熊先生书屋昨日圆满闭展收官、官方中秋码26FullMoon正式失效、合服浪潮第3天深度战备与黑土区抢地、转服整编第12日（剩余13天冷却；Group 21定档10月11日）、成长专家Justus定档10月及万圣节前瞻等最新动态。
game_id: han-shuang-qi-shi-lu
genre_tags: [4X SLG, 冰雪末日生存, 模拟经营, 放置挂机, 策略RPG]
language: zh-CN
timestamp: "2026-10-01T11:00:00Z"
confidence: high
research_schema_version: 1
modules_core: [overview, core-loop, progression, monetization, economy, social-liveops, versions, live-events, market-position, risks-unknowns, sources]
modules_systems: [base-build, content-modes, exploration, matchmaking, session-combat, territory-war]
modules_entities: [units]
unit_policy: representative
---

# 寒霜启示录 知识库 Manifest

```yaml
modules:
  core: [overview, core-loop, progression, monetization, economy, social-liveops, versions, live-events, market-position, risks-unknowns, sources]
  systems: [base-build, content-modes, exploration, matchmaking, session-combat, territory-war]
  entities: [units]
unit_policy: representative
```

## 模块启用说明

1. **核心模块（Core Modules）**：包含概览 ([overview.md](overview.md))、核心循环 ([core-loop.md](core-loop.md))、数值与长线养成 ([progression.md](progression.md))、商业化模型 ([monetization.md](monetization.md))、双轨经济模型 ([economy.md](economy.md))、社交与LiveOps运营 ([social-liveops.md](social-liveops.md))、版本总索引 ([versions.md](versions.md))、活动台账 ([live-events.md](live-events.md))、市场定位与竞品对比 ([market-position.md](market-position.md))、风险与未知项 ([risks-unknowns.md](risks-unknowns.md))，以及参考文献与证据台账 ([sources.md](sources.md))。
2. **系统模块（Systems Modules）**：
   - `base-build`：大熔炉供暖机制、火晶时代（FC1-FC10及火晶纪元/Fire Crystal Age）、心愿驿站、9座免费娱乐设施、破晓岛生态拓展、幸存者满意度与居民宿舍/猎人小屋等模拟经营建设。
   - `content-modes`：包含探险挂机副本、竞技场、日常整合分页、无尽试炼（Endless Trial - 蛮族首领风吼者·乌尔夫加 Wulfgar）、地心探险（大地之心新增50层）、燃霜矿区、霜龙霸主（跨王国巅峰王座争夺与随时竞猜修改）、王城争霸、冰火战歌联赛（Icefire Warhymn League，预选赛阵型锁定新规）、联盟凛冬围城（Winter Siege）、合服专属活动【全新起点（A New Beginning）】与【拓荒赞歌（Pioneering Praises）】第3天持续推进、韩籍啦啦队第二波全家便利商店跨界联动「寒霜就是你家！女神专属应援」第2天、国服《无尽冬日》国庆黄金周【辉煌盛世庆典】（含「绣球对碰赢奇珍」对对碰消除玩法与国庆专属兑换码【国庆快乐】）、中秋明月盛典全量闭环与中秋码26FullMoon正式失效、巴哈姆特30周年线上问答第16日达人试炼（全勤领主已解锁周边大抽奖资格，今日最新分享码4zd7qMQKd上线）、Facebook专属Supreme Chief Party审核发奖、诚品生活快闪店“熊先生书屋”（昨日22:00正式圆满闭展谢幕）与2026万圣节活动前瞻「Pumpkin Strike」。
   - `exploration`：冰原迷雾探索、野外资源点采集、苔原商路（Frost Wind Track）、灯塔情报任务（含军情处理指引）与野兽猎杀。
   - `matchmaking`：竞技场积分匹配、跨服/跨王国战（KvK / SvS）、王国转移（State Transfer，2026年9月13–19日第20组分组，涵盖States 4–4326，第三阶段全员自由转服期 Phase III 圆满闭幕，全服进入战后重整与 25 天冷却期第 12 日，剩余 13 天冷却期，下期周期 Group 21 定档 10 月 11–17 日如期启动）、合服浪潮机制（State Merger Wave 2026-09-29，约50组王国归并重组，按活跃玩家数与Top 100总战力匹配，并入编号最大目标服，今日进入第3天深度战备与黑土区抢地）、领航荣耀体系（Leading Glory System）、霜龙争霸赛区匹配池与跨服矿区/联赛匹配机制。
   - `session-combat`：包含单局放置回合/小队RPG战斗（探险/竞技场）以及4X大地图部队行军/集结SLG战斗模式，融入T12煌耀兵种战术与第18代新英雄战术协同。
   - `territory-war`：联盟领地大本营与旗帜铺路扩张、堡垒/要塞争夺、太阳城争霸（决战王城）、SvS 最强王国跨服攻防战机制、跨赛区巅峰王座争霸“霜龙霸主”（Frostdragon Tyrant）机制，以及合服浪潮（State Merger）导致的领地重置、大本营选址落地、黑土区插旗圈地与合服首届总统争霸战备战。
3. **实体模块（Entities Modules）**：精选 15 名具有新手引导、付费锚定、战斗/内城核心地位与最新第18世代的代表性英雄及专家（Units）。

## 2026年10月1日知识库最新状态说明

- **国服《无尽冬日》国庆黄金周正式开跑（2026-10-01 ~ 10-07）与官方国庆专属兑换码上线**：
  北京时间 2026 年 10 月 1 日，国服正式迎来国庆长假，官方社区公告《内含兑换码 | 国庆假期已加载，冰原模式启动！》，正式向全服发放节日专属兑换码【国庆快乐】（需大熔炉等级达标，有效期覆盖长假期间），连同前一日发放的预热兑换码【国庆节活动预告】形成双节福利矩阵；
  1. **全新消除小游戏「绣球对碰赢奇珍」进入黄金周冲刺**：领主通过消耗战备彩券参与庆典对对碰消除小游戏，积攒奇珍积分赢取奇珍宝箱，零氪与微氪玩家通过规划每日绣球任务可高效换取火晶与秘银；
  2. **狮舞庆华章与全服狂欢**：国庆打卡签到、双节专属养成礼包与全服限时掉落全面开启。
- **巴哈姆特 30 週年《寒霜啟示錄》線上雙重合作活動迎來第 16 日（2026-09-16 ~ 10-15）**：
  2026 年 9 月 16 日 10:00 至 10 月 15 日 23:59 (UTC+8)，官方台湾代理商杰游有限公司携手巴哈姆特 30 週年庆开启全月线上合作，今日（10 月 1 日）正式跨入下半程（第 16 日）：
  1. **线上问答挑战赛（30 题达人试炼）**：今日迎来第 16 题专业问答；
  2. **全勤领主已正式解锁 15 次问答实体周边大抽奖**：自 9 月 16 日开幕起每日坚持参与答题的领主，已于昨日达成累计 15 次问答大奖，全面解锁抽取寒霜酷娃包、白熊抱抱毯、寒霜小熊先生、寒霜英雄别册+序号卡等珍稀实体周边的抽奖资格；
  3. **最新社区分享问答兑换码矩阵**：今日巴哈论坛玩家热烈分享 10 月 1 日最新问答达成奖励序号 `4zd7qMQKd`（**1 小时通用加速 x 8、1,000 钻石 x 1、领主体力 x 5**，兑换有效期长达至 **2026 年 11 月 30 日 23:59**），连同昨日分享的 `K9WQ8EB4y`（1,000钻石 x 1、100点强化经验零件 x 2、传说通用英雄碎片 x 1）与 `4jxG5XyKb`、`wm6GMPv4w` 等形成活跃福利矩阵；
  4. **每日九宫格转盘**：今日转盘机会已重置，光圈定格格位直接派发专属虚宝序号或实体周边，双重保底金币全量派发，累积金币可直接投入勇者嘉年华主会场大抽奖。
- **韩籍啦啦队第二波全家便利商店（FamilyMart）跨界联动进入第 2 天（2026-09-30 ~ 10-27）**：
  官方台湾代理商杰游有限公司携手全家便利商店（FamilyMart）与 2026 TGS 展会中亮相的三大人气韩援啦啦队女神（全恩菲 @_j.eunb、郑熙静 @_jung_u、刘世彬 @live_for__me），开展「寒霜就是你家！女神专属应援」跨界联动：
  1. **FamiPort 6 款联名明信片云端列印**：全台全家便利商店 FamiPort 机台开放《寒霜启示录》女神专属 4x6 吋联名明信片云端列印；
  2. **列印明信片送发票虚宝兑换码**：领主列印任一款明信片，发票即可获得专属虚宝兑换码，A 组虚宝（9/30－10/13）全面热烈兑换中，兑换序号有效期限长达至 2026/12/31 23:59，每账号限兑各 1 次；
  3. **拍照留言抽实体周边“寒霜小白熊”**：领主在活动期间拍下明信片上传至官方粉丝团指定贴文并留言，即可参与抽奖，官方将抽取 3 只限量“寒霜小白熊”（抽奖截至 10/27 23:59）。
- **台北诚品生活“熊先生书屋”与诚品动漫祭线下实体快闪店昨日圆满闭展（2026-08-01 ~ 09-30）**：
  历经两个月（8月松烟店、9月西门店，全台 9 大门市巡展），台北诚品生活线下实体快闪店“熊先生书屋”已于昨日（2026 年 9 月 30 日 22:00）迎来最后一天正式圆满闭展收官：官方全彩 26 页漫画《寒霜启示录－英雄别册》（限量 18,000 册）、9 月「寒霜英雄款」附赠礼包卡与“寒霜酷娃包”快闪抽取正式绝版入库。
- **官方中秋专属特辑礼包码 `26FullMoon` 确认正式到期失效闭合**：
  官方全球社群中秋专属礼包码 `26FullMoon` 已于 2026 年 9 月 30 日彻底到期失效，兑换通道已关闭，官方移入失效列表；
  - 10月最新有效码：`国庆快乐`（国服10月1日最新节日码）、`4zd7qMQKd`（10月1日巴哈问答最新码）、`K9WQ8EB4y`、`4jxG5XyKb`、`wm6GMPv4w`（至2026/11/30）、`4zd7pgAKd` / `wQYm5nWw5` / `K5apdBzK5`（巴哈达人问答码）、全家 FamiPort 列印发票序号（A组 9/30~10/13）、国服【国庆节活动预告】、`GuDokYTKOR`、`2ndYoutubeKR`、`1stYoutubeKR`、`gogoWOS`、`OFFICIALSTORE`、`wm6B7MM4u`、`K6ZbjAXK6`；
  - 持续标红已失效码：`26FullMoon`（9月30日到期）、`FallEquinox26`（9月26日到期）、`JPsilverweek26`（9月24日到期）、`中秋节活动预告`（9月22日到期）、`WOS0919`、`K5aM8vzKq`、`WOS0909`、`4dp5ZGM4c`。
- **官方合服浪潮（State Merger Wave 2026-09-29）进入第 3 天深度战备与抢地布局**：
  在 9 月 29 日完成约 50 组成熟服务器强制合服维护后，今日各大联盟新大本营全面落成，旗帜铺设向中央黑土区核心迅速延伸，全力圈占高阶资源田与关键关卡；各公会加紧整编兵力与高阶煌耀兵种储备，全力备战合服后首轮王城争霸（Castle Battle）；专属活动【全新起点】与【拓荒赞歌】火热进行中。
- **跨服王国转移（State Transfer Group 20）战后整编第 12 日推进（剩余 13 天冷却；Group 21 定档 10 月 11–17 日）**：
  第 20 组（涵盖 States 4–4326）跨服移民已圆满闭幕。今日（10 月 1 日），全服处于战后整编第 12 日，迁移领主处于 25 天转服冷却期第 12 日（剩余 13 天冷却）；下一轮转服窗口（Group 21）定档将于 **2026 年 10 月 11 日至 10 月 17 日（UTC）**如期启动。
- **黎明学院收官成长专家贾斯图斯（Justus）定档 10 月正式列装**：
  官方确认根据此前玩家反馈，成长专家[贾斯图斯 (Justus)](entities/units/justus.md)定档于 2026 年 10 月在已解锁 Gen 6 英雄的合格王国中陆续推出，作为 2026 年度最后一位新专家上线；其主打王朝荣耀宝箱、宠物冒险次数与双倍掉落、地心迷宫荧光石收益加成。
- **2026年万圣节活动前瞻与数据爆料「Pumpkin Strike」定档 10 月 26 日**：
  海外玩家社区与客户端数据挖掘披露，2026 年万圣节主题活动预计将于 10 月 26 日开启，将推出全新“南瓜突击（Pumpkin Strike）”机制、新角色/英雄 Cassia、破晓岛防御型专属建筑（Defensive Island Building）及万圣节限定主题城堡装扮。
