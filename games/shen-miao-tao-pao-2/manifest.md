---
type: Manifest
title: 神庙逃亡2 知识库清单
description: 《神庙逃亡2》（神庙逃跑2 / Temple Run 2 中文版）知识库 Bundle 的模块规划与构成说明。
game_id: shen-miao-tao-pao-2
genre_tags: [endless-runner, casual, pvp-runner, action]
language: zh-CN
timestamp: "2026-09-21T11:00:00Z"
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

## 2026 年 9 月 21 日最新运营动态与知识库同步要点

1. **中秋周末双倍狂欢圆满收官与奖励结算补领期**：2026 年 9 月 21 日正值周一，为期 48 小时的中秋“周末双倍掉落狂欢”正式圆满收官，大盘进入活动代币【中秋月饼】与【节日福袋】的最终结算兑换与补领窗口。周末冲刺阶段玩家集中借助 [小香猪](/entities/units/xiao-xiang-zhu.md) 的额外掉落技能冲刺兑换限定羽翼“花好月圆”与限定灵宠“中秋福灯”；周一开始大盘转入周常巩固与十一国庆黄金周倒计时，为双节长假运营提供平稳过渡；
2. **十一国庆长假 9 天倒计时与迎国庆大版本内容前瞻**：距离 10 月 1 日国庆黄金周仅剩 9 天，项目组全面启动十一黄金周版本的筹备与内容预热。经典国风全明星阵容（如 [赵云](/entities/units/zhao-yun.md)、[雅丹天女](/entities/units/yadan-tian-nu.md)）及中国传统神兽坐骑（如 [年兽](/entities/units/nian-beast.md)、[傲狠](/entities/units/ao-hen.md)）的限时返场轮换排期已全面公布，配套国庆主题集字与赛道狂欢活动已全面就绪；
3. **海外原厂（Imangi Studios）9月重磅大版本：奥林匹斯山（Mount Olympus）与新英雄赫拉克勒斯（Hercules）持续热跑**：全球国际版稳定推进至 v1.136.x / v1.137.0 体系，Imangi Studios 官方在 9 月不仅持续推进“暮光之殿”（Twilight Palace: Academy）返场与新英雄“卢西恩·克罗斯”（Lucien Cross），更重磅推出希腊神话全新主题赛道“奥林匹斯山”（Mount Olympus），配套推出全新传奇英雄“赫拉克勒斯”（Hercules）、神庙通行证“通往奥林匹斯之路”（Road to Olympus Temple Pass）以及“云端之上”（Beyond the Clouds）限时全球金币收集挑战赛，并返场时光胡子西古尔（Sigur Chronos Time Beard）、赵云（Zhao Yun）等角色，与国服中秋及敦煌丝路形成了东西方神话与文化语境下的全球跑酷共振；
4. **社区礼包码（CDKEY）体系最新核验（2026 年 9 月 21 日可用代码）**：全面核验 2026 年 9 月 21 日可用的通用与专属礼包码（通用码 `smtw666`、`smtw888`、`smtw999`、`smtm520`，专属及VIP码 `SVIP666`、`SVIP777`、`SVIP888`，赛季节点码 `FALL2026`、`RUN2026` 等），通过游戏内设置兑换入口为玩家提供开局金币、钻石与实用加速道具；
5. **版本运行态势、减负体系与防作弊公平竞技**：中文稳定版持续维持在 v7.3.2 体系，实物周边收集赛与排位榜单严格执行“3km 赛道道具刷新保护”防脚本机制，配合“黄金矿山”挂机资源产出与订阅特权机制（12元免插页广告、15元免费重生双倍金币、18元荣耀勋章），稳固大盘留存与良性生态。
