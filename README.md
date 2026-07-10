# Awesome Vibe Coding Tools ✨

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Contributors Welcome](https://img.shields.io/badge/contributors-welcome-brightgreen.svg?style=flat)](CONTRIBUTING.md)

> A curated list of vibe coding plugins, IDEs, development tools, and workflow systems that enhance programming productivity through artificial intelligence.

## 📋 Table of Contents

- [AI-Enhanced IDEs & Editors](#ai-enhanced-ides--editors)
- [Terminal-Based AI Agents](#terminal-based-ai-agents)
- [VS Code Extensions](#vs-code-extensions)
- [Web-Based Development Platforms](#web-based-development-platforms)
- [Enterprise & Platform Solutions](#enterprise--platform-solutions)
- [Specialized Tools](#specialized-tools)
- [CLI Workflow Systems & Agent Enhancers](#cli-workflow-systems)
- [Workflow Systems & Spec-Driven Development](#workflow-systems)
- [Multi-Agent Orchestration & Collaboration](#multi-agent-orchestration)
- [Task, Memory & Workspace Management](#task-memory-workspace)
- [Skills, Context Engineering & Agent Packs](#skills-context-packs)
- [Visual Workflow Tooling](#visual-workflow-tooling)
- [Historical / Unavailable Workflow References](#historical-workflow-references)
- [Contributing](#contributing)
- [License](#license)

## 🚀 AI-Enhanced IDEs & Editors

- **[Cursor](https://cursor.com/):** AI-first coding editor and agent platform with code-aware chat, Composer, cloud/background agents, automations, Jira handoff, shared canvases, and `/loop` for local long-running agents.
- **[Windsurf](https://windsurf.codeium.com/):** Multi-IDE support from Codeium, with "Cascade Flow" agents for multi-step automation, live preview for UI, and robust team collaboration. Especially useful for fast prototyping, but often loses context in large projects.
- **[Kiro](https://kiro.dev/):** AWS experimental IDE with spec-driven scaffolding for microservices and cloud-native solutions, making end-to-end development and deployment frictionless.
- **[Google Antigravity](https://antigravity.google/):** Google's agent-first development platform with Antigravity 2.0 desktop app, CLI, and SDK. Orchestrates parallel agents, dynamic subagents, scheduled tasks, and integrations across AI Studio, Android, and Firebase.
- **[CodeBuddy (Tencent Cloud)](https://cloud.tencent.com/product/codebuddy):** AI-driven IDE for automated frontend/backend/database generation, integrated with multiple LLM choices and Figma-to-code capabilities.
- **[Trae](https://trae.ai/):** ByteDance automated builder, syncs Figma design to code, and specializes in low-code prototyping for small teams.
- **[Zed](https://zed.dev/):** Rust-powered superfast editor with 120fps rendering, native AI suggestions, and robust collaboration for frontend professionals.
- **[Lingma (Tongyi Lingma)](https://tongyi.aliyun.com/lingma):** Alibaba's flagship code assistant, supports Chinese/English, major IDEs and standalone operation.
- **[Comate (Baidu)](https://comate.baidu.com/):** Multi-lingual, 50% real adoption, supports all major IDEs and plugins, end-to-end developer automation.
- **[Qoder](https://qoder.ai/):** Intelligent code generation and programming assistant with support for multiple programming languages, offering code completion, error detection, and smart refactoring capabilities.
- **[Crystal (Claude Code Manager)](https://github.com/stravu/crystal):** Multi-session agent manager, Git worktree integration, Diff/merge viewer. Perfect for multi-solution prototyping.
- **[Void](https://voideditor.com/):** Open-source Cursor alternative, checkpoint visualization, agentic AI with any model/local hosting, privacy-focused for enterprise use.
- **[IntelliJ IDEA AI](https://www.jetbrains.com/idea/):** Enterprise mainstream Java IDE with native AI completion, code navigation for massive projects.
  - **[Explyt](https://github.com/explyt/explyt):** AI agent plugin for JetBrains IDEs that uses IDE tools (debugger, refactorings, static analysis) to handle complex code.


## 💻 Terminal-Based AI Agents

- **[Claude Code](https://claude.ai/code):** Full-codebase awareness and agentic edit/test/PR workflows across terminal, IDE, and background task surfaces. Dynamic workflows let it plan large tasks, run parallel subagents, and verify outputs before reporting back.
- **[Gemini CLI](https://ai.google.dev/gemini-api/docs/cli):** Google command-line flagship, 1M context, multimodal chat and robust Shell scripting automation.
- **[Aider](https://aider.chat/):** Terminal Git-integrated pair programmer, high Swe-bench scores, focused on patching and smart code navigation.
- **[Cosine CLI](https://cosine.sh/cli):** Autonomous AI engineer in your terminal with full local tool access. Plans, writes, tests, and iterates like a real developer. Features cross-surface continuity between terminal and web, runs in your actual environment with access to local files, builds, and tests. No context switching required.
- **[Goose](https://github.com/Squadrick/goose):** Extensible open-source CLI agent, plugin architecture, multi-model support, ideal for distributed code workflows.
- **[Kode](https://github.com/shareAI-lab/Kode):** Open-source multi-model CLI agent supporting GLM, Qwen, Kimi, DeepSeek, and more. Features true multi-model collaboration with intelligent task distribution, expert model consultation (AskExpertModel tool), and parallel subagent processing. Tab key quick model switching and flexible model allocation for different purposes (main, task, reasoning, quick).
- **[Factory CLI](https://factory.ai/product/ide):** AI Droids for terminal and IDE with multi-model support (Claude, GPT, Gemini). Features adjustable autonomy levels, agentic search for million-line codebases, and cross-platform context memory. Works natively in VS Code, JetBrains, Vim, and more with enterprise-grade security.
- **[OpenCode](https://github.com/opencodeinterpret/opencode):** Native terminal agent with LSP and dozens of LLMs. Suitable for polyglot projects and multi-model integration.
- **[Warp](https://www.warp.dev/):** AI-powered terminal, natural language commands and smart autocompletion.
- **[Codex CLI](https://openai.com/index/openai-codex/):** OpenAI's official tool, lightweight and fast terminal-based codegen.
- **[GitHub Copilot CLI](https://github.com/features/copilot/cli):** Terminal-native GitHub coding agent with `/plan`, background delegation, MCP/plugins/skills, and cross-session memory. Designed to move from issues to pull requests without leaving the shell.
- **[Crush](https://github.com/charmbracelet/crush):** Charmbracelet's agent, multi-model and LSP, highly customizable terminal-based coding.
- **[Cursor CLI](https://cursor.com/en/cli):** Shares context with Cursor IDE, supports advanced real-time code reviews, writing, and agentic guidance.
- **[Groq Code CLI](https://github.com/build-with-groq/groq-code-cli):** Extensible plugin framework for workflow automation in CLI, fully customizable.
- **[Amp](https://ampcode.com/):** Autonomous reasoning and editing, ideal for multi-model and agentic code tasks in the terminal.
- **[iflow CLI](https://github.com/iflow-ai/iflow-cli):** Intelligent workflow automation CLI tool for developers, providing AI-powered task orchestration and streamlined development processes in the terminal.
- **[Qoder CLI](https://qoder.com/cli):** Command-line version of Qoder, bringing intelligent code generation and AI programming assistance to the terminal with multi-language support and smart refactoring capabilities.
- **[qwen-code](https://github.com/QwenLM/qwen-code):** Terminal-based coding agent from Alibaba Cloud that lives in the digital world. Features full codebase awareness, OAuth authentication, multi-model support, and strong code understanding capabilities. Supports code generation, debugging, and refactoring with 1M context window and vision model integration.
- **[Auggie](https://augmentcode.com/cli):** Command-line version of Augment Code, bringing enterprise-grade AI coding assistance to the terminal with large context windows and regulatory compliance features.



## 🔌 VS Code Extensions

- **[GitHub Copilot](https://github.com/features/copilot):** Multi-model assistant spanning VS Code, GitHub.com, mobile, and background coding-agent workflows. Supports chat/edit/agent modes, code review, model selection, and enterprise governance.
- **[Cline](https://github.com/cline/cline):** Autonomous AI agent with file/web editing, fully open-source and extensible, supports CLI mode.
- **[Continue](https://github.com/continuedev/continue):** Open-source GPT/Claude/Gemini integration, inline code chat, file/project contextual support, API/model choice.
- **[RooCode](https://github.com/RooCodeInc/Roo-Code):** Agent teams allow concurrent multi-model automation, premium API support.
- **[KiloCode](https://github.com/Kilo-Org/kilocode):** Roo/Cline superset, orchestrator mode and error recovery, credit-based system, advanced multi-agent permissions.
- **[Cody (Sourcegraph)](https://sourcegraph.com/cody):** Multi-repo code search, explanation, custom style prompts, supports several major LLMs.
- **[CodeGPT](https://codegpt.co/):** In-editor chat/AI debugging, explanations, code/test/doc generation, supports OpenAI/Anthropic.
- **[Graphite](https://graphite.dev/):** Stacked PR workflow, instant AI code review comments, sidebar branch management.
- **[Tabnine](https://www.tabnine.com/):** Local deployment, adaptive to personal coding style, ideal for privacy/security-first teams.
- **[Gemini Code Assist](https://codeassist.google/):** Deep Google/Colab integration for real-time code support.
- **[ChatGPT for VS Code](https://marketplace.visualstudio.com/items?itemName=openai.chatgpt):** Direct OpenAI chat integration, supports debugging/testing/doc generation.
- **[Augment Code](https://augmentcode.com/):** 200K+ context tokens, optimized for large enterprise repos and regulatory compliance, with SOC2-ready deployment.


## 🌐 Web-Based Development Platforms

- **[Cosine](https://cosine.sh/):** Autonomous AI coding agent powered by Genie 2, designed to complete tasks end-to-end without human supervision. Features asynchronous task assignment, multi-agent deployment, and workflow integrations with Slack, Jira, and Linear. Achieves 72% on SWE-Lancer benchmark, leading in production-grade tasks.
- **[v0 (Vercel)](https://v0.app/):** Natural language to React UI, built-in shadcn/ui, dead-simple frontend app prototyping.
- **[Bolt.new (StackBlitz)](https://bolt.new/):** Full-stack app creation/deployment in-browser, leverages WebContainers, no local tooling required.
- **[Lovable](https://lovable.dev/):** No-code builder for instant full-stack web apps from natural language.
- **[Replit AI Agent/Ghostwriter](https://replit.com/ai):** Browser IDE, multi-lingual coding, on-the-fly explanation and bug fixing, real-time collaboration.
- **[Google AI Studio](https://aistudio.google.com/):** Google's prompt-to-production app builder powered by the Antigravity coding agent. Supports Firebase-backed apps, Workspace integrations, mobile idea capture, native Android app generation, Play test-track publishing, and export to Antigravity.
- **[Knack](https://www.knack.com/):** Automated code/data-driven dev, optimized for speed/quality/team use cases.
- **[CodeWP](https://codewp.ai/):** AI site builder for WordPress, end-to-end generation and deployment.
- **[Figma Make](https://www.figma.com/):** Figma's AI-powered feature that creates functional prototypes and web apps from natural language prompts. Automatically generates frontend and backend code with Supabase integration for backend services.
- **[Base44](https://base44.com/):** AI-powered no-code platform for building web and mobile apps through natural language conversations. Features built-in database, authentication, storage, analytics, and email functionality with seamless external service integration.
- **[Conductor](https://conductor.build/):** AI-powered development platform with automated code generation, error fixing, and batch refactoring capabilities. Integrates with GitHub, GitLab, AWS CodeCommit, Azure DevOps, and BitBucket for streamlined workflows.
- **[Aura](https://www.aura.build/):** AI-enhanced development platform offering real-time collaboration, intelligent code analysis, and automated optimization for building high-performance applications.
- **[Verdent](https://www.verdent.ai/):** Cloud-based AI development platform focused on sustainable and efficient application development with AI-driven code reviews and performance optimization.


## 🏢 Enterprise & Platform Solutions

- **[Codex (OpenAI)](https://openai.com/codex/):** Cloud agents, CLI, private deployments, comprehensive codegen with audit/security options.
- **[Devin (Cognition)](https://devin.ai/):** Team-grade autonomous software engineer for end-to-end automation.
- **[Replit](https://replit.com/):** Multi-agent workspaces, natural language generation, multi-user collaboration.
- **[Jules (Google)](https://jules.google/):** Automated pull requests, CI/CD and code repair integration.
- **[Open SWE (LangGraph)](https://swe.langchain.com/):** Open-source enterprise agent platform, workflow customizability.
- **[OpenHands](https://github.com/OpenHands/OpenHands):** Open-source, self-hostable AI software developer platform formerly known as OpenDevin. Agents can edit code, run commands, browse, and work through software tasks end-to-end with web, CLI, and enterprise deployment options.
- **[Coder Agents](https://coder.com/blog/introducing-coder-agents):** Self-hosted, model-agnostic coding agents built into the Coder control plane. Provides centralized controls for models, prompts, workspaces, usage, MCP, skills, subagents, and background execution on customer infrastructure.
- **[UiPath for Coding Agents](https://www.uipath.com/developers/coding-agents):** Enterprise automation platform layer for Claude Code, Codex, Gemini CLI, Cursor, and other coding agents. Lets agents build, review, test, and govern UiPath automations with RBAC, audit, and policy controls.
- **[Amazon Q Developer](https://aws.amazon.com/q/developer/):** AWS-native coding agent, IDE integration, cloud/service support.
- **[IBM CodeAssist](https://www.ibm.com/products/watsonx-code-assistant):** AI-powered mainframe developer automation, tailored for regulated industries.
- **[Tabnine Enterprise](https://www.tabnine.com/):** Private cloud, compliance/security for large teams.


## 🔧 Specialized Tools

- **[RepoPrompt](https://github.com/repo-prompt/repo-prompt):** Mac-native AI file/code management and iteration, perfect for version organization.
- **[DeepCode (Snyk)](https://snyk.io/product/deepcode-ai/):** AI fast code security analysis and actionable fix recommendations.
- **[Umami](https://umami.is/):** AI-driven frontend optimization/performance analytics.
- **[TraceRoot AI](https://traceroot.ai/):** Bug location & patch suggestion, automatic root cause.
- **[Chrome DevTools for agents](https://developer.chrome.com/docs/devtools/agents):** Stable Chrome DevTools MCP server, CLI, and agent skills that let coding agents inspect live browser state, debug runtime issues, emulate users, and run Lighthouse audits before shipping.
- **[Blitz](https://blitzjs.com/):** Native Next.js AI plugin for rapid frontend dev.
- **[BlackBox AI](https://blackbox.ai/):** Code completion plus security scan all-in-one.
- **[ColDeco](https://coldeco.ai/):** Visual AI-generated code inspection and review.
- **[IntelliDev](https://intellidev.ai/):** ML-powered terminal workflow assistant for devs/logs/tasks.


<a id="cli-workflow-systems"></a>
## 🧰 CLI Workflow Systems & Agent Enhancers

- **[anomalyco/opencode](https://github.com/anomalyco/opencode):** The open source coding agent.
- **[code-yeongyu/oh-my-openagent](https://github.com/code-yeongyu/oh-my-openagent):** OMO, the best agent harness (formerly oh-my-opencode), providing async subagents, curated tools, and a stronger agent experience for OpenCode and related coding agents.
- **[UfoMiao/zcf](https://github.com/UfoMiao/zcf):** Zero-Config Code Flow for Claude Code and Codex.
- **[Yeachan-Heo/oh-my-codex](https://github.com/Yeachan-Heo/oh-my-codex):** OmX, power tools for OpenAI Codex CLI with hooks, agent teams, HUDs, and more.
- **[alvinunreal/oh-my-opencode-slim](https://github.com/alvinunreal/oh-my-opencode-slim):** Slimmed, cleaned, and fine-tuned oh-my-opencode fork that consumes much less tokens.
- **[agent-sh/agentsys](https://github.com/agent-sh/agentsys):** A system for Claude Code, OpenCode, Codex, Cursor, and Kiro that automates everything around AI coding with plugins, agents, and skills.
- **[zhukunpenglinyutong/ai-max](https://github.com/zhukunpenglinyutong/ai-max):** A one-click upgrade pack for Claude Code with production-grade agents, skills, hooks, commands, rules, and MCP configuration.

<a id="workflow-systems"></a>
## 🧠 Workflow Systems & Spec-Driven Development

- **[obra/superpowers](https://github.com/obra/superpowers):** An agentic skills framework and software development methodology that works.
- **[github/spec-kit](https://github.com/github/spec-kit):** Toolkit to help you get started with Spec-Driven Development.
- **[bmad-code-org/BMAD-METHOD](https://github.com/bmad-code-org/BMAD-METHOD):** Breakthrough Method for Agile AI Driven Development.
- **[gsd-build/get-shit-done](https://github.com/gsd-build/get-shit-done):** A light-weight and powerful meta-prompting, context engineering, and spec-driven development system for Claude Code by TACHES.
- **[Fission-AI/OpenSpec](https://github.com/Fission-AI/OpenSpec):** Spec-driven development (SDD) for AI coding assistants.
- **[OthmanAdi/planning-with-files](https://github.com/OthmanAdi/planning-with-files):** Claude Code skill implementing Manus-style persistent markdown planning, the workflow pattern behind the $2B acquisition.
- **[Pimzino/spec-workflow-mcp](https://github.com/Pimzino/spec-workflow-mcp):** A Model Context Protocol server that provides structured spec-driven development workflow tools for AI-assisted software development, with a real-time web dashboard and VS Code extension.
- **[Pimzino/claude-code-spec-workflow](https://github.com/Pimzino/claude-code-spec-workflow):** Automated workflows for Claude Code, featuring spec-driven development for new features and a streamlined bug-fix workflow.
- **[gotalab/cc-sdd](https://github.com/gotalab/cc-sdd):** Spec-driven development for team workflows, transforming AI coding agents into production-ready requirements, design, tasks, and implementation pipelines.
- **[Q00/ouroboros](https://github.com/Q00/ouroboros):** Stop prompting. Start specifying.
- **[papaoloba/spec-based-claude-code](https://github.com/papaoloba/spec-based-claude-code):** Implementation of a Spec-Driven Development workflow in Claude Code using custom slash commands.
- **[pdoronila/cc-sdd](https://github.com/pdoronila/cc-sdd):** Spec Driven Development Workflow inside Claude Code.
- **[kellemar/claude-code-specs-generator](https://github.com/kellemar/claude-code-specs-generator):** A documentation and context management system inspired by Amazon's Kiro IDE that generates structured specification documents for Claude Code.

<a id="multi-agent-orchestration"></a>
## 🤖 Multi-Agent Orchestration & Collaboration

- **[affaan-m/everything-claude-code](https://github.com/affaan-m/everything-claude-code):** The agent harness performance optimization system. Skills, instincts, memory, security, and research-first development for Claude Code, Codex, Opencode, Cursor, and beyond.
- **[msitarzewski/agency-agents](https://github.com/msitarzewski/agency-agents):** A complete AI agency at your fingertips, from frontend wizards to Reddit community ninjas, from whimsy injectors to reality checkers, with specialized experts, processes, and deliverables.
- **[wshobson/agents](https://github.com/wshobson/agents):** Intelligent automation and multi-agent orchestration for Claude Code.
- **[paperclipai/paperclip](https://github.com/paperclipai/paperclip):** Open-source orchestration for zero-human companies.
- **[Yeachan-Heo/oh-my-claudecode](https://github.com/Yeachan-Heo/oh-my-claudecode):** Multi-agent orchestration for Claude Code with Autopilot, Ultrapilot, Swarm, Pipeline, and Ecomode modes, plus many built-in skills and specialized agents.
- **[fengshao1227/ccg-workflow](https://github.com/fengshao1227/ccg-workflow):** A multi-model collaborative development system with Claude orchestration, Codex backend support, Gemini frontend support, and a full-stack command set.
- **[stellarlinkco/myclaude](https://github.com/stellarlinkco/myclaude):** Multi-agent orchestration workflow for Claude Code, Codex, Gemini, and OpenCode.
- **[bfly123/claude_code_bridge](https://github.com/bfly123/claude_code_bridge):** Real-time multi-AI collaboration for Claude, Codex, and Gemini with persistent context and minimal token overhead.
- **[catlog22/Claude-Code-Workflow](https://github.com/catlog22/Claude-Code-Workflow):** A JSON-driven multi-agent development framework with intelligent CLI orchestration, context-first architecture, and automated workflow execution.
- **[Ido-Levi/Hephaestus](https://github.com/Ido-Levi/Hephaestus):** A semi-structured agentic framework where workflows build themselves as agents discover what needs to be done.
- **[avivl/claude-007-agents](https://github.com/avivl/claude-007-agents):** A unified AI agent orchestration system featuring dozens of specialized agents across 14 categories for modern software development.
- **[N1nEmAn/acca](https://github.com/N1nEmAn/acca):** A multi-AI collaborative workflow system that lets Antigravity orchestrate Claude CLI and Codex CLI together.
- **[williamnie/aegisFlow](https://github.com/williamnie/aegisFlow):** A multi-agent workflow that turns an idea into a full PRD and technical design, then orchestrates local toolchains to build it.

<a id="task-memory-workspace"></a>
## 🗂️ Task, Memory & Workspace Management

- **[eyaltoledano/claude-task-master](https://github.com/eyaltoledano/claude-task-master):** An AI-powered task management system you can drop into Cursor, Lovable, Windsurf, Roo, and others.
- **[BloopAI/vibe-kanban](https://github.com/BloopAI/vibe-kanban):** Get 10X more out of Claude Code, Codex, or any coding agent.
- **[steveyegge/beads](https://github.com/steveyegge/beads):** A memory upgrade for your coding agent.
- **[steveyegge/gastown](https://github.com/steveyegge/gastown):** Gas Town, a multi-agent workspace manager.
- **[snarktank/ai-dev-tasks](https://github.com/snarktank/ai-dev-tasks):** A simple task management system for managing AI dev agents.

<a id="skills-context-packs"></a>
## 🧩 Skills, Context Engineering & Agent Packs

- **[ComposioHQ/awesome-claude-skills](https://github.com/ComposioHQ/awesome-claude-skills):** A curated list of awesome Claude Skills, resources, and tools for customizing Claude AI workflows.
- **[muratcankoylan/Agent-Skills-for-Context-Engineering](https://github.com/muratcankoylan/Agent-Skills-for-Context-Engineering):** A comprehensive collection of Agent Skills for context engineering, multi-agent architectures, and production agent systems.
- **[garrytan/gstack](https://github.com/garrytan/gstack):** Garry Tan's current Claude Code setup with 15 opinionated tools covering CEO, designer, engineering management, release, docs, and QA roles.
- **[Vercel Plugin for Coding Agents](https://vercel.com/changelog/introducing-vercel-plugin-for-coding-agents):** Official context plugin for Claude Code and Cursor that injects Vercel platform knowledge in real time. Ships 47+ skills, specialist agents, slash commands, and post-tool validation.
- **[diet103/claude-code-infrastructure-showcase](https://github.com/diet103/claude-code-infrastructure-showcase):** Examples of Claude Code infrastructure with skill auto-activation, hooks, and agents.
- **[OneRedOak/claude-code-workflows](https://github.com/OneRedOak/claude-code-workflows):** Battle-tested workflows and configurations distilled from heavy Claude Code usage in an AI-native startup context.
- **[feiskyer/claude-code-settings](https://github.com/feiskyer/claude-code-settings):** Claude Code settings, commands, and agents for vibe coding.
- **[quboqin/template-agenticide-vibecoding](https://github.com/quboqin/template-agenticide-vibecoding):** A customized Claude Code R&D workflow system and AI team collaboration framework based on spec-driven and test-driven development.

<a id="visual-workflow-tooling"></a>
## 🛠️ Visual Workflow Tooling

- **[breaking-brake/cc-wf-studio](https://github.com/breaking-brake/cc-wf-studio):** A visual workflow editor for AI agents with natural-language editing, export, and run support.
- **[Stitch](https://stitch.withgoogle.com/):** Google Labs' AI-native UI design canvas that turns natural language into high-fidelity interfaces. Supports rapid iteration, critique, and export toward downstream developer tools.
- **[OleynikAleksandr/antigravity-subagents](https://github.com/OleynikAleksandr/antigravity-subagents):** Infrastructure that enables Antigravity IDE to utilize specialized sub-agents.

<a id="historical-workflow-references"></a>
## 🕰️ Historical / Unavailable Workflow References

- **zengruifeng56-del/auto-dev-scheduler:** An AI concurrent auto-scheduling tool deeply integrated with OpenSpec. The repository was unavailable on GitHub when checked on March 22, 2026, so it is kept here as a historical reference.


## 🤝 Contributing

Contributions are welcome! 

### How to Contribute

1. Fork this repository
2. Create a new branch (`git checkout -b feature/new-tool`)
3. Add your tool with proper formatting and official URL
4. Commit your changes (`git commit -am 'Add new tool: ToolName'`)
5. Push to the branch (`git push origin feature/new-tool`)
6. Create a Pull Request

### Tool Submission Guidelines

- Include the official website URL
- Provide a clear, concise description
- Categorize appropriately
- Ensure the tool uses AI for coding/development
- For workflow systems and agent stacks, place them in the most relevant workflow category

## 📄 License

This project is licensed under the MIT License.

## ⭐ Star History

If you find this list helpful, please consider giving it a star! ⭐

---

**Made with ❤️ **
