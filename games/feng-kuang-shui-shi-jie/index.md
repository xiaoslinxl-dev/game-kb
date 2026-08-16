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
- [资料来源与参考文献 (sources.md)](/sources.md) — 官方渠道、应用商店、行业媒体报道（GameLook/新浪电竞/凤凰网/游侠）与玩家社区攻略汇总

## 2. 系统模块 (Systems)

- [基地建造与生存经营 (systems/base-build.md)](/systems/base-build.md) — 木筏扩展、民居/发电站人口突破、切鱼厂/材料厂/选种厂加工流水线与指挥中心英雄委派
- [海域探索与资源收集 (systems/exploration.md)](/systems/exploration.md) — 海面拾荒、深海潜水探险、钓鱼垂钓、古物修复与动态天气系统
- [对抗与卡牌战斗系统 (systems/session-combat.md)](/systems/session-combat.md) — 5v5 前后排布阵、战术飞钩机制、阵法加成与海兽技能协同
- [玩法模式与副本体系 (systems/content-modes.md)](/systems/content-modes.md) — 主线闯关（70关蓝图分水岭与800关双博士）、日常试炼副本、竞技场、世界 BOSS 与大地图联盟城战

## 3. 实体模块 (Entities)

本知识库采用 `representative`（代表性实体）策略，收录了 14 个核心英雄与海兽：

- [实体名册总览 (entities/units/_index.md)](/entities/units/_index.md) — 代表性英雄与海兽名册导航
- **T0 国家队与关键主战英雄**：
  - [大嘴山姆 (da-zui-shan-mu.md)](/entities/units/da-zui-shan-mu.md) — 物理主坦（懂王，全屏嘲讽聚怪，闪避反击）
  - [兰博 (lan-bo.md)](/entities/units/lan-bo.md) — 能量主C（自由者核心，红温无上限增伤，持久战一哥）
  - [探案双子星 (tan-an-shuang-zi-xing.md)](/entities/units/tan-an-shuang-zi-xing.md) — 坦克/召唤（美人鱼联动限定超凡主坦，人鱼分身聚怪承伤）
  - [北境大帝 (bei-jing-da-di.md)](/entities/units/bei-jing-da-di.md) — 坦克/干扰（S1 限定超凡，冲锋切后排霸体免控）
  - [千代 (qian-dai.md)](/entities/units/qian-dai.md) — 刺客/爆发（S2 限定超凡，精准锁定最高攻击主C连环收割）
  - [巫师老侃 (wu-shi-lao-kan.md)](/entities/units/wu-shi-lao-kan.md) — 增伤辅助（侃爷，开局全队护盾，攻速暴击全面强化）
  - [蜜雪儿 (mi-xue-er.md)](/entities/units/mi-xue-er.md) — 控场辅助（极寒冰冻打断，全队能量快速回复）
  - [机器屠夫 (ji-qi-tu-fu.md)](/entities/units/ji-qi-tu-fu.md) — 副坦/控制（对位战术飞钩，集火秒杀与通关双博士必备）
  - [铁腿红魔 (tie-tui-hong-mo.md)](/entities/units/tie-tui-hong-mo.md) — 物理副C（前中排范围打击与群体眩晕控制）
  - [小丑杰克 (xiao-chou-jie-ke.md)](/entities/units/xiao-chou-jie-ke.md) — 暴击刺客（单体秒杀切后排，克制敌方脆皮）
- **开荒过渡英雄**：
  - [一龙 (yi-long.md)](/entities/units/yi-long.md) — 6元首充平民前排，强力群攻清理杂兵
  - [雷教授 (lei-jiao-shou.md)](/entities/units/lei-jiao-shou.md) — 新手免费能量群攻，平稳过渡后可无损重生
- **核心代表性海兽**：
  - [鳌蟹 (ao-xie.md)](/entities/units/ao-xie.md) — S2 超凡品质最强防御海兽，全队高额护盾与霸体免控
  - [海豚 (hai-tun.md)](/entities/units/hai-tun.md) — 23级解锁万金油海兽，持续为 3 名友军提供回血与减伤
