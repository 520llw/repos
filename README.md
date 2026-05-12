# 近三个月 GitHub 热门仓库汇总（2026.02 – 2026.05）

> 📌 **个人化清单**：如果你是科研学生 / 论文写作场景，直接看 [`for-researchers.md`](./for-researchers.md)（精选 Skill + MCP + PDF/RAG 工具 + 一周工作流）。
>
> 整理日期：**2026-05-12**
> 整理范围：最近 ~3 个月（2026 年 2 月 — 5 月）在 GitHub 上涨星显著、被多家科技博客 / 趋势聚合站（Trendshift、OSSInsight、GitHub Trending、BytebyteGo、Medium、shareuhack 等）反复提到的项目。
> 用途：作为本仓库后续研究 / 选题 / 复刻 / 写作的"原始素材池"。
>
> ⚠️ 星数来自第三方聚合（博客、月度榜单、Trending 截图），不是实时拉取，与 GitHub 实时数字可能有少量偏差；请以仓库实时为准。

---

## 目录

1. [年度爆款 / 病毒级项目](#1-年度爆款--病毒级项目)
2. [AI 编程 Agent & CLI](#2-ai-编程-agent--cli)
3. [Agent 框架 / 多智能体系统](#3-agent-框架--多智能体系统)
4. [Claude Skills / Agent Skills 生态](#4-claude-skills--agent-skills-生态)
5. [MCP（Model Context Protocol）生态](#5-mcpmodel-context-protocol生态)
6. [本地 LLM / 推理运行时](#6-本地-llm--推理运行时)
7. [图像 / 视频 / 3D 生成](#7-图像--视频--3d-生成)
8. [科研 / 论文 / 机器学习](#8-科研--论文--机器学习)
9. [写作 / 笔记 / 知识管理](#9-写作--笔记--知识管理)
10. [生产力 / 自动化 / 工作流](#10-生产力--自动化--工作流)
11. [Rust / 系统 / 数据库](#11-rust--系统--数据库)
12. [学习资源 / 教程 / 书](#12-学习资源--教程--书)
13. [本周 GitHub Trending 当日榜（抓取快照）](#13-本周-github-trending-当日榜抓取快照)
14. [观察到的宏观趋势](#14-观察到的宏观趋势)
15. [来源](#15-来源)

---

## 1. 年度爆款 / 病毒级项目

| 项目 | 类型 | 关键信息 |
|---|---|---|
| **OpenClaw** (PSPDFKit 创始人 Peter Steinberger) | 个人 AI 助理 | 2026.01 底病毒式爆红，几天内从 9k → 60k 星，3 月已突破 21 万、4 月接近 30 万星。可常驻、浏览网页、填表、跑 shell、写并执行代码、控制智能家居；**会自己写新 skill 扩展自己**。被称为"近年增速最快的开源项目"。 |
| **OpenCode** | 开源编码 Agent CLI | 2026 年 2 月 100k 星 / 250 万 月活开发者 → 4 月 147k 星 / 650 万月活；定位为 OpenAI / Gemini / DeepSeek / Ollama / Codex 等 200+ 模型的统一 CLI。 |
| **bytedance/UI-TARS-desktop** | 多模态 GUI Agent | 字节出品的"开源多模态 AI agent stack"，近期 Trending 单日 +900 星。 |
| **decolua/9router** | AI 代理路由 | "Unlimited FREE AI coding with auto-fallback"，本周冲榜单日 +900 星。 |
| **NousResearch/hermes-agent** | 个人长期记忆 Agent | "The agent that grows with you"，14.5 万星量级，单日仍 +2k。 |

---

## 2. AI 编程 Agent & CLI

> 这是过去 90 天最拥挤的赛道，**几乎每周都有新项目登榜**。

- **OpenCode** — 开源、模型无关的编码 Agent CLI（见上）。
- **Google `gemini-cli` / 终端 Agent** — 2026.04 Google 官方发布，ReAct loop + MCP 支持 + 1M 上下文。
- **OpenAI Codex（GPT-5.5 升级版）** — 2026.04 重回"最佳编码 Agent"榜单第 1。
- **millionco/react-doctor** — React 代码质量 AI 检测器（8.3k 星）。
- **rohitg00/agentmemory** — 给编码 Agent 加可持久记忆（5k 星，单日 +400）。
- **lsdefine/GenericAgent** — ~3.3K 行种子代码自演化出技能树，号称 token 消耗只有同类的 1/6。
- **Jcode** — 专攻代码生成的 Agent 套件，5 月登 Trending。
- **OpenClaw** — 见 §1（也算编码 agent，但能力远超）。

---

## 3. Agent 框架 / 多智能体系统

| 项目 | 体量 | 一句话 |
|---|---|---|
| **Langflow** | ~146k★ | 可视化拖拽搭 RAG + multi-agent。 |
| **Dify** | ~136k★ → 2026 持续涨 | 可视化 LLM app 平台，企业向。 |
| **Flowise** | ~51k★ | 老牌可视化 LangChain 编排。 |
| **CrewAI** | 生产级多 Agent，角色分工，1500+ 企业采用。 |
| **MetaGPT / AutoGen / LobeHub** | 多智能体协作经典框架。 |
| **TauricResearch / TradingAgents** | 2026.05 上 Trending | 多 Agent LLM 金融交易框架。 |
| **VoltAgent/awesome-ai-agent-papers** | 论文索引 | 2026 起 AI Agent 研究论文按月分类。 |
| **caramaschiHG/awesome-ai-agents-2026** | 索引 | 300+ Agent 资源，月更。 |
| **ARUNAGIRINATHAN-K/awesome-ai-agents-2026** | 索引 | 编码 / 创意 / 语音 / 研究 / 企业五大类。 |

---

## 4. Claude Skills / Agent Skills 生态

> Anthropic 在 **2025.10 推出 Skill 格式**，**2025.12 作为开放标准发布**。
> 2026 年 2 月起 Skill 生态在 GitHub 出现**显式爆发**：Skill 现已被 Claude Code、Claude.ai、Claude API、OpenAI Codex、Cursor、Gemini CLI、Antigravity、Windsurf 同时支持。

| 仓库 | 看点 |
|---|---|
| **rohitg00/awesome-claude-code-toolkit** | "2026.02 GitHub Trending #1"。135 agents、35 skills（通过 SkillKit 桥接 40 万+）、42 commands、176+ plugins、20 hooks、15 rules、14 MCP 配置。 |
| **VoltAgent/awesome-agent-skills** | 1000+ skill，社区共建，跨 Claude Code / Codex / Cursor / Gemini CLI / Antigravity。 |
| **ComposioHQ/awesome-claude-skills** | 老牌精选 Claude Skill 索引。 |
| **travisvn/awesome-claude-skills** | 偏 Claude Code 工作流。 |
| **hesreallyhim/awesome-claude-code** | Skills + hooks + slash-commands + orchestrators + plugins 一站式。 |
| **GetBindu/awesome-claude-code-and-skills** | 社区贡献的 Skill 集合。 |
| **BehiSecc/awesome-claude-skills** | 精选 Skill 列表。 |
| **antigravity-awesome-skills** | 1200+ skill，几乎覆盖所有场景。 |
| **quemsah/awesome-claude-plugins** | 用 n8n 自动统计 Claude Code 插件采用率。 |

**Skill 是什么**：一个文件夹 + `SKILL.md`（YAML frontmatter: name / description + Markdown 指令），可附 scripts / references / assets。对 Agent 来说就是"可调用的领域专家手册"。

---

## 5. MCP（Model Context Protocol）生态

| 仓库 | 看点 |
|---|---|
| **modelcontextprotocol/servers** | 官方 MCP server 集合（首发即为 GitHub 最快趋势项目之一）。 |
| **github/github-mcp-server** | GitHub 官方 MCP server——仓库管理 / Issue & PR / Actions / 安全 / 协作。 |
| **microsoft/mcp** | 微软官方 MCP 实现目录。 |
| **modelcontextprotocol/{kotlin,csharp,typescript,rust}-sdk** | 官方多语言 SDK。 |
| **GitMCP** (gitmcp.io) | 把任意 GitHub repo 包装成 MCP server。 |
| 社区工具：MCP Hunt / Smithery / Toolbase / ToolHive | 发现 / 部署 / 管理 MCP server。 |

---

## 6. 本地 LLM / 推理运行时

- **Ollama** — 2026 突破 162k–165k 星，桌面端登陆 macOS / Windows，已成为本地推理事实标准。
- **AUTOMATIC1111 / stable-diffusion-webui** — 163k 星，老牌，仍稳。
- **llama.cpp / Open Interpreter** — 本地推理基础设施代表。
- **DeepSeek-V3** — 开源权重证明可比肩闭源旗舰；2026 本地化部署关键节点。
- **tinyhumansai/openhuman** — Rust 写的"个人 AI super intelligence"，单日 Trending +366。

---

## 7. 图像 / 视频 / 3D 生成

| 项目 | 说明 |
|---|---|
| **ComfyUI** | 2026 已破 106k 星，节点式工作流，对每一步精细控制。 |
| **HunyuanVideo** | 腾讯混元的大视频生成系统框架（~12k 星，仍在涨）。 |
| **SANA** | 线性扩散 Transformer 高分辨率合成，2026.04 ~5.1k 星。 |
| **LTX-Video** | 图→视频、文→视频扩散模型。 |
| **VideoCrafter2** | 解决高质量视频扩散的数据瓶颈。 |
| **playcanvas/supersplat** | 3D Gaussian Splat 编辑器，本周 Trending +500/天。 |
| **showlab/Awesome-Video-Diffusion / AlonzoLeeeooo/awesome-video-generation** | 视频生成论文 / 模型索引。 |

---

## 8. 科研 / 论文 / 机器学习

- **SkalskiP/top-cvpr-2026-papers** — CVPR 2026 4090 篇接收论文中精选热门 + 代码 + Demo。
- **VoltAgent/awesome-ai-agent-papers** — 2026 AI Agent 研究论文（agent engineering / memory / eval / workflow / autonomous）。
- **dair-ai/AI-Papers-of-the-Week** — 每周 ML 顶会顶刊精选。
- **aimerou/awesome-ai-papers** — CV / NLP / Audio / Multimodal / RL 五大方向按时间。
- **Engineer1999/A-Curated-List-of-Must-Read-ML-Research-Papers** — 按主题分类的必读清单。
- **rasbt / LLMs-from-scratch** — 93k 星，PyTorch 从零实现 GPT。
- **Lordog / dive-into-llms** — 37k 星，中文 LLM 教程，本周 Trending 持续上榜。
- **Hugging Face `ml-intern`** — 2026.04 发布，开源 ML 工程师 Agent，可读论文 / 训练模型 / 部署。
- 研究热点关键词：**LightRAG**（图增强 RAG）、**EvoScientist**（多 Agent 自演化科研框架）。

---

## 9. 写作 / 笔记 / 知识管理

- **AFFiNE Pro** — 一体化 notes，可写 / 画 / 排程。
- **Notesnook** — E2E 加密笔记，主打隐私。
- **Super Productivity** — 离线优先深度工作任务管理；可同步 GitHub / Jira / CalDAV。
- **OnlyOffice / Collabora 类开源在线编辑器** — 文档 / 表格 / 幻灯片 / PDF，实时协作 + AI。
- **RAGFlow** — 文档摄取 → 向量索引 → 查询规划 → 工具调用 Agent 一体的开源 RAG 引擎；写作 / 知识库场景重头。

---

## 10. 生产力 / 自动化 / 工作流

- **n8n** — 2026 破 150k 星，开源可视化自动化平台，原生 AI 节点 + 400+ 集成，自托管 fair-code。
- **Langflow / Dify / Flowise** — 见 §3，可视化 AI workflow。
- **datawhalechina/easy-vibe** — "vibe coding 2026"，面向初学者的现代编码课，本周 Trending +800/天。
- **CloakHQ/CloakBrowser** — "可过所有 bot 检测"的 Chromium 隐身浏览器，本周 +1300/天，自动化抓取热门。
- **yikart/AiToEarn** — "用 AI 赚钱"工具集，本周 +400/天。

---

## 11. Rust / 系统 / 数据库

- **SurrealDB** — 分布式文档 + 图数据库，SQL + 图遍历。
- **RustFS** — 开源 S3 兼容高性能对象存储，可与 MinIO / Ceph 共存迁移。
- **RuVector** — 高性能实时自学习向量图数据库（Rust）。
- **Apache Spark Rust 替代品（跨平台）** — 统一批 / 流 / AI 计算。
- **Yazi / Starship / WezTerm / Zellij / Nushell** — 现代终端工具链的 Rust 矩阵。
- 趋势：**本地优先 + Rust 重写经典基础设施**继续蔓延。

---

## 12. 学习资源 / 教程 / 书

- **freeCodeCamp/freeCodeCamp** — 仍是头部学习仓库。
- **EbookFoundation/free-programming-books** — 多语言免费编程书目大全。
- **rasbt/LLMs-from-scratch** — 从零造 LLM（93k★）。
- **Lordog/dive-into-llms** — LLM 编程教程（中文，37k★）。
- **microsoft/generative-ai-for-beginners** — 21 课从零做生成式 AI 应用。
- **jwasham/coding-interview-university** — 计算机科学学习路线 + 面试。
- **codecrafters-io/build-your-own-x** — 手写 X（数据库 / 编辑器 / 区块链 / OS …）。
- **CuriousLearner/Awesome-Learning** / **johnpaulada/awesome-learning-collections** — Awesome 学习索引的索引。

---

## 13. 本周 GitHub Trending 当日榜（抓取快照）

> 抓取时间：2026-05-12，仅供参考（Trending 每小时刷新）

| # | 仓库 | 语言 | 总星 | 当日涨星 | 描述 |
|---|---|---|---|---|---|
| 1 | bytedance/UI-TARS-desktop | TypeScript | 33,331 | +956 | 开源多模态 AI Agent stack |
| 2 | CloakHQ/CloakBrowser | Python | 6,850 | +1,320 | 反检测 Chromium |
| 3 | yikart/AiToEarn | TypeScript | 11,347 | +427 | 用 AI 赚钱 |
| 4 | playcanvas/supersplat | TypeScript | 7,561 | +531 | 3D Gaussian Splat 编辑器 |
| 5 | datawhalechina/easy-vibe | JavaScript | 10,263 | +812 | vibe coding 2026 教程 |
| 6 | decolua/9router | JavaScript | 8,812 | +941 | 免费 AI coding 路由 |
| 7 | tinyhumansai/openhuman | Rust | 1,868 | +366 | 个人 AI super intelligence |
| 8 | millionco/react-doctor | TypeScript | 8,331 | +212 | React AI 代码质量检测 |
| 9 | Lordog/dive-into-llms | Jupyter | 37,527 | +422 | LLM 编程教程 |
| 10 | AUTOMATIC1111/stable-diffusion-webui | Python | 162,977 | +39 | SD WebUI |
| 11 | rasbt/LLMs-from-scratch | Jupyter | 93,294 | +337 | PyTorch 从零 GPT |
| 12 | NousResearch/hermes-agent | Python | 145,790 | +2,065 | 长期记忆 Agent |
| 13 | rohitg00/agentmemory | TypeScript | 5,103 | +430 | Agent 持久记忆 |

---

## 14. 观察到的宏观趋势

1. **从"一个聊天机器人"到"一队 Agent 协作"**。本三个月几乎所有上榜 AI 项目都是 multi-agent / orchestration，纯 chatbot 几乎不再上榜。
2. **Skill 化**。Anthropic 的 Skill 格式跨平台落地（Codex / Cursor / Gemini CLI / Antigravity / Windsurf 全部支持），2026.02 起 Skill 索引仓库扎堆冲榜。
3. **MCP 成为新事实标准**。GitHub、Microsoft 都给了官方 server；任意工具/服务都在被 MCP 化。
4. **本地优先**。Ollama、DeepSeek、Open Interpreter、tinyhumansai 这一脉持续走强，"无云依赖"成为新卖点。
5. **可视化拖拽 + 代码**双轨并存。Langflow / Dify / n8n / Flowise 让非工程师也能搭 Agent 流水线。
6. **开源复刻闭源工具的周期从年缩到月**。Trending 一半以上的新晋热门是某个付费 SaaS 的开源替代。
7. **Rust 在基础设施层继续吃掉系统软件**。数据库、对象存储、终端、向量库、推理运行时新项目几乎全是 Rust。
8. **写作 / 笔记侧相对沉默**——AFFiNE、Notesnook、Super Productivity 仍是头部，但本周期没有出现"OpenClaw 量级"的写作类爆款，是潜在的研究 / 选题空白。
9. **GitHub Octoverse 2025 数据**：AI 相关 repo 已 430 万，LLM 相关 repo 年增 178%。

---

## 15. 来源

- [Top AI GitHub Repositories in 2026 — bytebytego blog](https://blog.bytebytego.com/p/top-ai-github-repositories-in-2026)
- [GitHub Trending（实时）](https://github.com/trending)
- [Top 20 GitHub Repositories for AI Agents in 2026 — Fungies.io](https://fungies.io/top-github-repositories-ai-agent-frameworks-2026/)
- [awesome-ai-agents-2026 — caramaschiHG](https://github.com/caramaschiHG/awesome-ai-agents-2026)
- [Trendshift — GitHub trending insights](https://trendshift.io/)
- [OSSInsight — Trending AI Repositories](https://ossinsight.io/trending/ai)
- [Top 12 GitHub AI Repositories Worth Your Time in 2026 — Medium / Pythonworld](https://medium.com/the-pythonworld/top-12-github-ai-repositories-that-are-actually-worth-your-time-in-2026-ca4afe2bfa8b)
- [Top 5 Trending AI GitHub Repos — May 2026 — askglitch](https://www.askglitch.com/blog/top-5-trending-ai-github-repos-may-2026)
- [What 100 Trending GitHub Projects Tell Us About Where AI Is Going — dev.to](https://dev.to/ji_ai/what-100-trending-github-projects-tell-us-about-where-ai-is-actually-going-4977)
- [awesome-opensource-ai — alvinreal](https://github.com/alvinreal/awesome-opensource-ai)
- [Best AI Coding Agents in 2026 — MightyBot](https://mightybot.ai/blog/coding-ai-agents-for-accelerating-engineering-workflows/)
- [AI-Coding-Landscape — joylarkin](https://github.com/joylarkin/AI-Coding-Landscape)
- [Top 10 Open-Source AI Projects on GitHub 2026 — BuildMVPFast](https://www.buildmvpfast.com/blog/best-open-source-ai-projects-github-2026)
- [Trending Papers — Hugging Face](https://huggingface.co/papers/trending)
- [dair-ai / AI-Papers-of-the-Week](https://github.com/dair-ai/AI-Papers-of-the-Week)
- [SkalskiP / top-cvpr-2026-papers](https://github.com/SkalskiP/top-cvpr-2026-papers)
- [VoltAgent / awesome-ai-agent-papers](https://github.com/VoltAgent/awesome-ai-agent-papers)
- [Engineer1999 / A-Curated-List-of-Must-Read-ML-Research-Papers](https://github.com/Engineer1999/A-Curated-List-of-Must-Read-ML-Research-Papers)
- [aimerou / awesome-ai-papers](https://github.com/aimerou/awesome-ai-papers)
- [ComposioHQ / awesome-claude-skills](https://github.com/ComposioHQ/awesome-claude-skills)
- [VoltAgent / awesome-agent-skills](https://github.com/VoltAgent/awesome-agent-skills)
- [travisvn / awesome-claude-skills](https://github.com/travisvn/awesome-claude-skills)
- [hesreallyhim / awesome-claude-code](https://github.com/hesreallyhim/awesome-claude-code)
- [rohitg00 / awesome-claude-code-toolkit](https://github.com/rohitg00/awesome-claude-code-toolkit)
- [quemsah / awesome-claude-plugins](https://github.com/quemsah/awesome-claude-plugins)
- [10 Must-Have Skills for Claude in 2026 — Medium](https://medium.com/@unicodeveloper/10-must-have-skills-for-claude-and-any-coding-agent-in-2026-b5451b013051)
- [Top 5 GitHub Repos for Free Claude Code Skills — Analytics Vidhya](https://www.analyticsvidhya.com/blog/2026/03/github-repositories-to-get-free-claude-code-skills/)
- [modelcontextprotocol / servers](https://github.com/modelcontextprotocol/servers)
- [github / github-mcp-server](https://github.com/github/github-mcp-server)
- [microsoft / mcp](https://github.com/microsoft/mcp)
- [GitMCP](https://gitmcp.io/)
- [Complete Guide to MCP in 2026 — dev.to](https://dev.to/universe7creator/the-complete-guide-to-model-context-protocol-mcp-building-ai-native-applications-in-2026-5e57)
- [GitHub Trending Weekly 2026-04-08 — shareuhack](https://www.shareuhack.com/en/posts/github-trending-weekly-2026-04-08)
- [8 Open-Source AI Tools for Productivity in 2026 — Medium](https://medium.com/synthetic-futures/8-open-source-ai-tools-that-will-actually-make-you-productive-in-2026-583d5ba71f81)
- [9 Open Source AI & MCP Productivity Projects — GitHub Blog](https://github.blog/open-source/accelerate-developer-productivity-with-these-9-open-source-ai-and-mcp-projects/)
- [This year's most influential open source projects — GitHub Blog](https://github.blog/open-source/maintainers/this-years-most-influential-open-source-projects/)
- [Top 20 AI Projects on GitHub to Watch in 2026 — NocoBase / Medium](https://medium.com/@nocobase/top-20-ai-projects-on-github-to-watch-in-2026-not-just-openclaw-909b3bae62f6)
- [20 Most Starred GitHub Projects (2026) — apidog](https://apidog.com/blog/top-rising-github-projects/)
- [Top 15 GitHub Projects in 2026 — dev.to](https://dev.to/ali-asghar/top-15-github-projects-every-developer-should-explore-in-2026-32o4)
- [Top 23 Trending Rust Projects (Jan 2026) — glukhov.org](https://www.glukhov.org/post/2026/01/most-popular-rust-projects-on-github)
- [OSSInsight — Top Rust](https://ossinsight.io/languages/Rust)
- [RuVector — AIToolly](https://aitoolly.com/ai-news/article/2026-02-28-ruvector-high-performance-real-time-self-learning-vector-graph-neural-network-and-database-built-wit)
- [TradingAgents — AIToolly](https://aitoolly.com/ai-news/article/2026-05-04-tradingagents-tauricresearch-launches-multi-agent-llm-framework-for-financial-trading)
- [Hugging Face ml-intern — AIToolly](https://aitoolly.com/ai-news/article/2026-04-25-hugging-face-launches-ml-intern-an-open-source-ai-agent-for-machine-learning-engineering-tasks)
- [lsdefine / GenericAgent](https://github.com/lsdefine/GenericAgent)
- [Super Productivity](https://super-productivity.com/)
- [Best Open Source Note Taking Apps 2026 — toolfinder](https://toolfinder.com/best/open-source-note-taking-apps)
- [15 Most Popular GitHub Repos 2026 — Hostinger](https://www.hostinger.com/tutorials/most-popular-github-repos)
- [10 Most Popular GitHub Repos for Learning AI — KDnuggets](https://www.kdnuggets.com/10-most-popular-github-repositories-for-learning-ai)
- [free-programming-books](https://ebookfoundation.github.io/free-programming-books/)

---

*由 Claude 在 `claude/curate-trending-repos-ElLLl` 分支上整理，作为本仓库的研究索引；后续可以按主题在此基础上拆 issue / 深挖单个仓库。*
