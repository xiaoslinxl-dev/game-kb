---
type: Manifest
title: 神庙逃亡2 知识库清单
description: 《神庙逃亡2》（神庙逃跑2 / Temple Run 2 中文版）知识库 Bundle 的模块规划与构成说明。
game_id: shen-miao-tao-pao-2
genre_tags: [endless-runner, casual, pvp-runner, action]
language: zh-CN
timestamp: "2026-09-30T11:00:00Z"
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

## 2026 年 9 月 30 日最新运营动态与知识库同步要点

1. **十一国庆长假倒计时 0 天（今晚 24:00 正式开跑）与黄金周大版本全网爆发前夕**：截至 2026 年 9 月 30 日（周三），迎国庆黄金周进入最后倒计时 0 天（节前黄金预备期全面收官）。创梦天地项目组完成了国庆大版本的全量热更新部署与服务器承载扩容；今夜 24:00（10 月 1 日 0:00），国庆黄金周“七天乐连登豪华签到”和“全明星国风狂欢盛典”正式全面开跑；全明星国风限定角色（如 [赵云](/entities/units/zhao-yun.md)、[雅丹天女](/entities/units/yadan-tian-nu.md)）及中国传统神兽坐骑（如 [年兽](/entities/units/nian-beast.md)、[傲狠](/entities/units/ao-hen.md)）的预购锁定通道将于今晚 24:00 截止，并在 10 月 1 日 0:00 准时转为国庆限时特惠商铺；
2. **全明星国风阵容狂欢盛典与七天乐签到今晚 0 点盛大开启**：全服“七天乐连登豪华签到”预约参与量创新高，玩家连续 7 天登录即可逐日领取海量钻石、金币、稀有道具及限时羽翼试用；排位赛新赛季冲榜与双倍金币掉落狂欢同步于 10 月 1 日 0:00 激活，形成长假初期的强力促活与商业化势能；
3. **九月开学季收官今夜 24:00 终极下线结算**：“玩转九月开学季”活动在 2026 年 9 月 30 日 24:00 正式截档下线，结束整个九月的运营周期。赛道内【书本】与【书包】主题掉落道具今夜 24:00 后不再刷新，开学季活动兑换商城及专属头像框“青春启航”迎来最后数小时兑换倒计时；未使用的开学季代币将在 10 月 1 日凌晨统一按固定汇率（1代币:500金币）折换为基础金币全量发放至玩家邮箱；
4. **海外原厂（Imangi Studios）国际版保持高热运行（v1.136.0 / v1.137.0）**：希腊神话全新主题赛道“奥林匹斯山”（Mount Olympus）热度持续攀升；专属神庙通行证“通往奥林匹斯之路”（Road to Olympus Temple Pass，持续至 10 月 11 日 - 10 月 12 日）处于中程冲刺期，终极大奖传奇新英雄“赫拉克勒斯”（Hercules）受全球跑者追捧；全球挑战“云端之上”（Beyond the Clouds）持续释放丰厚奖励与时光胡子西古尔（Sigur Chronos Time Beard）；海外商城轮换返场经典中国风英雄 [赵云](/entities/units/zhao-yun.md) 与哪吒（Nezha），并开启神秘赛道“暮光之殿”（Twilight Palace）新跑者“卢西恩·克罗斯”（Lucien Cross）的限时挑战；
5. **社区礼包码（CDKEY）体系最新核验（2026 年 9 月 30 日最新有效代码）**：全面核验 2026 年 9 月 30 日可用的通用与专属礼包码（通用码 `smtw666`、`smtw888`、`smtw999`、`smtm520`，专属及VIP码 `SVIP666`、`SVIP777`、`SVIP888`，赛季节点码 `FALL2026`、`RUN2026`，迎国庆前瞻码 `GQ2026` / `CHINA2026` 等），通过游戏内设置兑换入口为玩家提供开局金币、钻石与实用加速道具；
6. **版本运行态势、减负体系与防作弊公平竞技**：中文稳定版持续维持在 v7.3.2 体系，实物周边收集赛与排位榜单严格执行“3km 赛道道具刷新保护”防脚本机制，配合“黄金矿山”挂机资源产出与订阅特权机制（12元免插页广告、15元免费重生双倍金币、18元荣耀勋章），稳固大盘留存与良性生态。
