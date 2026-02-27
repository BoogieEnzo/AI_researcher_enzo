# AI Researcher Enzo

一个基于 MCP 工具链的**自动化文献综述助手**。  
目标：给一个研究主题，让 AI 自动帮你完成“找论文 → 看论文 → 写综述”的大部分工作。

---

## 1. 适合谁？

- 做科研 / 写课程论文的学生、工程师、研究员
- 想快速做一篇“某个方向的相关工作综述”
- 已经有一点命令行基础，能装 Python / Node / Zotero

---

## 2. 功能一览

- **自动检索开源论文**：通过 `arxiv-mcp-server` 搜 arXiv
- **补充学术搜索**：通过 `openalex-mcp` 访问 OpenAlex（2.4 亿+ 文献）
- **读取你自己的文献库**：通过 `zotero-mcp` 访问 Zotero（含闭源期刊）
- **生成结构化输出**：
  - `example/papers_summary.md`：论文摘要汇总
  - `example/IMPLEMENT.md`：综述大纲 / 框架
  - （后续可扩展 `literature_review.md`：综述正文）

---

## 3. 安装前提

本项目假设你已经具备：

- **Python** ≥ 3.9
- **Node.js** ≥ 18
- **OpenCode**（1.2+，支持 MCP，`opencode` 命令可用）
- （可选）**Zotero** + API Key（如果要访问闭源期刊）

---

## 4. 安装步骤

1. **克隆本仓库**

git clone https://github.com/yourname/AI_researcher_enzo.git
cd AI_researcher_enzo
