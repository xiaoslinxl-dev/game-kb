---
type: Manifest
title: 神庙逃亡2 知识库清单
description: 《神庙逃亡2》（神庙逃跑2 / Temple Run 2 中文版）知识库 Bundle 的模块规划与构成说明。
game_id: shen-miao-tao-pao-2
genre_tags: [endless-runner, casual, pvp-runner, action]
language: zh-CN
timestamp: "2026-10-07T11:00:00Z"
confidence: high
modules_core: [overview, core-loop, progression, monetization, economy, social-liveops, market-position, risks-unknowns, sources]
modules_systems: [session-combat, content-modes]
modules_entities: [units]
modules: [overview, core-loop, progression, monetization, economy, social-liveops, market-position, risks-unknowns, sources, session-combat, content-modes, units]
unit_policy: representative
---

# 模块选择说明

《神庙逃亡2》（神庙逃跑2 / Temple Run 2 中文版）由美国 Imangi Studios 研发、深圳市创梦天地科技有限公司（乐逗游戏 / iDreamSky）在中国大陆引进、深度本土化二次开发并长期运营。作为全球移动游戏史上的现象级 3D 越野跑酷动作手游，其中国版本加入了大量的本土化系统、丰富的主题赛道与长线商业化运营机制。

## 启用模块说明

- **Core (核心模块)**：全量包含 Overview（概述）、Core Loop（核心循环）、Progression（养成与进度）、Monetization（变现与付费设计）、Economy（经济体系与代币循环）、Social/LiveOps（社交与长线运营）、Market Position（市场定位与竞品分析）、Risks/Unknowns（风险与未知项）和 Sources（资料来源与参考文献）。
- **Systems (系统模块)**：
  - `session-combat`：涵盖单局跑酷操作、重力感应与划屏避障、道具拾取、三位一体技能联动以及 2v2 竞技场干扰与对抗机制。
  - `content-modes`：涵盖经典无尽模式、竞技场/排位赛（1v1/2v2）、主题地图副本（如玩具王国、丝路奇遇、赛博神庙、百花戈壁、全民假日、月夜穹顶等）、黄金矿山挂机及限时收集赛等多重玩法。
- **Entities (实体模块)**：采用 `representative`（代表性实体）策略，挑选了 12 个具有代表性的角色、坐骑、宠物与羽翼配饰（如危险盖伊、莉莉丝、赵云、比奥斯博士、安妮、沃利纳特、雅丹天女、年兽、傲狠、仙灵鹤、小香猪、花蝶梦翅膀），覆盖新手入门、长线留存福利、版本付费锚点、传统文化联动与竞技 PvP Meta。

## 2026 年 10 月 7 日最新运营动态与知识库同步要点

1. **十一国庆长假第七天（Day 7）收官日与返程平稳收尾**：截至 2026 年 10 月 7 日（周三），中国国庆黄金周进入第 7 天收官日。随着返程高峰逐渐进入终局平稳期，全服跑酷活跃度平稳过渡，7 天长假累计跑酷总局数与单日 DAU 创下长假新高，离线单机跑酷与在线排位赛双端服务器平稳承载、零故障平稳运行；
2. **“七天乐连登豪华签到”迎来 Day 7 压轴终极大奖正式解锁下发**：全服七天乐签到迎来第 7 天压轴终极大奖解锁，玩家连续登录满 7 天即可免费领取第七天专属至尊大礼包（包含全明星绝版角色/稀有宠物自选礼盒、顶级钻石大礼袋、超级暴走加速道具及幸运宝珠等），七天黄金周留存转化达成终极收官；
3. **排位赛国庆黄金周冲榜季（1v1/2v2）今晚 24:00 终极收官结算**：国庆黄金周排位赛特惠冲榜季进入最后终极决胜冲刺阶段（今晚 10 月 7 日 24:00 准时结束本轮长假限时冲分加成、段位保护卡与胜场双倍积分狂欢），全服排行榜进行赛季荣誉结算，并下发专属国庆黄金周限定头像框、王者称号与丰厚赛季宝箱奖励；
4. **全明星国风特惠商铺与长假充值加赠最后 24 小时收官清盘**：全明星国风限定角色（[赵云](/entities/units/zhao-yun.md)、[雅丹天女](/entities/units/yadan-tian-nu.md)）及中国传统神兽坐骑（[年兽](/entities/units/nian-beast.md)、[傲狠](/entities/units/ao-hen.md)）与羽翼（[花蝶梦](/entities/units/hua-die-meng.md)）的特惠组合进入最后 24 小时限时销售；全赛道双倍金币掉落狂欢今晚 24:00 同步结束，玩家配合 [小香猪](/entities/units/xiao-xiang-zhu.md) 的额外金币掉落技能完成最终资源扫尾；
5. **海外原厂（Imangi Studios）国际版保持高热运行（v1.136.0 / v1.137.0）**：希腊神话全新主题赛道“奥林匹斯山”（Mount Olympus）持续火爆，专属神庙通行证“通往奥林匹斯之路”（Road to Olympus Temple Pass，持续至 10 月 11 日 - 10 月 12 日）仅余最后 4 天极限冲刺期，全球跑者加速积累“赫拉克勒斯的卷轴”（Hercules' Scrolls）冲刺传奇新英雄“赫拉克勒斯”（Hercules）与赫拉克勒斯英雄礼包（Hercules Hero Pack Bundle）；全新全球挑战“赫拉克勒斯的试炼”（Trial of Hercules）全面推进至终局冲刺阶段，全服金币与时光胡子西古尔（Sigur Chronos Time Beard）奖励持续解锁下发；海外商城轮换返场经典中国风英雄 [赵云](/entities/units/zhao-yun.md) 与哪吒（Nezha），神秘赛道“暮光之殿”（Twilight Palace）新跑者“卢西恩·克罗斯”（Lucien Cross）限时挑战进入收尾阶段；国际版 10 月中下旬万圣节特别季（Haunted Harvest / Spooky Summit）前瞻与 10 月 13 日 Google Play Fest 特惠预告进一步升温；
6. **社区礼包码（CDKEY）体系最新核验（2026 年 10 月 7 日最新有效代码）**：全面核验 2026 年 10 月 7 日可用的通用与专属礼包码（通用码 `smtw666`、`smtw888`、`smtw999`、`smtm520`，专属及VIP码 `SVIP666`、`SVIP777`、`SVIP888`，秋季与国庆码 `FALL2026`、`RUN2026`、`GQ2026`、`CHINA2026` 等），通过游戏内设置兑换入口为玩家提供开局金币、钻石与实用加速道具；
7. **节后复工减负过渡与防作弊公平竞技**：明日（10 月 8 日）全国正式复工复课，游戏运营平稳过渡至节后日常减负节奏（“黄金矿山”挂机资源平稳保障日常养成消耗），实物周边收集赛与排位榜单严格执行“3km 赛道道具刷新保护”防脚本机制，配合订阅特权机制（12元免插页广告、15元免费重生双倍金币、18元荣耀勋章），稳固大盘良性生态。
