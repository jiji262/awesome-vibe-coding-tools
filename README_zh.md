# Awesome Vibe Coding Tools ✨

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![欢迎贡献](https://img.shields.io/badge/贡献者-欢迎-brightgreen.svg?style=flat)](CONTRIBUTING.md)

> 精心整理的 AI 编程插件、IDE、开发工具与 workflow 系统列表，通过人工智能提升编程效率。

## 📋 目录

- [AI 增强型 IDE 和编辑器](#-ai-增强型-ide-和编辑器)
- [终端 AI 编程助手](#-终端-ai-编程助手)
- [VS Code 扩展插件](#-vs-code-扩展插件)
- [在线开发平台](#-在线开发平台)
- [企业级解决方案](#-企业级解决方案)
- [专业工具](#-专业工具)
- [CLI 工作流系统与增强套件](#cli-workflow-systems)
- [工作流系统与规格驱动开发](#workflow-systems)
- [多智能体编排与协作](#multi-agent-orchestration)
- [任务、记忆与工作区管理](#task-memory-workspace)
- [Skills、上下文工程与 Agent 套件](#skills-context-packs)
- [可视化工作流工具](#visual-workflow-tooling)
- [历史 / 不可用工作流参考](#historical-workflow-references)
- [贡献指南](#-贡献指南)
- [许可证](#-许可证)

## 🚀 AI 增强型 IDE 和编辑器

- **[Cursor](https://cursor.com/):** AI 优先的代码编辑器与 agent 平台，支持代码感知聊天、Composer、云端/后台 agents、automations、Jira 委派、共享 canvases，以及用于本地长运行 agents 的 `/loop`。
- **[Windsurf](https://windsurf.codeium.com/):** Codeium 的多 IDE 支持工具，具备"级联流"智能体多步骤自动化、UI 实时预览和强大的团队协作功能。特别适合快速原型开发，但在大项目中容易丢失上下文。
- **[Kiro](https://kiro.dev/):** AWS 实验性 IDE，具备规范驱动的微服务和云原生解决方案脚手架，使端到端开发和部署变得顺畅。
- **[Google Antigravity](https://antigravity.google/):** 谷歌的 agent-first development platform，包含 Antigravity 2.0 桌面端、CLI 和 SDK。可编排并行 agents、dynamic subagents、定时任务，并与 AI Studio、Android 和 Firebase 集成。
- **[腾讯云 CodeBuddy](https://cloud.tencent.com/product/codebuddy):** AI 驱动的 IDE，用于自动化前端/后端/数据库生成，集成多种 LLM 选择和 Figma 转代码功能。
- **[Trae](https://trae.ai/):** 字节跳动的自动化构建工具，同步 Figma 设计到代码，专门针对小团队的低代码原型开发。
- **[Zed](https://zed.dev/):** Rust 驱动的超高速编辑器，120fps 渲染、原生 AI 建议和强大的前端开发协作功能。
- **[通义灵码](https://tongyi.aliyun.com/lingma):** 阿里巴巴的旗舰代码助手，支持中英文、主要 IDE 和独立运行。
- **[百度 Comate](https://comate.baidu.com/):** 多语言支持，50% 真实采用率，支持所有主要 IDE 和插件，端到端开发自动化。
- **[Qoder](https://qoder.ai/):** 智能代码生成和编程助手，支持多种编程语言，提供代码补全、错误检测和智能重构功能。
- **[Crystal (Claude Code Manager)](https://github.com/stravu/crystal):** 多会话智能体管理器，Git 工作树集成，差异/合并查看器。非常适合多解决方案原型开发。
- **[Void](https://voideditor.com/):** 开源 Cursor 替代品，检查点可视化，支持任何模型/本地托管的智能体 AI，注重企业隐私。
- **[IntelliJ IDEA AI](https://www.jetbrains.com/idea/):** 企业级主流 Java IDE，原生 AI 补全，大型项目代码导航。

## 💻 终端 AI 编程助手

- **[Claude Code](https://claude.ai/code):** 具备全代码库感知，可在终端、IDE 和后台任务场景中执行智能体编辑/测试/PR 流程。Dynamic workflows 可规划大型任务、运行并行 subagents，并在汇报前验证输出。
- **[Gemini CLI](https://ai.google.dev/gemini-api/docs/cli):** 谷歌命令行旗舰产品，100万上下文，多模态聊天和强大的 Shell 脚本自动化。
- **[Aider](https://aider.chat/):** 终端 Git 集成的结对编程工具，高 Swe-bench 分数，专注于补丁和智能代码导航。
- **[Cosine CLI](https://cosine.sh/cli):** 终端中的自主 AI 工程师，具备完整的本地工具访问能力。能够像真实开发者一样规划、编写、测试和迭代。具备终端和网页之间的跨平台连续性，在真实环境中运行，可访问本地文件、构建和测试。无需切换上下文。
- **[Goose](https://github.com/Squadrick/goose):** 可扩展的开源 CLI 智能体，插件架构，多模型支持，适合分布式代码工作流。
- **[Kode](https://github.com/shareAI-lab/Kode):** 开源多模型 CLI 智能体，支持 GLM、Qwen、Kimi、DeepSeek 等。具备真正的多模型协作能力，智能任务分配、专家模型咨询（AskExpertModel 工具）和并行子代理处理。Tab 键快速切换模型，灵活分配不同用途的模型（主要、任务、推理、快速）。
- **[Factory CLI](https://factory.ai/product/ide):** 面向终端和 IDE 的 AI Droids，支持多模型（Claude、GPT、Gemini）。具备可调节的自主性级别、百万行代码库的智能搜索和跨平台上下文记忆。原生支持 VS Code、JetBrains、Vim 等，具备企业级安全性。
- **[OpenCode](https://github.com/opencodeinterpret/opencode):** 原生终端智能体，支持 LSP 和数十种 LLM。适合多语言项目和多模型集成。
- **[Warp](https://www.warp.dev/):** AI 驱动的终端，自然语言命令和智能自动补全。
- **[Codex CLI](https://openai.com/index/openai-codex/):** OpenAI 官方工具，轻量快速的终端代码生成。
- **[GitHub Copilot CLI](https://github.com/features/copilot/cli):** GitHub 的终端原生编码智能体，支持 `/plan`、后台委派、MCP/plugins/skills 与跨会话记忆。可直接从 issue 走到 PR，不用离开 shell。
- **[Crush](https://github.com/charmbracelet/crush):** Charmbracelet 的智能体，多模型和 LSP，高度可定制的终端编码。
- **[Cursor CLI](https://cursor.com/en/cli):** 与 Cursor IDE 共享上下文，支持高级实时代码审查、编写和智能体指导。
- **[Groq Code CLI](https://github.com/build-with-groq/groq-code-cli):** 可扩展插件框架，CLI 工作流自动化，完全可定制。
- **[Amp](https://ampcode.com/):** 自主推理和编辑，适合终端中的多模型和智能体代码任务。
- **[iflow CLI](https://github.com/iflow-ai/iflow-cli):** 智能工作流自动化CLI工具，为开发者提供AI驱动的任务编排和终端中的简化开发流程。
- **[Qoder CLI](https://qoder.com/cli):** Qoder 的命令行版本，将智能代码生成和 AI 编程辅助带到终端，支持多语言和智能重构功能。
- **[qwen-code](https://github.com/QwenLM/qwen-code):** 阿里云开发的终端编程智能体，生活在数字世界中。具备全代码库感知、OAuth 认证、多模型支持和强大的代码理解能力。支持代码生成、调试和重构，拥有 100 万上下文窗口和视觉模型集成。
- **[Auggie](https://augmentcode.com/cli):** Augment Code 的命令行版本，将企业级AI编程辅助带到终端，具有大上下文窗口和法规遵从性功能。

## 🔌 VS Code 扩展插件

- **[GitHub Copilot](https://github.com/features/copilot):** 覆盖 VS Code、GitHub.com、移动端和后台 coding agent 的多模型助手。支持 chat/edit/agent 模式、代码审查、模型选择和企业级治理。
- **[Cline](https://github.com/cline/cline):** 自主 AI 智能体，具备文件/网络编辑功能，完全开源可扩展，支持 CLI 模式。
- **[Continue](https://github.com/continuedev/continue):** 开源 GPT/Claude/Gemini 集成，内联代码聊天，文件/项目上下文支持，API/模型选择。
- **[RooCode](https://github.com/RooCodeInc/Roo-Code):** 智能体团队允许并发多模型自动化，高级 API 支持。
- **[KiloCode](https://github.com/Kilo-Org/kilocode):** Roo/Cline 超集，编排器模式和错误恢复，基于积分的系统，高级多智能体权限。
- **[Cody (Sourcegraph)](https://sourcegraph.com/cody):** 多仓库代码搜索，解释，自定义样式提示，支持多个主要 LLM。
- **[CodeGPT](https://codegpt.co/):** 编辑器内聊天/AI 调试，解释，代码/测试/文档生成，支持 OpenAI/Anthropic。
- **[Graphite](https://graphite.dev/):** 堆叠 PR 工作流，即时 AI 代码审查评论，侧边栏分支管理。
- **[Tabnine](https://www.tabnine.com/):** 本地部署，适应个人编码风格，适合隐私/安全优先的团队。
- **[Gemini Code Assist](https://codeassist.google/):** 深度谷歌/Colab 集成，实时代码支持。
- **[ChatGPT for VS Code](https://marketplace.visualstudio.com/items?itemName=openai.chatgpt):** 直接 OpenAI 聊天集成，支持调试/测试/文档生成。
- **[Augment Code](https://augmentcode.com/):** 20万+ 上下文令牌，针对大型企业仓库和法规遵从性进行优化，支持 SOC2 级部署。

## 🌐 在线开发平台

- **[Cosine](https://cosine.sh/):** 由 Genie 2 驱动的自主 AI 编码代理，设计用于端到端完成任务而无需人工监督。具备异步任务分配、多智能体部署，以及与 Slack、Jira、Linear 的工作流集成。在 SWE-Lancer 基准测试中达到 72%，在生产级任务中领先。
- **[v0 (Vercel)](https://v0.app/):** 自然语言转 React UI，内置 shadcn/ui，极简前端应用原型开发。
- **[Bolt.new (StackBlitz)](https://bolt.new/):** 浏览器内全栈应用创建/部署，利用 WebContainers，无需本地工具。
- **[Lovable](https://lovable.dev/):** 无代码构建器，从自然语言即时创建全栈网络应用。
- **[Replit AI Agent/Ghostwriter](https://replit.com/ai):** 浏览器 IDE，多语言编程，即时解释和错误修复，实时协作。
- **[Google AI Studio](https://aistudio.google.com/):** 由 Antigravity coding agent 驱动的 prompt-to-production 应用构建平台。支持 Firebase 后端、Workspace 集成、移动端灵感捕获、原生 Android 应用生成、Play 测试轨发布，以及导出到 Antigravity。
- **[Knack](https://www.knack.com/):** 自动化代码/数据驱动开发，针对速度/质量/团队用例优化。
- **[CodeWP](https://codewp.ai/):** WordPress 的 AI 网站构建器，端到端生成和部署。
- **[Figma Make](https://www.figma.com/):** Figma 的 AI 驱动功能，通过自然语言提示创建功能性原型和 Web 应用。自动生成前端和后端代码，并支持 Supabase 集成。
- **[Base44](https://base44.com/):** AI 驱动的无代码平台，通过自然语言对话构建 Web 和移动应用。内置数据库、认证、存储、分析和邮件功能，支持无缝外部服务集成。
- **[Conductor](https://conductor.build/):** AI 驱动的开发平台，具备自动化代码生成、错误修复和批量重构能力。集成 GitHub、GitLab、AWS CodeCommit、Azure DevOps 和 BitBucket，实现流畅工作流。
- **[Aura](https://www.aura.build/):** AI 增强的开发平台，提供实时协作、智能代码分析和自动化优化，用于构建高性能应用。
- **[Verdent](https://www.verdent.ai/):** 基于云的 AI 开发平台，专注于可持续和高效的应用开发，具备 AI 驱动的代码审查和性能优化。

## 🏢 企业级解决方案

- **[Codex (OpenAI)](https://openai.com/codex/):** 云智能体，CLI，私有部署，具备审计/安全选项的综合代码生成。
- **[Devin (Cognition)](https://devin.ai/):** 团队级自主软件工程师，端到端自动化。
- **[Replit](https://replit.com/):** 多智能体工作空间，自然语言生成，多用户协作。
- **[Jules (Google)](https://jules.google/):** 自动化拉取请求，CI/CD 和代码修复集成。
- **[Open SWE (LangGraph)](https://swe.langchain.com/):** 开源企业智能体平台，工作流可定制性。
- **[OpenHands](https://github.com/OpenHands/OpenHands):** 开源、可自托管的 AI 软件开发者平台，前身为 OpenDevin。Agents 可以编辑代码、运行命令、浏览网页，并通过 Web、CLI 和企业部署选项端到端处理软件任务。
- **[Coder Agents](https://coder.com/blog/introducing-coder-agents):** 内置在 Coder control plane 中的自托管、模型无关 coding agents。集中管理模型、提示词、工作区、用量、MCP、skills、subagents 和后台执行，可运行在客户自有基础设施上。
- **[UiPath for Coding Agents](https://www.uipath.com/developers/coding-agents):** 面向 Claude Code、Codex、Gemini CLI、Cursor 等 coding agents 的企业自动化平台层。让 agents 构建、审查、测试和治理 UiPath 自动化，并接入 RBAC、审计和策略控制。
- **[Amazon Q Developer](https://aws.amazon.com/q/developer/):** AWS 原生编码智能体，IDE 集成，云/服务支持。
- **[IBM CodeAssist](https://www.ibm.com/products/watsonx-code-assistant):** AI 驱动的大型机开发者自动化，为受监管行业量身定制。
- **[Tabnine Enterprise](https://www.tabnine.com/):** 私有云，大型团队的合规/安全。

## 🔧 专业工具

- **[RepoPrompt](https://github.com/repo-prompt/repo-prompt):** Mac 原生 AI 文件/代码管理和迭代，非常适合版本组织。
- **[DeepCode (Snyk)](https://snyk.io/product/deepcode-ai/):** AI 快速代码安全分析和可操作的修复建议。
- **[Umami](https://umami.is/):** AI 驱动的前端优化/性能分析。
- **[TraceRoot AI](https://traceroot.ai/):** 错误定位和补丁建议，自动根因分析。
- **[Chrome DevTools for agents](https://developer.chrome.com/docs/devtools/agents):** 稳定版 Chrome DevTools MCP server、CLI 和 agent skills，让 coding agents 检查真实浏览器状态、调试运行时问题、模拟用户，并在发布前运行 Lighthouse 审计。
- **[Agent QA](https://github.com/vostride/agent-qa)：** 面向自然语言 Web 与移动应用测试的源码可用 CLI 和 MCP 工具，支持执行记忆与界面适配。采用 FSL-1.1-ALv2 许可证，每个版本发布两年后转换为 Apache-2.0。
- **[Blitz](https://blitzjs.com/):** Next.js 原生 AI 插件，快速前端开发。
- **[BlackBox AI](https://blackbox.ai/):** 代码补全加安全扫描一体化。
- **[ColDeco](https://coldeco.ai/):** 可视化 AI 生成的代码检查和审查。
- **[IntelliDev](https://intellidev.ai/):** ML 驱动的终端工作流助手，用于开发/日志/任务。


<a id="cli-workflow-systems"></a>
## 🧰 CLI 工作流系统与增强套件

- **[anomalyco/opencode](https://github.com/anomalyco/opencode)：** 开源编码代理。
- **[code-yeongyu/oh-my-openagent](https://github.com/code-yeongyu/oh-my-openagent)：** OMO，最佳智能体运行框架（原 oh-my-opencode），为 OpenCode 和相关编码代理提供异步子代理、精选工具与更强的代理体验。
- **[UfoMiao/zcf](https://github.com/UfoMiao/zcf)：** 面向 Claude Code 与 Codex 的零配置代码流。
- **[Yeachan-Heo/oh-my-codex](https://github.com/Yeachan-Heo/oh-my-codex)：** OmX，为 OpenAI Codex CLI 提供 hooks、智能体团队、HUD 等增强能力。
- **[alvinunreal/oh-my-opencode-slim](https://github.com/alvinunreal/oh-my-opencode-slim)：** oh-my-opencode 的精简、清理与微调版本，显著降低 token 消耗。
- **[agent-sh/agentsys](https://github.com/agent-sh/agentsys)：** 面向 Claude Code、OpenCode、Codex、Cursor、Kiro 的自动化系统，用插件、agents 与 skills 自动化 AI 编码周边工作。
- **[zhukunpenglinyutong/ai-max](https://github.com/zhukunpenglinyutong/ai-max)：** 一键提升 Claude Code“智商”的增强套件，包含生产级 agents、skills、hooks、commands、rules 与 MCP 配置。

<a id="workflow-systems"></a>
## 🧠 工作流系统与规格驱动开发

- **[obra/superpowers](https://github.com/obra/superpowers)：** 一个真正有效的智能体技能框架与软件开发方法论。
- **[github/spec-kit](https://github.com/github/spec-kit)：** 帮助你快速开始规格驱动开发（Spec-Driven Development）的工具包。
- **[bmad-code-org/BMAD-METHOD](https://github.com/bmad-code-org/BMAD-METHOD)：** 敏捷 AI 驱动开发的突破性方法。
- **[gsd-build/get-shit-done](https://github.com/gsd-build/get-shit-done)：** 由 TACHES 打造的轻量而强大的元提示、上下文工程与规格驱动开发系统，适用于 Claude Code。
- **[Fission-AI/OpenSpec](https://github.com/Fission-AI/OpenSpec)：** 面向 AI 编码助手的规格驱动开发（SDD）。
- **[OthmanAdi/planning-with-files](https://github.com/OthmanAdi/planning-with-files)：** 在 Claude Code 中实现类 Manus 的持久化 Markdown 规划技能，即支撑那次 20 亿美元收购背后的工作流模式。
- **[Pimzino/spec-workflow-mcp](https://github.com/Pimzino/spec-workflow-mcp)：** 一个 MCP 服务器，为 AI 辅助软件开发提供结构化规格驱动工作流工具，并带有实时 Web 仪表盘与 VSCode 扩展。
- **[Pimzino/claude-code-spec-workflow](https://github.com/Pimzino/claude-code-spec-workflow)：** 面向 Claude Code 的自动化工作流，提供新功能的规格驱动开发流程与缺陷修复流程。
- **[gotalab/cc-sdd](https://github.com/gotalab/cc-sdd)：** 把 AI 编码代理转化为生产可用的规格驱动开发系统，覆盖需求、设计、任务到实现。
- **[Q00/ouroboros](https://github.com/Q00/ouroboros)：** 停止提示式写作，开始精确定义。
- **[papaoloba/spec-based-claude-code](https://github.com/papaoloba/spec-based-claude-code)：** 使用自定义斜杠命令在 Claude Code 中实现规格驱动开发工作流。
- **[pdoronila/cc-sdd](https://github.com/pdoronila/cc-sdd)：** 在 Claude Code 内部实现的规格驱动开发工作流。
- **[kellemar/claude-code-specs-generator](https://github.com/kellemar/claude-code-specs-generator)：** 受 Amazon Kiro IDE 启发的文档与上下文管理系统，可生成结构化规格文档，增强 Claude Code 对项目的理解。

<a id="multi-agent-orchestration"></a>
## 🤖 多智能体编排与协作

- **[affaan-m/everything-claude-code](https://github.com/affaan-m/everything-claude-code)：** 面向 Claude Code、Codex、Opencode、Cursor 等的智能体编排与性能优化系统，涵盖 skills、memory、安全与研究优先开发。
- **[msitarzewski/agency-agents](https://github.com/msitarzewski/agency-agents)：** 把完整 AI agency 带到你手边：从前端专家到社区运营、从创意注入到现实校验，每个智能体都有明确人格、流程与交付物。
- **[wshobson/agents](https://github.com/wshobson/agents)：** 面向 Claude Code 的智能自动化与多智能体编排。
- **[paperclipai/paperclip](https://github.com/paperclipai/paperclip)：** 面向零人工公司的开源编排系统。
- **[Yeachan-Heo/oh-my-claudecode](https://github.com/Yeachan-Heo/oh-my-claudecode)：** 面向 Claude Code 的多智能体编排系统，支持 Autopilot、Ultrapilot、Swarm、Pipeline、Ecomode 五种执行模式，并内置大量 skills 与专用 agents。
- **[fengshao1227/ccg-workflow](https://github.com/fengshao1227/ccg-workflow)：** 多模型协作开发系统：Claude 负责编排，Codex 负责后端，Gemini 负责前端，提供一键安装与覆盖全流程的命令集。
- **[stellarlinkco/myclaude](https://github.com/stellarlinkco/myclaude)：** 多智能体编排工作流系统，支持 Claude Code、Codex、Gemini 与 OpenCode。
- **[bfly123/claude_code_bridge](https://github.com/bfly123/claude_code_bridge)：** Claude、Codex 与 Gemini 的实时多 AI 协作桥接，具备持久上下文和较低 token 开销。
- **[catlog22/Claude-Code-Workflow](https://github.com/catlog22/Claude-Code-Workflow)：** JSON 驱动的多智能体开发框架，具备智能 CLI 编排、上下文优先架构和自动化工作流执行。
- **[Ido-Levi/Hephaestus](https://github.com/Ido-Levi/Hephaestus)：** 半结构化智能体框架：工作流会随着智能体发现需求而自我构建，而不是完全依赖预先预测。
- **[avivl/claude-007-agents](https://github.com/avivl/claude-007-agents)：** 统一的 AI 智能体编排系统，涵盖 14 个类别中的数十个专用 agents，用于现代软件开发。
- **[N1nEmAn/acca](https://github.com/N1nEmAn/acca)：** 多 AI 协作工作流系统，让 Antigravity 编排 Claude CLI 与 Codex CLI 协同工作。
- **[williamnie/aegisFlow](https://github.com/williamnie/aegisFlow)：** 多智能体工作流：调用本地 CLI 工具，把一个想法转化为完整 PRD 和技术设计，并调度工具进行开发。

<a id="task-memory-workspace"></a>
## 🗂️ 任务、记忆与工作区管理

- **[eyaltoledano/claude-task-master](https://github.com/eyaltoledano/claude-task-master)：** 可嵌入 Cursor、Lovable、Windsurf、Roo 等环境的 AI 任务管理系统。
- **[BloopAI/vibe-kanban](https://github.com/BloopAI/vibe-kanban)：** 让 Claude Code、Codex 或任何编码代理发挥 10 倍效率。
- **[steveyegge/beads](https://github.com/steveyegge/beads)：** 为编码代理提供记忆增强。
- **[steveyegge/gastown](https://github.com/steveyegge/gastown)：** Gas Town：多智能体工作区管理器。
- **[snarktank/ai-dev-tasks](https://github.com/snarktank/ai-dev-tasks)：** 一个用于管理 AI 开发智能体的简洁任务管理系统。

<a id="skills-context-packs"></a>
## 🧩 Skills、上下文工程与 Agent 套件

- **[ComposioHQ/awesome-claude-skills](https://github.com/ComposioHQ/awesome-claude-skills)：** 精选的 Claude Skills、资源与工具清单，用于定制 Claude AI 工作流。
- **[muratcankoylan/Agent-Skills-for-Context-Engineering](https://github.com/muratcankoylan/Agent-Skills-for-Context-Engineering)：** 面向上下文工程、多智能体架构与生产级智能体系统的综合 Agent Skills 集合。
- **[garrytan/gstack](https://github.com/garrytan/gstack)：** 复现 Garry Tan 当前的 Claude Code 配置：15 个带强观点的工具，分别扮演 CEO、设计师、工程经理、发布经理、文档工程师和 QA。
- **[Vercel Plugin for Coding Agents](https://vercel.com/changelog/introducing-vercel-plugin-for-coding-agents)：** 面向 Claude Code 和 Cursor 的官方上下文插件，实时注入 Vercel 平台知识。内置 47+ skills、专用 agents、slash commands 和 post-tool 校验。
- **[diet103/claude-code-infrastructure-showcase](https://github.com/diet103/claude-code-infrastructure-showcase)：** 展示 Claude Code 基础设施实践示例，包含 skill 自动激活、hooks 与 agents。
- **[OneRedOak/claude-code-workflows](https://github.com/OneRedOak/claude-code-workflows)：** 作者长期重度使用 Claude Code 后沉淀出的最佳工作流与配置，基于 AI 原生创业实践经验。
- **[feiskyer/claude-code-settings](https://github.com/feiskyer/claude-code-settings)：** 面向氛围编程（vibe coding）的 Claude Code 设置、命令与 agents。
- **[quboqin/template-agenticide-vibecoding](https://github.com/quboqin/template-agenticide-vibecoding)：** 基于 Spec-Driven 与 Test-Driven 的 Claude Code 定制化研发流程与 AI 团队协作框架。

<a id="visual-workflow-tooling"></a>
## 🛠️ 可视化工作流工具

- **[breaking-brake/cc-wf-studio](https://github.com/breaking-brake/cc-wf-studio)：** 面向 AI 智能体的可视化工作流编辑器，支持自然语言编辑、导出并运行工作流。
- **[Stitch](https://stitch.withgoogle.com/)：** Google Labs 的 AI 原生 UI 设计画布，可把自然语言转成高保真界面，支持快速迭代、批注反馈，以及面向后续开发工具的导出。
- **[OleynikAleksandr/antigravity-subagents](https://github.com/OleynikAleksandr/antigravity-subagents)：** 为 Antigravity IDE 提供专用子智能体基础设施。

<a id="historical-workflow-references"></a>
## 🕰️ 历史 / 不可用工作流参考

- **zengruifeng56-del/auto-dev-scheduler：** 与 OpenSpec 深度绑定的 AI 并发自动调度工具。该仓库在 2026 年 3 月 22 日检查时已无法在 GitHub 访问，因此这里仅作为历史参考保留。


## 🤝 贡献指南

欢迎贡献！请阅读我们的[贡献指南](CONTRIBUTING.md)，了解如何提交拉取请求、报告问题和建议新工具。

### 如何贡献

1. Fork 此仓库
2. 创建新分支 (`git checkout -b feature/new-tool`)
3. 添加您的工具，使用正确的格式和官方 URL
4. 提交更改 (`git commit -am 'Add new tool: ToolName'`)
5. 推送到分支 (`git push origin feature/new-tool`)
6. 创建拉取请求

### 工具提交指南

- 包含官方网站 URL
- 提供清晰、简洁的描述
- 适当分类
- 确保工具使用 AI 进行编码/开发
- 对 workflow 系统和 agent 套件，请放入最合适的 workflow 分类

## 📄 许可证

本项目采用 MIT 许可证 - 详情请查看 [LICENSE](LICENSE) 文件。

## ⭐ Star 

如果您觉得这个列表有帮助，请考虑给个 star！⭐
