---
okf_version: "0.1"
---

# 疯狂水世界 知识库索引

欢迎查阅《疯狂水世界》（英文名：*Flot Shelter*）开放知识库（OKF v0.1 Bundle）。本知识库系统化梳理了益世界旗下“末日海洋生存 + 模拟经营建造 + 放置卡牌 + SLG 联盟城战”小游戏与双端爆款手游的核心玩法机制、系统架构、经济变现与代表性实体。

## 1. 核心文档 (Core Modules)

- [概览 (overview.md)](/overview.md) — 游戏定位、开发背景、混合玩法结构与各大市场奖项（华为年度最受欢迎游戏、微信新锐突破小游戏）
- [架构配置 (manifest.md)](/manifest.md) — 模块构成规划与元数据定义
- [核心循环 (core-loop.md)](/core-loop.md) — 拾荒/潜水 -> 加工/订单 -> 5v5推图/城战 -> 资源再投入的三层闭环
- [数值与养成系统 (progression.md)](/progression.md) — 玩家等级上限（100级）、英雄3星技能质变、专武、超凡装备精炼词条、海兽与藏品长线养成
- [商业化与付费变现 (monetization.md)](/monetization.md) — 12元自动生产特权、首充/月卡/战令阶梯、第8天转盘抽卡、弹窗礼包与赛季商店
- [经济系统 (economy.md)](/economy.md) — 基础建材（木材/塑料/金属）、加工品流水线、钻石硬通货、蓝图建造红线与代币产销循环
- [社交与长线运营 (social-liveops.md)](/social-liveops.md) — 联盟互助科技与大地图城战、周度活动轮换、陈小春代言狂浪节、AI短剧与《美人鱼》跨界联动
- [市场定位与竞品分析 (market-position.md)](/market-position.md) — 益世界“模拟经营+”矩阵定位、与传统SLG/小游戏竞品差异化对比
- [风险与不确定性 (risks-unknowns.md)](/risks-unknowns.md) — 战力数值虚标与胜率脱节、小号攻城刷功勋风险、自动化特权付费门槛与赛季更替贬值
- [资料来源与参考文献 (sources.md)](/sources.md) — 官方渠道、应用商店、行业媒体报道（GameLook/新浪电竞/游侠）与玩家社区攻略汇总

## 2. 系统模块 (Systems Modules)

- [基地建造与生存经营 (systems/base-build.md)](/systems/base-build.md) — 木筏扩展、民居与发电站突破人口上限、工厂加工线与指挥中心英雄委派
- [海域探索与资源收集 (systems/exploration.md)](/systems/exploration.md) — 海面拾荒、深海潜水探险、钓鱼捕捞、古物修复与动态天气系统
- [对抗与卡牌战斗系统 (systems/session-combat.md)](/systems/session-combat.md) — 5v5 阵型卡牌战斗、战术飞钩机制、阵法光环克制与国家队 Meta
- [玩法模式与副本体系 (systems/content-modes.md)](/systems/content-modes.md) — 4300关主线推图、140关试炼副本、限时世界 BOSS、跨服竞技场与大地图联盟城战

## 3. 实体模块 (Entities Modules)

- [代表性英雄与海兽名册总览 (entities/units/_index.md)](/entities/units/_index.md) — 14 个代表性核心英雄与海兽实体图鉴与职能索引
- [大嘴山姆 (entities/units/da-zui-shan-mu.md)](/entities/units/da-zui-shan-mu.md) — 懂王，T0 物理主坦，高闪避与全屏嘲讽聚怪
- [兰博 (entities/units/lan-bo.md)](/entities/units/lan-bo.md) — T0 能量主C，自由者阵营攻速红温爆发与持久战真神
- [探案双子星 (entities/units/tan-an-shuang-zi-xing.md)](/entities/units/tan-an-shuang-zi-xing.md) — 美人鱼联动限定超凡主坦，人鱼分身嘲讽与随赛季进阶技能
- [北境大帝 (entities/units/bei-jing-da-di.md)](/entities/units/bei-jing-da-di.md) — S1 限定超凡坦克/干扰，冲锋切后排与免控霸体
- [千代 (entities/units/qian-dai.md)](/entities/units/qian-dai.md) — S2 限定超凡刺客，精准锁定敌方最高攻目标与隐匿收割
- [巫师老侃 (entities/units/wu-shi-lao-kan.md)](/entities/units/wu-shi-lao-kan.md) — 侃爷，T0 全队增伤与开局护盾核心辅助
- [蜜雪儿 (entities/units/mi-xue-er.md)](/entities/units/mi-xue-er.md) — 极寒冰冻控场与全队回能 16 点战术“发动机”
- [机器屠夫 (entities/units/ji-qi-tu-fu.md)](/entities/units/ji-qi-tu-fu.md) — T0 对位战术飞钩副坦，通关 800 关双博士关键卡
- [铁腿红魔 (entities/units/tie-tui-hong-mo.md)](/entities/units/tie-tui-hong-mo.md) — 物理近战副C与前中排范围控制
- [小丑杰克 (entities/units/xiao-chou-jie-ke.md)](/entities/units/xiao-chou-jie-ke.md) — 高暴击单体秒杀切后刺客，专武 60 级质变
- [一龙 (entities/units/yi-long.md)](/entities/units/yi-long.md) — 6元首充平民开荒物理前排，高性价比范围输出
- [雷教授 (entities/units/lei-jiao-shou.md)](/entities/units/lei-jiao-shou.md) — 新手免费赠送能量群攻过渡卡
- [鳌蟹 (entities/units/ao-xie.md)](/entities/units/ao-xie.md) — S2 超凡品质最强综合防御与套盾免控海兽
- [海豚 (entities/units/hai-tun.md)](/entities/units/hai-tun.md) — 23级培育室解锁万金油持续回血减伤海兽
