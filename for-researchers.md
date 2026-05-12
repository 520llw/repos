# 面向科研学生的 Claude Code 工具箱

> 整理日期：**2026-05-12**
> 适用画像：日常用 Claude Code 做**科研 + 写论文 + 跟前沿**的研究生 / PhD。
> 目标：用最少的安装/配置，把"读文献 → 跑实验 → 画图 → 写论文 → 引用核对 → 出 slides/poster"整条链路 agent 化。
>
> 阅读顺序建议：先看 §1 推荐组合套装 → 按 §2 配 MCP（拿到学术数据源）→ 按 §3 装 Skill（拿到行为模板）→ 按 §4 选 PDF/RAG 工具（消化文献）→ §5 写作与发表 → §6 数据分析 → §7 一周工作流示例。

---

## 1. 推荐"开箱即用"组合（懒人版）

如果只挑 3 个仓库装，我会按下面这个顺序：

1. **K-Dense-AI / claude-scientific-skills** —— 一整套"研究 / 科学 / 工程 / 分析 / 金融 / 写作"现成 Agent Skills，开箱即用，对接 Claude Code / Codex / Gemini CLI。
   https://github.com/K-Dense-AI/claude-scientific-skills
2. **54yyyu / zotero-mcp** —— 把**本地 Zotero 库**直接接到 Claude，对 PDF 做摘要、提注释、向量相似搜索、写综述时按主题召回。
   https://github.com/54yyyu/zotero-mcp
3. **openags / paper-search-mcp** —— 一个 MCP 就能同时搜 arXiv / PubMed / bioRxiv / medRxiv / Google Scholar / Semantic Scholar / Crossref / OpenAlex / PMC / Europe PMC / dblp / OpenAIRE / CiteSeerX / SSRN / Zenodo / HAL / Unpaywall 等 **20+ 学术源**。
   https://github.com/openags/paper-search-mcp

> 这三个加起来覆盖："拿数据 + 管文献 + 执行任务模板"。

如果还想再加 2 个，按写作需求二选一：

- 写中文/通用论文 → **kgraph57 / paper-writer-skill**（IMRAD 全流程 + 引用管理 + 质量 checklist）
- 写 ML/CV/NLP 顶会论文 → **Master-cai / Research-Paper-Writing-Skills**（彭思达老师笔记适配版）

---

## 2. 学术数据 MCP（必装）

| MCP | 用途 | 链接 |
|---|---|---|
| **paper-search-mcp** (openags) | 一站搜 arXiv / PubMed / bioRxiv / medRxiv / Scholar / Semantic Scholar / Crossref / OpenAlex / PMC / Europe PMC / dblp / OpenAIRE / CiteSeerX / SSRN / Zenodo / HAL / Unpaywall 等 20+ 源 | https://github.com/openags/paper-search-mcp |
| **zotero-mcp** (54yyyu) | 接本地/网页 Zotero 库；做总结、读注释、对全库做向量相似检索 | https://github.com/54yyyu/zotero-mcp |
| **arxiv-mcp-server** (blazickjp) | 专门针对 arXiv 的精细化检索 & 分析；可顺着 Semantic Scholar 拉引用网络 | https://github.com/blazickjp/arxiv-mcp-server |
| **semantic-scholar-fastmcp-mcp-server** (zongmin-yu) | 16 个工具：论文 / 作者 / 引文网络的细粒度访问 | https://github.com/zongmin-yu/semantic-scholar-fastmcp-mcp-server |
| **akapet00 / semantic-scholar-mcp** | 同上，备选实现 | https://github.com/akapet00/semantic-scholar-mcp |
| **francojc / mcp-research** | 多源书目检索 + 自动把发现的论文写回 Zotero（带智能 tag） | https://github.com/francojc/mcp-research |
| **citecheck** (arXiv 论文实现) | 投稿前自动校验和修复参考文献：跨 PubMed / Crossref / arXiv / Semantic Scholar 多源校验 | https://arxiv.org/html/2603.17339 |
| **github-mcp-server** (官方) | 仓库 / Issue / PR / Actions / 代码搜索；和实验代码协作必备 | https://github.com/github/github-mcp-server |

**最小套装**：`paper-search-mcp` + `zotero-mcp` + `citecheck` + `github-mcp-server`。

---

## 3. Skill 包：研究 → 写作 → 投稿全流程

### 3.1 综合型（一次装满）

| 仓库 | 看点 |
|---|---|
| **K-Dense-AI / claude-scientific-skills** | 现成 Agent Skills 大全，覆盖科研 / 工程 / 分析 / 写作；与 Claude Code / Codex / Gemini CLI 兼容 |
| **K-Dense-AI / claude-scientific-writer** | "深度研究 + 写作"二合一：实时文献检索 + 可验证引用，产出论文 / 报告 / 海报 / 基金书 / 综述 |
| **Galaxy-Dawn / claude-scholar** | 半自动研究助理；跨 ideation / coding / experiments / writing / publication |
| **flonat / claude-research** | 48 个 PhD 工作流 skill：`/proofread`、`/latex-autofix`、`/literature`、`/bib-validate`、`/code-review` 等 |
| **Imbad0202 / academic-research-skills** | 12-agent 论文写作系统：风格校准 / 质量检查 / LaTeX 加固 / 可视化 / 改稿教练 / 引用转换 / 防 leak / VLM 配图核对 |
| **delibae / claude-prism** | **离线优先**的科学写作工作台：LaTeX + Python + 100+ 科学 skill，全部本地跑（断网友好）|
| **pedrohcgs / claude-code-my-workflow** | 学术模板：LaTeX/Beamer + R + 多 agent review + 质量门 + 对抗式 QA + 复现协议（已被用来跑出 800+ 页博士课件）|

### 3.2 文献综述 / 深度调研

| 仓库 | 看点 |
|---|---|
| **lingzhi227 / agent-research-skills** | 31 个 skill 覆盖全研究生命周期：从文献检索到 slides；含 GitHub repo 调研 |
| **Weizhena / Deep-Research-skills** | 结构化深度调研 skill，**人在回路**控制流程 |
| **Imbad0202 / academic-research-skills** | 6 阶段系统综述：frontier → survey → deep dive → code → synthesis → report；含 7 个脚本处理搜索 API / PDF / 数据库 / BibTeX / 报告 |

### 3.3 论文写作

| 仓库 | 看点 |
|---|---|
| **kgraph57 / paper-writer-skill** | Claude Code 全流程论文写作：IMRAD 结构、文献管理、质量 checklist |
| **Master-cai / Research-Paper-Writing-Skills** | ML / CV / NLP 顶会论文专用，彭思达老师公开笔记改编，适配 Codex / Claude Code / Gemini |
| **yunshenwuchuxun / latex-paper-skills** | 模块化 LaTeX 论文写 / 改 / 管理 |
| **ndpvt-web / latex-document-skill** | 通用 LaTeX skill：27 模板 + 27 自动化脚本 + 26 参考；自动 BibTeX 抓取、PDF 可视核对、引用交叉检查、图表计数；模板覆盖论文 / 简历 / 学位论文 / 课件 / 作业 / 海报 / slides |

### 3.4 演讲 / 海报 / Slides

| 仓库 | 看点 |
|---|---|
| **Gabberflast / academic-pptx-skill** | 学术 PPT skill：强制 action title、结构化论证、图表纪律、引用标准、沟通优先；与 Anthropic 内置 PPTX skill 协作 |
| **K-Dense-AI / claude-scientific-writer** 内置 | `latex-posters`、`scientific-slides` 子 skill |

### 3.5 学科专用

- **christopherkenny / skills** —— 政治学者 Claude Skills（统计 / 复制 / 写作）
- 经济学 / 因果推断 → **pedrohcgs / claude-code-my-workflow**

---

## 4. PDF 读取 / 论文消化（与 Skill 互补）

| 工具 | 适合谁 |
|---|---|
| **Future-House / paper-qa**（PaperQA2）| 想要"高准确率 + 带引用的 RAG"问答系统；面向科学文献调优过 |
| **khoj-ai / openpaper** | 想要"网页 + AI 注释 + 引用管理 + 音频摘要"一体化阅读器 |
| **WangQrkkk / PaperQuay** | 桌面优先文献管理器；PDF 阅读 / 翻译 / 概览 / Agent 工作流；可选 Zotero 兼容 |
| **GROBID** (`kermitt2/grobid`) | 学术 PDF → 结构化 XML/TEI，最稳的生产级解析器（ResearchGate、Mendeley、CERN 都在用）|
| **Nougat** (Meta) | 公式 / 数学密集型 PDF 的 OCR |
| **Filimoa / open-parse** | 给 LLM 用的文件解析改进版 |
| **allenai / science-parse** | AllenAI 出品，结构化抽取 |

**典型组合**：`GROBID 解析 → paper-qa 索引 → Claude + zotero-mcp 调用问答`。

---

## 5. 写作 / 引用 / 投稿专项

- **引用核对**：`citecheck` MCP（跨 PubMed / Crossref / arXiv / Semantic Scholar 自动校验、修补 DOI/URL）+ `flonat/claude-research` 中的 `/bib-validate`、`/check-refs`。
- **LaTeX 自动修**：`flonat/claude-research` 的 `/latex-autofix`；或 `ndpvt-web/latex-document-skill` 的 PDF 视觉核对脚本。
- **图表配图核对**：`Imbad0202/academic-research-skills` 的 **VLM 配图验证**（防止"图说不一致"）。
- **防数据/答案泄漏**：同上的 anti-leakage protocol，适合写 benchmark 论文时用。
- **学位论文 / 大综述长文档**：`pedrohcgs/claude-code-my-workflow`（多 agent review + 复现协议）。

---

## 6. 数据分析 / 实验代码 / 复现

| 仓库 | 看点 |
|---|---|
| **nimrodfisher / data-analytics-skills** | 数据分析任务的 Claude skill 大全 |
| **K-Dense-AI / claude-scientific-skills** | 包含统计 / 数据处理 / 可视化 skill |
| **rohitg00 / awesome-claude-code-toolkit** 中 `agents/data-ai/data-scientist.md` | 数据科学 agent profile |
| **Reproducible-Science-Curriculum / data-exploration-RR-Jupyter** | 可复现 Jupyter 探索性分析的课程级范例 |

**强烈建议在仓库根目录放一份 `CLAUDE.md`**：写清你的数据规范（路径 / 列名 / 单位 / seed / 输出位置）、可视化规范（DPI、配色、字号、subplot 风格）、实验目录约定。Claude Code 会每轮自动加载这份文件，等于给所有 skill 装了"实验室手册"。

---

## 7. 一周工作流示例（怎么把这些串起来）

```
周一  跟前沿
  └─ paper-search-mcp 拉本周新论文 → claude-scholar 自动分类
  └─ paper-qa 批量摘要 → 5 条候选导入 Zotero
  └─ zotero-mcp + Deep-Research-skills 选题深挖

周二  实验 / 代码
  └─ github-mcp-server 拉相关 repo → claude-scientific-skills 跑复现
  └─ data-analytics-skills 处理数据 → 出第一版图

周三  写作 introduction
  └─ paper-writer-skill / Research-Paper-Writing-Skills 起草
  └─ /literature （flonat/claude-research）拉证据 + 自动 cite

周四  实验 + 修图
  └─ academic-research-skills VLM 配图核对
  └─ /latex-autofix 修编译错误

周五  自检 + slides
  └─ citecheck 校验全部引用、补 DOI
  └─ academic-pptx-skill 出组会 slides
```

---

## 8. 安装与最小配置示例

> 下面是大致流程，具体以各仓库 README 为准（部分仓库自带 `install.sh` 或 `claude plugin add` 命令）。

```bash
# 1. 在你的项目里建 .claude/ 目录
mkdir -p .claude/skills && cd .claude/skills

# 2. 装 skill 包（多数 skill 就是文件夹，clone 进去即可）
git clone https://github.com/K-Dense-AI/claude-scientific-skills
git clone https://github.com/flonat/claude-research
git clone https://github.com/kgraph57/paper-writer-skill
git clone https://github.com/ndpvt-web/latex-document-skill

# 3. 配置 MCP server（写到 ~/.claude/settings.json 或项目 settings.json）
# 示例（伪代码，参数以官方 README 为准）：
# {
#   "mcpServers": {
#     "paper-search": { "command": "uvx", "args": ["paper-search-mcp"] },
#     "zotero":       { "command": "uvx", "args": ["zotero-mcp"], "env": { "ZOTERO_API_KEY": "..." } },
#     "arxiv":        { "command": "uvx", "args": ["arxiv-mcp-server"] },
#     "github":       { "command": "uvx", "args": ["github-mcp-server"] }
#   }
# }

# 4. 在项目根写一份 CLAUDE.md（实验室手册）：
#    - 数据规范 / 实验目录 / 绘图风格 / 引用 style / 写作语言
```

---

## 9. 进一步深读 / 来源

- [GitHub: K-Dense-AI/claude-scientific-skills](https://github.com/K-Dense-AI/claude-scientific-skills)
- [GitHub: K-Dense-AI/claude-scientific-writer](https://github.com/K-Dense-AI/claude-scientific-writer)
- [GitHub: Galaxy-Dawn/claude-scholar](https://github.com/Galaxy-Dawn/claude-scholar)
- [GitHub: flonat/claude-research](https://github.com/flonat/claude-research)
- [GitHub: Imbad0202/academic-research-skills](https://github.com/Imbad0202/academic-research-skills)
- [GitHub: lingzhi227/agent-research-skills](https://github.com/lingzhi227/agent-research-skills)
- [GitHub: Weizhena/Deep-Research-skills](https://github.com/Weizhena/Deep-Research-skills)
- [GitHub: kgraph57/paper-writer-skill](https://github.com/kgraph57/paper-writer-skill)
- [GitHub: Master-cai/Research-Paper-Writing-Skills](https://github.com/Master-cai/Research-Paper-Writing-Skills)
- [GitHub: yunshenwuchuxun/latex-paper-skills](https://github.com/yunshenwuchuxun/latex-paper-skills)
- [GitHub: ndpvt-web/latex-document-skill](https://github.com/ndpvt-web/latex-document-skill)
- [GitHub: delibae/claude-prism](https://github.com/delibae/claude-prism)
- [GitHub: pedrohcgs/claude-code-my-workflow](https://github.com/pedrohcgs/claude-code-my-workflow)
- [GitHub: Gabberflast/academic-pptx-skill](https://github.com/Gabberflast/academic-pptx-skill)
- [GitHub: christopherkenny/skills](https://github.com/christopherkenny/skills)
- [GitHub: openags/paper-search-mcp](https://github.com/openags/paper-search-mcp)
- [GitHub: 54yyyu/zotero-mcp](https://github.com/54yyyu/zotero-mcp)
- [GitHub: blazickjp/arxiv-mcp-server](https://github.com/blazickjp/arxiv-mcp-server)
- [GitHub: zongmin-yu/semantic-scholar-fastmcp-mcp-server](https://github.com/zongmin-yu/semantic-scholar-fastmcp-mcp-server)
- [GitHub: akapet00/semantic-scholar-mcp](https://github.com/akapet00/semantic-scholar-mcp)
- [GitHub: francojc/mcp-research](https://github.com/francojc/mcp-research)
- [arXiv: citecheck MCP server](https://arxiv.org/html/2603.17339)
- [GitHub: Future-House/paper-qa](https://github.com/Future-House/paper-qa)
- [GitHub: khoj-ai/openpaper](https://github.com/khoj-ai/openpaper)
- [GitHub: WangQrkkk/PaperQuay](https://github.com/WangQrkkk/PaperQuay)
- [GitHub: kermitt2/grobid](https://github.com/kermitt2/grobid)
- [GitHub: Filimoa/open-parse](https://github.com/Filimoa/open-parse)
- [GitHub: allenai/science-parse](https://github.com/allenai/science-parse)
- [GitHub: nimrodfisher/data-analytics-skills](https://github.com/nimrodfisher/data-analytics-skills)
- [GitHub: rohitg00/awesome-claude-code-toolkit](https://github.com/rohitg00/awesome-claude-code-toolkit)
- [GitHub: Reproducible-Science-Curriculum/data-exploration-RR-Jupyter](https://github.com/Reproducible-Science-Curriculum/data-exploration-RR-Jupyter)
- [Claude Code & Cowork for Academic Research — March 2026 Update](https://cornwl.github.io/files/claude-academic-guide.html)
- [Claude Code for Scientists — Patrick Mineault](https://www.neuroai.science/p/claude-code-for-scientists)
- [Claude Code Academic Workflow — psantanna.com](https://psantanna.com/claude-code-my-workflow/)
