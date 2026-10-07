# game-kb

游戏知识库，一游戏一目录。正文按主题组织，事实末尾使用可点击的证据引用。

## 游戏目录

- [baye](games/baye/index.md)
- [dou-luo-da-lu-hun-shi-dui-jue](games/dou-luo-da-lu-hun-shi-dui-jue/index.md)
- [dou-luo-da-lu-lie-hun-shi-jie-guan-fu](games/dou-luo-da-lu-lie-hun-shi-jie-guan-fu/index.md)
- [feng-kuang-shui-shi-jie](games/feng-kuang-shui-shi-jie/index.md)
- [genshin-impact](games/genshin-impact/index.md)
- [han-shuang-qi-shi-lu](games/han-shuang-qi-shi-lu/index.md)
- [shen-miao-tao-pao-2](games/shen-miao-tao-pao-2/index.md)

## 知识写入

Agent 在沙箱中整理完整 Markdown 和来源材料，调用统一工具核验与发布：

```bash
python3 /workspace/tools/submit_evidence.py submit --request candidate.json --repo-root /workspace/game-kb
```

请求包含 `game_id`、`file`、`markdown`、`expected_sha256`、`sources: [{url, reference}]` 及可选 `scope`。来源由 Firecrawl 独立读取，JEV 判断引用忠实性与正文完整支持；两问通过后，工具写入正文、证据台账与核验记录并提交。

证据统一在各游戏的 `sources/evidence.md`。段落或表格内容末尾使用 `[@证据](sources/evidence.md#ev-<MD5>)`；子目录使用相应的相对路径。证据编号为原始 URL 与原文摘录组成的 JSON 数组的 MD5，不由 Agent 手填已通过状态。

刷新必须保留原文的研究主题，不能用一则活动替换整篇系统知识。来源不可读、证据不足或工具失败时，不发布替代稿，不把技术失败判成旧知识错误。

旧过程资料完整归档至 `.wiki_evidence/legacy/`；历史修订保持原版本含义。新台账存在不代表全部旧正文已经重新核验。
