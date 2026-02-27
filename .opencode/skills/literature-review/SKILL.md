---
name: literature-review
description: 自动化文献综述工作流 - 从论文搜索到综述生成
---

# 文献综述工作流

## 快速开始

1. 用户提供研究主题
2. 搜索论文（arXiv + Semantic Scholar + OpenAlex）
3. 筛选核心论文（4-8 篇）
4. 下载 PDF
5. 生成框架 IMPLEMENT.md
6. 撰写初稿 literature_review.md
7. 人工审核

## 7 阶段工作流

### Phase 1: 项目初始化
- 创建 IMPLEMENT.md 框架
- 创建 literature_review.md 初稿

### Phase 2: 文献收集

**数据源：**

| 来源 | 用途 | 工具 |
|------|------|------|
| arXiv | 最新 DL 方法、预印本 | arxiv_search_papers |
| Semantic Scholar | 学术论文+引用分析 | semantic-scholar_search_papers |
| OpenAlex | 学术论文搜索 | openalex_search_works |

**搜索策略：**
```
Query: "[topic] AND (deep learning OR neural network OR transformer)"
Categories: cs.AI, cs.LG, cs.OS, cs.DC
Date: 最近 2-3 年
```

### Phase 3: 论文筛选

1. 收集 20-50 篇相关论文
2. 按标题/摘要筛选
3. 人工确认 4-8 篇核心论文
4. 创建文献矩阵：

| 类别 | 子类 | 关键论文 | 数量 | 来源 |
|------|------|----------|------|------|
| 方法 | CNN | [refs] | N | arXiv |
| 方法 | Transformer | [refs] | N | arXiv |

### Phase 4: 提取信息

提取每篇论文：
- 标题、作者、年份
- 摘要要点
- 核心方法
- 性能数据

### Phase 5: 生成框架

基于 IMPLEMENT.md 模板生成结构：
- 标题
- 摘要
- 引言
- 主体章节（2-4 章）
- 结论
- 参考文献

### Phase 6: 撰写初稿

**写作规范：**
- 谨慎语言：may, suggests, appears to
- 避免绝对：不说 "X is the best"
- 每句引用：每个 claim 需要 reference

**标准结构：**
```markdown
# [标题]

## 摘要

## 1. 引言
### 1.1 研究背景
### 1.2 研究意义

## 2. [主体章节 1]

## 3. [主体章节 2]

## 4. 结论与展望

## 参考文献
```

### Phase 7: 人工审核

- 检查事实准确性
- 验证引用
- 格式调整

## MCP 工具

- `arxiv_search_papers` - 搜索 arXiv 论文
- `arxiv_download_paper` - 下载 PDF
- `semantic-scholar_search_papers` - 搜索学术论文
- `openalex_search_works` - 搜索 OpenAlex

## 目录结构

```
~/AI_researcher_enzo/
├── AGENTS.md
├── IMPLEMENT.md
├── papers_summary.md
├── literature_review.md
├── papers/
│   └── *.pdf
└── .opencode/
    └── skills/
        └── literature-review/
            └── SKILL.md
```
