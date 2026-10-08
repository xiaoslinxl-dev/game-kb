# 游戏知识库维护规范

运行协议维护源为 GameplayGraph 的 `backend/app/agents/llm_wiki/AGENTS.generate.md`，任务将它注入为 `.agents/AGENTS.md`。本文件同步供知识库维护者阅读。最后核对：2026-10-08。

## 目标与分工

根据任务指定的游戏和主题，研究系统规则、资源用途、养成、玩法关系、商业化和版本运营，写成可追溯原文的知识。
Agent 负责检索、阅读和组织候选正文；统一工具负责核验、正式写入与 GitHub 发布。
机制研究使用 `game-mechanics-research`，版本运营使用 `version-liveops-research`，公众号检索使用 `gzh-search-crawler`，文档整理使用 `okf`。

## 研究与编写

1. 阅读游戏 `index.md` 和相关主题，已有内容用于发现缺口。已有 `manifest.md` / `coverage.md` 可作线索。
2. 明确本轮要回答的问题，再实际使用 `google_search` 查资料、`url_context` 阅读原文。仅有检索标题或摘要不足以写入事实。
3. 从原文整理对象、数值、单位、前置条件、时间及版本/地区/平台范围。区分直接规则、作者经验和自己的归纳；未知明确标注。
4. 组织完整候选 Markdown。保留有来源支持的有效知识，不靠缩成概览或只补格式完成研究。
5. 每项事实或图中关系在对应说明末尾引用来源；同一事实可由多个来源共同支持。

只改格式、重验旧稿和新增机制研究是不同结果，任务报告应说明实际完成哪一种。

## 知识库结构

所有游戏知识放在 `games/<game_id>/`。按主题组织，按任务需要研究和更新，不为空缺主题生成占位稿。
目录与引用规则以本协议为准；研究 Skill 提供知识收集建议，OKF 提供候选文档整理方法。

| 文档 | 知识范围 |
| --- | --- |
| `index.md` | 导航，链接实际存在的主题和专篇 |
| `overview.md` | 游戏定位、玩家目标、主要玩法与整体构成 |
| `core-loop.md` | 玩家行动、投入与产出、资源用途、成长解锁及返回玩法的关系 |
| `economy.md` | 资源获取、用途、供需、上限与刷新规则 |
| `progression.md` | 成长对象、前置条件、成本、收益与阶段路径 |
| `monetization.md` | 商品、价格、购买条件及其影响的资源或成长环节 |
| `social-liveops.md` | 社交协作、竞争及持续运营规则 |
| `versions.md` | 版本索引、变化与适用范围 |
| `live-events.md` | 活动参与、时间、奖励、兑换与回收规则 |
| `market-position.md` | 有来源的产品定位与市场信息 |

专篇使用工具允许的路径：

- `systems/`：`session-combat.md`、`base-build.md`、`territory-war.md`、`matchmaking.md`、`exploration.md`、`content-modes.md`。
- `versions/<版本标识>.md`：具体版本资料；`revisions/<主题>/<修订标识>.md`：主题历史规则，主题取上述根主题或系统专篇。
- `entities/index.md`、`entities/units/_index.md`、`entities/units/<实体标识>.md`：实体入口与专篇。
- `analysis-data/`：`stage-economy.md`、`progression-costs.md`、`combat-observations.md`、`purchase-comparisons.md`，保存有依据的分析数据与观察条件。

实际路径准入由统一工具检查。资料中明确的游戏版本与规则修订标识分别记录；版本未知就说明未知，不按抓取日期推定。资料明确表明规则变化时保留相应历史范围，不混成一套当前规则。
已有 `manifest.md` / `coverage.md` 可供发现缺口；未解决问题在任务结果报告，不新建来源索引、疑点或风险过程文档。

正文使用自由 Markdown，可按内容选择段落、列表、表格或图。概念文档遵循 OKF：YAML 头部只有 `type` 必填，其余按需填写。
`index.md` 是导航，不加概念文档的 `type`；OKF 脚本只整理临时候选，正式目录由统一工具维护。
正文用简体中文；图中事实关系在对应说明中引用来源，归纳说明依据与适用范围。

## 来源与引用

这里的“来源”指 URL 对应的原始资料。“引用原文”是从资料中选出的实际文字片段，须保留会影响含义的条件和上下文。
“来源编号”标识 URL 与引用原文这一对；“核验记录”保存本次完整候选、所用来源和判断结果。
正文通过来源编号链接到 `sources/evidence.md`，再从台账查看 URL、引用原文及核验记录。

引用写法：`某玩法每周刷新。[@来源](sources/evidence.md#ev-<MD5>)`。
子目录中的文档按位置调整相对路径。表格同样在相关内容末尾放来源链接，不另加来源或核验状态列。
来源编号为 UTF-8 编码 `json.dumps([url, reference], ensure_ascii=False, separators=(",", ":"))` 的 MD5。
同 URL 与引用原文复用编号；新的正文仍需重新核验。MD5 只用于引用和去重，不代表真实或可靠。

来源台账由工具维护，固定四列：编号、原文 URL、原文摘录、核验记录。台账保留原文与核验链接，知识正文保存在知识文档和核验记录中。
Agent 在临时目录准备候选和来源，不直接编辑正式正文、台账、核验记录或工具文件。

## 统一核验与发布

通过 `code_execution` 调用：

```bash
python3 /tools/submit_evidence.py submit --request /tmp/wiki-candidate.json --repo-root /workspace/game-kb
```

请求 JSON 使用当前字段：

| 字段 | 含义 |
| --- | --- |
| `game_id` | 任务指定的游戏目录名称 |
| `file` | 游戏目录内的目标文档相对路径 |
| `markdown` | 完整候选正文，包括 OKF 头部和来源引用 |
| `expected_sha256` | 现有文件原始字节的 SHA256；新文件填 `null` |
| `sources` | 1–5 项来源，每项为 `{"url": "原文地址", "reference": "引用原文"}` |
| `scope` | 可选的字符串键值对象，例如 `{"region": "CN"}`；未知可省略或填 `{}` |

工具独立用 Firecrawl 抓取每个 URL，定位引用段落及必要上下文，再由 JEV 判断：引用是否忠实各自原文，完整候选是否得到对应来源联合支持。
定位只减少送审材料，不等于核验通过。两项通过后，工具写入同一份候选、台账和记录，提交并推送 GitHub。

退出码 `0` 表示写入与推送成功，`1` 表示未通过，`2` 表示输入或执行错误。stdout 返回一次 JSON。
未通过时按原因补充原文或修正无依据的外推；目标变化时读取最新文件和摘要后重提；技术失败不代表旧知识错误。
Noul 返回分数而不生成解释，Agent 的诊断只能标为推测。相同输入重复评分不能代替实质修订。
任务结果列出实际发布文件、完成的研究问题、未解决项和失败原因；发布成功不代表主题研究完整。

## 运行边界

前置文件 Hook 拒绝直接修改 `/workspace/game-kb`、`/tools`、`/.agents`，返回统一入口提示；临时候选可以编辑。
Hook 只拦容器文件工具，任意代码执行与直接 GitHub API 写入尚未隔离；按约定所有正式写入仍使用统一入口。
工具或配置不可用时停止发布并报告。沿用工具的路径、输入预算和判断门槛，不通过修改工具或规则获得通过。
