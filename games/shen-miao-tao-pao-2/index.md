---
okf_version: "0.1"
---

# 神庙逃亡2 知识库索引

欢迎查阅《神庙逃亡2》（神庙逃跑2 / Temple Run 2 中文版）开放知识库（OKF v0.1 Bundle）。本知识库系统化梳理了美国 Imangi Studios 研发、创梦天地（乐逗游戏 / iDreamSky）深度二次开发与长期运营的国民级 3D 越野跑酷动作手游的核心机制、长线系统、经济变现与代表性实体。

## 1. 核心分析模块 (Core)

- [游戏概述 (overview.md)](/overview.md) — 游戏基本信息、研发发行背景、本土化二次开发与长青产品概况
- [架构配置 (manifest.md)](/manifest.md) — 模块规划与元数据定义
- [核心循环 (core-loop.md)](/core-loop.md) — 单局避障跑酷 -> 资源结算 -> 三位一体角色/坐骑/宠物养成 -> 竞技/高分追求的闭环架构
- [进度与养成系统 (progression.md)](/progression.md) — 通用属性金币升级、角色/坐骑/宠物/羽翼技能协同与排位赛赛季段位晋升
- [商业化与变现设计 (monetization.md)](/monetization.md) — 混合变现模式（内购 IAP + 激励广告 IAA + 礼包直购 + 宝珠盲盒抽卡）
- [经济系统与代币循环 (economy.md)](/economy.md) — 金币、钻石、幸运宝珠与活动代币的产销流转与防通胀机制
- [社交与长线运营 (social-liveops.md)](/social-liveops.md) — 2v2 组队排位、好友排行榜、高频主题版本、收集赛与黄金矿山挂机
- [市场定位与竞品分析 (market-position.md)](/market-position.md) — 跑酷品类头部地位、创梦天地发行护城河与主流竞品差异化对比
- [风险与不确定性 (risks-unknowns.md)](/risks-unknowns.md) — 玩法机制老化、数值膨胀对冲、排位外挂防治与合规防沉迷挑战
- [资料来源与参考文献 (sources.md)](/sources.md) — 官方公告、应用商店、行业媒体深度报道与社区攻略汇编

## 2. 玩法与系统模块 (Systems)

- [单局跑酷与竞技对抗 (systems/session-combat.md)](/systems/session-combat.md) — 重力感应与手势避障、道具拾取、三位一体技能释放与竞技场干扰对抗
- [内容玩法与模式 (systems/content-modes.md)](/systems/content-modes.md) — 无尽经典模式、1v1/2v2 竞技排位、主题场景副本、黄金矿山与限时收集赛

## 3. 代表性实体 (Entities)

本知识库采用 `representative`（代表性实体）策略，收录了 10 个核心角色、坐骑、宠物与羽翼：

- [实体名册总览 (entities/units/_index.md)](/entities/units/_index.md) — 代表性角色与坐骑分类索引
- **核心角色（Characters）**：
  - [危险盖伊 (guy-dangerous.md)](/entities/units/guy-dangerous.md) — 经典初始探险家主角，自带护盾技能，新手入门基石
  - [莉莉丝 (lilith.md)](/entities/units/lilith.md) — 竞技场 T0 级主战角色，提升 20% 速度上限与能量节约
  - [赵云 (zhao-yun.md)](/entities/units/zhao-yun.md) — 国风三国风云限定角色，国风商业化与竞技主力
  - [比奥斯博士 (dr-bios.md)](/entities/units/dr-bios.md) — 7日签到免费赠送 A 级科幻角色，长线留存福利代表
  - [安妮 (anne.md)](/entities/units/anne.md) — 浪漫婚纱主题限定角色，主打 2v2 双人组队协同加速
- **核心坐骑（Mounts）**：
  - [年兽 (nian-beast.md)](/entities/units/nian-beast.md) — 经典中国神话春节限定坐骑，国风坐骑先驱
  - [傲狠 (ao-hen.md)](/entities/units/ao-hen.md) — 竞技场顶级干扰坐骑，30% 概率封印对手加速并自带二次护盾
- **核心宠物（Pets）**：
  - [仙灵鹤 (xian-ling-he.md)](/entities/units/xian-ling-he.md) — 首款中国神话风格宠物，提供金币与得分加成
  - [小香猪 (xiao-xiang-zhu.md)](/entities/units/xiao-xiang-zhu.md) — 生肖猪年春节签到限定萌宠，提供活动代币掉落
- **核心羽翼装备（Wings）**：
  - [花蝶梦 (hua-die-meng.md)](/entities/units/hua-die-meng.md) — 精灵翅膀羽翼装备，提供飞行姿态与 12 倍爆分加成
