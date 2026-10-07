# 游戏 Wiki 研究与受控写入协议

最后验证：2026-10-07。该文件由任务装配为沙箱 `.agents/AGENTS.md`，研究和核验脚本均在 Agent 沙箱执行。

## 研究

先读 `index.md`、现有主题正文，以及已有 `manifest.md` / `coverage.md` 的覆盖线索。
保留有依据的既有内容，优先补系统规则、资源用途、养成路径、玩法关系、版本与活动条件的缺口。
机制研究读 `game-mechanics-research`；版本与活动读 `version-liveops-research`。
检索结果只是线索，必须读取对应网页正文；摘录保留对象、数字、单位、否定和适用限制。
多来源共同支持一个结论时，每个 URL 提交自己的摘录；来源身份高不代表正文支持任何结论。
版本未知不得当成当前版本；有冲突或读不到正文时，保留诊断结果，不编造事实。

## 文档与引用

正式文档路径由受控工具检查，正文使用自由 Markdown：段落、列表、表格、图均可。
不强制 frontmatter、game_id 字段、固定表头、row_id、核验状态列或来源列。
每项游戏事实在内容末尾放可点击证据链接，多来源允许多个链接。
图的关系也须有对应证据，不能用整节几个引用替代逐项支持关系。
`game_id` 是任务和工具元数据，不是正文必填字段。

Source 由工具维护 `sources/evidence.md`，固定五列：

| 证据编号 | 原文 URL | 原文摘录 | 支持的内容 | 核验记录 |
| --- | --- | --- | --- | --- |

证据编号是 UTF-8 编码 `json.dumps([url, reference], ensure_ascii=False, separators=(",", ":"))` 的 MD5。
同 URL 与摘录复用同证据；新结论仍须核验，保留此前已核验的支持内容。
多来源联合核验时，支持内容注明联合证据组；单条来源不冒充独立证明整个全文。
链接锚点为 `ev-<MD5>`。MD5 只解决身份与去重，不证明知识正确。
不手写 Source、核验记录或已核验正文，不创建 sources.md 索引、pending-claims.md 或 risks-unknowns.md 等过程文档。
现有旧文件与线索先保存，迁移没有完成前不得直接删除或宣称全库已核验。

## 唯一写入入口

通过 `code_execution` 执行沙箱 `tools/submit_evidence.py submit --request <JSON路径>`。
工具读取原文件字节，检查路径、来源和引用，独立 Firecrawl 抓取，然后一次 JEV 两问：
引用是否忠实各自网页；候选全文是否被对应引用完整支持。
两问通过才写入同一份冻结 Markdown、Source 和记录，并选择性提交推送 GitHub。
这是脚本流程，不是产品后台重复核验，也不注册 function。

输入：`game_id`、游戏目录相对路径 `file`、完整 `markdown`、`expected_sha256`、`sources`、`scope`。
已有文件的 expected_sha256 来自原始字节 SHA256；新文件填 null。
正文引用用相对链接 `[证据](sources/evidence.md#ev-<MD5>)`；位于子目录时按实际位置调整相对路径。
不要提交 request_id、row、expected_paragraph、source_id 或另一份 content。
候选全文包含所有保留事实及其来源，不为降低预算而删除有效旧知识。

退出码 0 表示本次写入和推送完成；1 表示核验不通过；2 表示输入、抓取、配置、目标变化或发布错误。
脚本 stdout 一次 JSON，按固定原因修正或补足证据后重新输入；Noul 不生成解释文字。
失败不得手动写正文，不得改原文凑通过；技术错误也不证明旧知识错误。
目标变化时重新读取最新正文和摘要，重新核验；不自动合并、强推或 git add .。
工具缺失时停止发布并报告，不能退回普通编辑工具手写。

## 边界

AGENTS 与技能是调用指导，不等于写权限隔离；不能宣称 Agent 无法绕过。
不匹配 shell 中脚本名称来证明安全，不增加命令黑名单、站点特例、数字池或日期豁免。
旧 OKF / mechanics / liveops 校验脚本仅用于历史格式审计，不注入新任务、不作为新正文 Schema 门禁。
实际部署、Trigger 重建、真实抓取 / JEV / GitHub 回读分别验收，代码合入不等于这些已完成。
