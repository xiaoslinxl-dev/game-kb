---
type: Manifest
title: 寒霜启示录 (Whiteout Survival) 知识库 Manifest
description: 点点互动（Century Games）冰雪末日SLG《寒霜启示录》的OKF v0.1知识库清单与模块配置 rationale，已同步2026年9月29日合服浪潮（State Merger Wave ~50组）正式执行落地与版图重置、中秋盛典全面收官与资产折算、中秋码26FullMoon最后数小时压哨冲刺、Facebook专属Supreme Chief Party今日截标、巴哈问答第14日（明日第15日解锁周边大抽奖）、转服整编第10日（剩余15天冷却；Group 21定档10月11日）与2026万圣节前瞻等最新动态。
game_id: han-shuang-qi-shi-lu
genre_tags: [4X SLG, 冰雪末日生存, 模拟经营, 放置挂机, 策略RPG]
language: zh-CN
timestamp: "2026-09-29T11:00:00Z"
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
   - `content-modes`：包含探险挂机副本、竞技场、日常整合分页、无尽试炼（Endless Trial - 蛮族首领风吼者·乌尔夫加 Wulfgar）、地心探险（大地之心新增50层）、燃霜矿区、霜龙霸主（跨王国巅峰王座争夺与随时竞猜修改）、王城争霸、冰火战歌联赛（Icefire Warhymn League，预选赛阵型锁定新规）、联盟凛冬围城（Winter Siege）、合服专属活动【全新起点（A New Beginning）】与【拓荒赞歌（Pioneering Praises）】、中秋明月盛典（全面收官闭环，资产折算安全生肉与补给箱全量发放）、巴哈姆特30周年线上问答第14日达人试炼（全勤领主迎来最后24小时倒计时，明日第15日正式解锁周边大抽奖资格）、Facebook专属Supreme Chief Party今日截标，以及“双星同行”（Kingshot 联动）、诚品“熊先生书屋”（进入最后48小时闭幕倒计时）与2026万圣节活动前瞻。
   - `exploration`：冰原迷雾探索、野外资源点采集、苔原商路（Frost Wind Track）、灯塔情报任务（含军情处理指引）与野兽猎杀。
   - `matchmaking`：竞技场积分匹配、跨服/跨王国战（KvK / SvS）、王国转移（State Transfer，2026年9月13–19日第20组分组，涵盖States 4–4326，第三阶段全员自由转服期 Phase III 圆满闭幕，全服进入战后重整与 25 天冷却期第 10 日，剩余 15 天冷却期，下期周期 Group 21 定档 10 月 11–17 日如期启动）、合服浪潮机制（State Merger Wave 2026-09-29，约50组王国归并重组，按活跃玩家数与Top 100总战力匹配，并入编号最大目标服）、领航荣耀体系（Leading Glory System）、霜龙争霸赛区匹配池与跨服矿区/联赛匹配机制。
   - `session-combat`：包含单局放置回合/小队RPG战斗（探险/竞技场）以及4X大地图部队行军/集结SLG战斗模式，融入T12煌耀兵种战术与第18代新英雄战术协同。
   - `territory-war`：联盟领地大本营与旗帜铺路扩张、堡垒/要塞争夺、太阳城争霸（决战王城）、SvS 最强王国跨服攻防战机制、跨赛区巅峰王座争霸“霜龙霸主”（Frostdragon Tyrant）机制，以及合服浪潮（State Merger）导致的领地重置、主城随机迁城、旗帜建材100%返还与合服首届总统争霸战。
3. **实体模块（Entities Modules）**：精选 15 名具有新手引导、付费锚定、战斗/内城核心地位与最新第18世代的代表性英雄及专家（Units）。

## 2026年9月29日知识库最新状态说明

- **官方合服浪潮（State Merger Wave 2026-09-29 UTC）今日正式执行与雪原版图大洗牌**：
  官方于今日（2026 年 9 月 29 日 UTC）正式对此前公示的约 50 组成熟王国执行强制合服维护操作：
  1. **归并与目标王国确立**：各合服组别依据服务器活跃玩家总数与 Top-100 领主综合战力进行配对，组内所有源王国（Sources）统一合并至组内编号最大的目标王国（Destination，Highest State Code）；
  2. **主城随机迁城与领地重置**：合服完成后，所有参与王国的领主主城被系统随机传送至雪原安全区域；原各联盟的大本营（HQ）与旗帜领地全盘重置清空，旗帜建造消耗的基础资源 100% 全额原路返还至联盟金库；
  3. **重建瓶颈与圈地竞赛**：各联盟迅速进入“重建瓶颈期（Rebuilding Bottleneck）”，盟内管理争分夺秒确立新大本营并铺设旗帜圈占黑土区与高阶资源点；成员使用联盟迁城或高级迁城重新聚拢；
  4. **王权与官职全盘归零**：合并前各服产生的总统（执政官）称号与官职全部清空，所有要塞与堡垒重新开放争夺；合并后各大公会将通过首场王城争霸（Castle Battle）决出新王国的首任最高统治者；
  5. **合服专属活动开启**：并服后的新王国同步上线【全新起点（A New Beginning）】纪念碑全服协作任务与【拓荒赞歌（Pioneering Praises）】个人/联盟宝箱积分回馈活动，加速新服生态凝聚。
- **中秋节「明月盛典」全量闭环、资产邮件自动折算与中秋特辑码 `26FullMoon` 最后数小时压哨冲刺（Moonlit Celebration Closed）**：
  官方中秋限时盛典在经历核心任务与【望月商舖】（于昨日 9 月 28 日 23:59:59 UTC 彻底关闭）后，今日（9 月 29 日）宣告全面收官圆满闭环：
  1. **资产自动折算落地**：未在商铺关闭前消耗的「盈月之章」已按 1:1,000 安全生肉、未放飞的「祝福明燈」已按 1:10,000 安全资源补给箱，由系统通过游戏内邮件完成全量折算下发；
  2. **中秋特辑码 `26FullMoon` 迎来最后数小时压哨兑换**：官方社群中秋专属礼包码 `26FullMoon`（含 1,000 宝石、8 个 1 小时训练加速、50K 生肉、50K 木材、10K 煤炭、5K 铁矿、200 VIP 经验、1 把黄金钥匙）将于**今日 9 月 29 日 23:59:00 UTC / 9月30日 07:59 UTC+8 正式过期失效**，各大攻略站发出最终极限压哨提醒；
  3. **最新专属礼包兑换码动态与到期更新**：
     - 今日有效码：`26FullMoon`（今日到期）、`wm6GMPv4w`（巴哈问答最新码，至 2026/11/30）、`4zd7pgAKd` / `wQYm5nWw5` / `K5apdBzK5`（巴哈达人问答码）、`GuDokYTKOR`、`2ndYoutubeKR`、`1stYoutubeKR`、`gogoWOS`、`OFFICIALSTORE`、`wm6B7MM4u`、`K6ZbjAXK6`；
     - 持续标红已失效码：`FallEquinox26`（9月26日到期）、`JPsilverweek26`（9月24日到期）、`中秋节活动预告`（9月22日到期）、`WOS0919`（9月21日到期）、`K5aM8vzKq`（9月21日到期）、`WOS0909`、`4dp5ZGM4c`。
- **跨服王国转移（State Transfer Group 20）战后整编第 10 日推进（剩余 15 天冷却；Group 21 定档 10 月 11–17 日）**：
  第 20 组（涵盖 States 4–4326）跨服移民已于 9 月 19 日 23:59 UTC 圆满闭幕。今日（9 月 29 日），全服处于战后整编第 10 日：
  1. **战后阵型重组与战备期深度推进**：各大主力联盟完成人员收口与内部分组，各大公会主战盟与分盟架构完全确立，清点高阶兵力与煌耀兵种储备，全力备战接下来的太阳城争霸与跨服 SvS 最强王国战；
  2. **冷却期激活与下期周期前瞻**：迁移领主处于 25 天转服冷却期第 10 日（剩余 15 天冷却）；社区权威转服看板（WSCO Transfer Board）确认，下一轮转服窗口（Group 21）定档将于 **2026 年 10 月 11 日至 10 月 17 日（UTC）**如期启动，目前已开启新一轮跨服组别预测与转服意向登记。
- **巴哈姆特 30 週年线上双重合作活动进入第 14 日（明日第 15 日解锁周边大抽奖资格）**：
  2026 年 9 月 16 日 10:00 至 10 月 15 日 23:59 (UTC+8)，官方台湾代理商杰游有限公司携手巴哈姆特 30 週年庆开启全月线上合作：
  1. **线上问答挑战赛（30 题达人试炼）**：今日迎来第 14 题专业问答；
  2. **全勤领主迎来最后 24 小时倒计时**：自 9 月 16 日开幕起每日坚持参与答题的领主，在今日完成第 14 题答题后，**仅差最后 1 天答题**即可在明日（9 月 30 日，第 15 日）正式解锁累计 15 次问答实体周边大抽奖资格（抽取寒霜酷娃包、白熊抱抱毯、寒霜小熊先生、寒霜英雄别册+序号卡等限量周边）；
  3. **每日九宫格转盘**：今日转盘机会已重置，光圈定格格位直接派发专属虚宝序号或实体周边，双重保底金币全量派发；累积金币可直接投入勇者嘉年华主会场大抽奖。
- **官方 Facebook「Supreme Chief Party」专属社区活动今日截标闭环（Closing Today, 9-29 23:59 UTC）**：
  2026 年 9 月 24 日至 9 月 29 日 23:59 UTC，官方 Facebook 面向持有“Supreme Chief”（头号粉丝）顶级徽章领主开启的专属回馈派对将于今日（9 月 29 日 23:59 UTC）正式截标收官，官方将在 3 个工作日内向 100 位入选领主发放 14 天限定专属头像框。
- **诚品书店“熊先生书屋”与诚品动漫祭线下联动进入最后 48 小时闭幕倒计时（2026-08-01 ~ 09-30）**：
  全台 9 大门市合作进入最后 48 小时闭幕倒计时（将于明日 9 月 30 日 22:00 结束圆满闭展），官方全彩 26 页漫画《寒霜启示录－英雄别册》（限量 18,000 册）与 9 月「寒霜英雄款」附赠礼包卡进入最终绝版清仓阶段。
- **2026年万圣节活动前瞻与数据爆料 (Halloween 2026 Leaks)**：
  海外玩家社区与客户端数据挖掘披露，2026 年万圣节主题活动预计将于 10 月 26 日开启，将推出全新“南瓜突袭（Pumpkin Strike）”机制、时隔数月回归的“卡西亚许愿小屋（Kasia's Wish House）”、破晓岛防御型专属建筑及万圣节限定主题城堡装扮；晨曦学堂收官成长专家贾斯图斯确认将于 10 月上线。
- **Sensor Tower 8月出海榜单确认点点互动全球第 2**：
  Sensor Tower 最新发布的 2026 年 8 月中国手游发行商全球收入榜显示，腾讯、点点互动、柠檬微趣稳居全国前三；《寒霜启示录》以单月近 1 亿美元预估流水高居全球移动游戏第 3 位，全生态总流水逼近 50 亿美元大关；点点互动旗下三支柱矩阵巩固全球领先地位。
