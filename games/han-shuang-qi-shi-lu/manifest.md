---
type: Manifest
title: 寒霜启示录 (Whiteout Survival) 知识库 Manifest
description: 点点互动（Century Games）冰雪末日SLG《寒霜启示录》的OKF v0.1知识库清单与模块配置 rationale。
game_id: han-shuang-qi-shi-lu
genre_tags: [4X SLG, 冰雪末日生存, 模拟经营, 放置挂机, 策略RPG]
language: zh-CN
timestamp: "2026-09-12T11:00:00Z"
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
   - `content-modes`：包含探险挂机副本、竞技场、日常整合分页、无尽试炼（Endless Trial - 蛮族首领风吼者·乌尔夫加 Wulfgar）、地心探险（大地之心新增50层）、燃霜矿区、霜龙霸主（跨王国巅峰王座争夺与随时竞猜修改）、王城争霸、冰火战歌联赛（Icefire Warhymn League，2026年9月3日预选赛阵型锁定新规）、联盟凛冬围城（Winter Siege）以及“双星同行”（Kingshot 联动）与诚品“熊先生书屋”活动。
   - `exploration`：冰原迷雾探索、野外资源点采集、苔原商路（Frost Wind Track）、灯塔情报任务（含军情处理指引）与野兽猎杀。
   - `matchmaking`：竞技场积分匹配、跨服/跨王国战（KvK / SvS）、王国转移（State Transfer，2026年9月13–19日第20组分组，涵盖States 4–4326，正处于最后不足13小时临战终极倒计时）、领航荣耀体系（Leading Glory System）、霜龙争霸赛区匹配池与跨服矿区/联赛匹配机制。
   - `session-combat`：包含单局放置回合/小队RPG战斗（探险/竞技场）以及4X大地图部队行军/集结SLG战斗模式，融入T12煌耀兵种战术与第18代新英雄战术协同。
   - `territory-war`：联盟领地大本营与旗帜铺路扩张、堡垒/要塞争夺、太阳城争霸（决战王城）、SvS 最强王国跨服攻防战机制，以及跨赛区巅峰王座争霸“霜龙霸主”（Frostdragon Tyrant）机制。
3. **实体模块（Entities Modules）**：精选 15 名具有新手引导、付费锚定、战斗/内城核心地位与最新第18世代的代表性英雄及专家（Units）。

## 2026年9月12日知识库最新状态说明

- **跨服王国转移（State Transfer）进入最后13小时临战倒计时**：第20组（涵盖States 4–4326）移民窗口定于2026年9月13日00:00 UTC（北京时间08:00）正式开启第一阶段，当前进入最后不足13小时临战冲刺阶段。各王国管理层正在最终敲定Power Cap与普通/特殊邀请席位，领主正在全面清理溢出非安全资源、排空医务所伤兵并储备移民卷轴。
- **活跃礼包码核实与临界失效提醒**：限时大额资源礼包码 `4dp5ZGM4c` **于今日（9月12日）迎来最后兑换截止日（不足13小时紧急失效预警）**；`WOS0909`（9月9日上线）持续稳定有效；常驻与社区专属码保持活跃；线下诚品动漫祭西门店“熊先生书屋”持续开展9月消费礼并配发“寒霜英雄款”专属兑换码。
- **跨赛区巅峰王座争夺“霜龙霸主”（Frostdragon Tyrant）全面收录**：正式收录超越单服与双服的顶级军团争夺战机制，详尽解构霜龙古国中央王城、生命/庇护/龙息/锋刃四座神秘石塔增益、护卫水晶战术技能、车头超百万钻石与数千加速的高烈度战损模型，以及战前竞猜全面支持开打前无损随时修改的最新机制。
- **财务与市场矩阵核实**：Sensor Tower 与 AppMagic 最新数据显示，《寒霜启示录》海外单月流水稳居近1亿美元（8月全球手游总收入第3，AppMagic净流水9690万美元位列全球第6），稳居全球4X SLG霸主地位；母公司Century Games（点点互动）三支柱矩阵（《Whiteout Survival》、《Kingshot》与《Tasty Travels》）合力吸金，稳居全球发行商内购收入榜第2位。
- **火晶纪元资料片（v1.33.9）机制全量运转**：心愿驿站（Wish Station）与心愿印记、9座免费娱乐设施每日随机掉落领主装备/宝符/宠物/专家材料、无尽试炼风吼者乌尔夫加挑战、大地之心新增50层高难关卡稳步推进，成长专家贾斯图斯推迟至10月上线。
