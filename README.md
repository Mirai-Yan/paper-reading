# paper-reading · 论文批判性精读 Skill

一个用于 Claude 的 Agent Skill：对单篇或多篇学术文章做**结构化、批判性**精读，像一位严苛而善意的同行评审兼导师——准确重建作者的论证，挖出薄弱处与反例，并推演出可做的研究切口。对法学论文（教义学、实证、法理、比较法）有专门调校。

A Claude Agent Skill for structured, critical close reading of academic papers (single or multiple), with special guidance for legal scholarship.

## 输出结构

每次分析固定输出：

1. **一句话/一段话论点**——抓可被反驳的主张，并附一句"说人话"版
2. **问题的产生与学术对话**——问题缘起 + 学术对话地图
3. **作者的论证过程**——材料、分析方法、如何回应前人，难懂处随手翻译
4. **论证的薄弱处与反例**——按严重程度排序，先立靶再击破，每条配具体反例
5. **向深处推演：新问题与可能的创新切口**
6. **跨文本综合**（仅多篇时）——对话结构、演进脉络、共同盲区
7. **金句索引**——带可回查位置的关键句，区分"可支持引用"与"可作批评对象"

## 使用方式

输入 `/reading`，或上传/粘贴论文并说"帮我精读这篇""这组文献在对话什么""找找这篇的漏洞"等。

## 安装

- **Claude.ai / Claude 应用**：将本仓库打包为 zip（保留 `paper-reading/` 文件夹结构），在设置的 Skills 中上传。
- **Claude Code**：将本文件夹放入 `~/.claude/skills/paper-reading/`（个人）或项目内 `.claude/skills/paper-reading/`。

## 文件

```
paper-reading/
├── SKILL.md                              # 主指令
└── references/
    └── critical-reading-toolkit.md       # 系统化"挑刺"清单
```

## License

MIT — 见 [LICENSE](LICENSE)。
