# game-kb

游戏竞品分析 LLM-Wiki 知识库。一游戏一目录，Git 提交历史为变更权威源。

## 目录结构



## 知识准入与受控写入

知识库严禁直接手动修改正式文档或伪造核验状态。正式知识必须通过沙箱受控工具核验发布：

{"decision": "error", "written": false, "reason_codes": ["INPUT_ERROR: 请求文件不可读或不是合法JSON"], "next_action": "核对输入或执行环境后重新提交"}

每次提交通过 Firecrawl 独立抓取和 JEV 双问判断（引用忠实性 + 正文完整支持）后，自动写入正文、证据台账及审计记录并发布至 GitHub main 分支。
