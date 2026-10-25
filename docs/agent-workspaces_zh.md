# Agent 工作台、CLI 编排与手机控制对照

[English](agent-workspaces.md) · [返回清单](../README_zh.md)

快照日期：**2026-10-25**。星数通过 GitHub API 查询，是注明日期的历史值，不是实时徽章。共收录 **60 个仓库**，包含低星但相关的例外，以及历史项目。

## 范围与方法

通过 12 组 GitHub 查询与网页搜索，覆盖桌面 GUI、CLI 编排、任务/团队控制台、ACP 客户端、终端复用器和手机/IM 桥接。GitHub 检索共得到 **665 个去重仓库命中**；这是发现范围，不代表逐个安装或完整审查了 665 款产品。候选仓库元数据已逐一核对，能力结论以官方文档、release 或源码校准。这是注明日期的调研，不能保证穷尽 GitHub 上的所有项目。

最接近原始需求的是复用本机 Claude Code/Codex CLI 的工具。阅读时区分：

- **发现能力：** 检测已装可执行文件、识别运行中进程、导入历史记录，是三种不同能力。
- **Agent 与模型：** 换 API Provider/模型，不能直接证明换了持有会话的 CLI Agent。
- **交接方式：** 同一应用线程接力、携历史新建 Agent/thread、恢复原生 Provider 会话，是不同契约。隐藏推理、工具状态、缓存和附件通常无法完整迁移。
- **手机能力：** 导入配置、手机浏览器、原生 App、控制同一桌面运行会话，不能互相替代。本地执行通常要求主机在线。
- **证据等级：** “未证实”表示本轮资料不足，不代表绝对不支持；没有逐个安装实测。已核验发布标签的能力会单独注明。

按原始需求，优先比较 **Agent Orchestrator、T3 Code** 的已发布应用内上下文交接；**Orca、AionUI、Paseo** 的多 CLI/多端工作台；**Multica、Paperclip** 的任务与团队管理。下表保留邻近类、小众类和历史类，避免只展示推荐项目而隐藏检索结果。

## CLI 工作台与多设备客户端 (24)

| 项目 | 星数 | CLI 接入 / 定位 | Agent / 模型边界 | 手机 / 状态 | 许可 |
| --- | --- | --- | --- | --- | --- |
| [stablyai/orca](https://github.com/stablyai/orca) | 105,365 | 本机多 CLI IDE、worktree、SSH 与审查 | 可选模型；同聊天跨 Agent 接力未证实；聊天界面仍实验性 | iOS / Android beta | MIT |
| [multica-ai/multica](https://github.com/multica-ai/multica) | 53,752 | 桌面检测已装 CLI；issue、小队与运行管理 | 模型调整影响后续 run；同会话跨 Agent 接力未证实 | Web；iOS 仅源码，尚未上架 | Multica License, additional restrictions |
| [iOfficeAI/AionUi](https://github.com/iOfficeAI/AionUi) | 33,756 | 自动发现本机 CLI；桌面与 WebUI 协作 | 按 Agent 选模型；独立会话；跨 Agent 接力未证实 | WebUI / 消息渠道 | Apache-2.0 |
| [pingdotgg/t3code](https://github.com/pingdotgg/t3code) | 29,960 | 控制已安装 CLI，复用已有订阅 | v0.1.2：同应用线程交接预算内上下文；可选模型；项目早期 | iOS / Android / Web | MIT |
| [slopus/happy](https://github.com/slopus/happy) | 24,304 | 桌面/手机 Agent 工作台；可配置原生执行引擎 | 默认自有执行循环；不兼容引擎通过交接重建上下文；旧 CLI 进入维护期 | iOS / Android / Web | MIT |
| [getpaseo/paseo](https://github.com/getpaseo/paseo) | 21,939 | 自动发现原生 CLI Provider；多主机工作台 | 换 Provider 接力会创建新 Agent；有第三方历史转换插件 | iOS / Android / Web | Apache-2.0 |
| [superset-sh/superset](https://github.com/superset-sh/superset) | 15,540 | CLI IDE，集成 worktree、终端、审查与预览 | 换 Agent 会开新会话；macOS 为主，Linux 实验，暂无 Windows 包 | iPhone / iPad：Pro，系统 26+ | Elastic-2.0 |
| [siteboon/claudecodeui](https://github.com/siteboon/claudecodeui) | 14,278 | CloudCLI：本机 Claude、Codex、Cursor、OpenCode 的 Web UI | 自动发现已有会话；可选模型；新聊天选择 Provider | 浏览器 / PWA | AGPL-3.0 |
| [OrchestratorInc/agent-orchestrator](https://github.com/OrchestratorInc/agent-orchestrator) | 13,606 | 自动检测本机 CLI；任务、worktree 与审查 | v0.14.6：空闲本地会话可换 Agent/模型；历史有预算；云会话不支持切换 | iOS / Android | Apache-2.0 |
| [EKKOLearnAI/ekko-studio](https://github.com/EKKOLearnAI/ekko-studio) | 11,540 | 检测并启动本机 CLI；Global 模式复用原配置 | 多 Agent/模型工作台；同会话跨 Agent 接力未证实 | App / Web 连接 | BUSL-1.1 |
| [omnigent-ai/omnigent](https://github.com/omnigent-ai/omnigent) | 11,036 | 带 UI 与共享会话的 CLI meta-harness | 会话内可选模型；多 Agent 协作不等于主引擎接力；原生 wrapper 不支持 Windows | 终端 / Web / 手机 | Apache-2.0 |
| [op7418/CodePilot](https://github.com/op7418/CodePilot) | 6,507 | 本机 Claude/Codex 运行时与多 Provider 助手 | v0.67.17 首次执行后锁定运行时；可在该运行时内换模型/Provider | 消息平台桥接 | BUSL-1.1 |
| [generalaction/emdash](https://github.com/generalaction/emdash) | 6,079 | 自动发现本机 CLI；桌面、worktree、审查与 SSH | 按任务/聊天选择 Agent；跨 Agent 历史移交未证实 | 专用手机控制未证实 | Apache-2.0 |
| [tiann/hapi](https://github.com/tiann/hapi) | 5,298 | CLI wrapper 与自托管远程会话控制 | Claude/Codex 可按模式限制换模型；跨 Agent 接力未证实 | PWA / Telegram；原生端需构建 | AGPL-3.0 |
| [get-bb/bb](https://github.com/get-bb/bb) | 4,600 | 多 CLI IDE、共享服务器与执行主机 | 已发布的接力会新建 thread 并引用旧 thread，复用工作区 | Web；Android alpha | MIT |
| [spacering-net/codeg](https://github.com/spacering-net/codeg) | 4,091 | 多 CLI ACP 工作台；桌面 / Web / Docker | 文档宣称历史导入/恢复/交接；同线程切换语义未核实 | iOS / Android APK | Apache-2.0 |
| [golutra/golutra](https://github.com/golutra/golutra) | 3,862 | Tauri 桌面多 CLI 编排 | 同会话接力未证实；README 与许可的商业使用表述存在差异 | 手机控制仍列为 Upcoming | BUSL-1.1 |
| [RunMaestro/Maestro](https://github.com/RunMaestro/Maestro) | 3,495 | 桌面本机 CLI 会话、worktree、自动化与群聊 | 跨 Agent 咨询/群聊不等于切换同一原生会话 | Web / 局域网 / 隧道 | AGPL-3.0 |
| [supabitapp/supacode](https://github.com/supabitapp/supacode) | 2,398 | 原生 macOS 终端/worktree 控制台 | Claude/Codex/Copilot hooks；需 macOS 26+；同聊天接力未证实 | 手机支持未证实 | FSL-1.1-ALv2 |
| [happier-dev/happier](https://github.com/happier-dev/happier) | 2,054 | 检测已有 CLI；加密多设备控制 | 可控制模型；同会话跨 Agent 接力明确尚未发布 | iOS / Android / Web / 桌面 | MIT |
| [nimbalyst/nimbalyst](https://github.com/nimbalyst/nimbalyst) | 1,972 | 本机 Claude/Codex 可视化工作区；Crystal 后继 | 并行会话与模型/Provider 选择；同线程跨 Agent 接力未证实 | iPhone / iPad；Android 计划中 | MIT |
| [maddada/Ghostex](https://github.com/maddada/Ghostex) | 1,425 | Rust/GPUI 多 CLI 原生工作台 | 宣称任务中可交接；同会话上下文契约未核实 | Android APK / iOS TestFlight | MIT |
| [kdlbs/kandev](https://github.com/kdlbs/kandev) | 1,008 | 多 CLI 运行时的看板/流水线工作台 | 可能使用托管运行时；按步骤配置 Agent/模型；同聊天接力未证实 | 浏览器，经 VPN / 隧道 | AGPL-3.0 |
| [flyhero/antumi](https://github.com/flyhero/antumi) | 24 | 本机 CLI 检测、聊天、任务看板与额度 | Agent 移交可见文本；切回可恢复其原生会话；可选模型 | 未见已文档化手机端 | Apache-2.0 |

## 终端工作区与手机桥接 (10)

| 项目 | 星数 | CLI 接入 / 定位 | Agent / 模型边界 | 手机 / 状态 | 许可 |
| --- | --- | --- | --- | --- | --- |
| [warpdotdev/warp](https://github.com/warpdotdev/warp) | 65,692 | 内置 Agent 与外部 CLI 支持的智能终端 | 运行外部 CLI 不代表跨 Agent 原生会话迁移 | 远程能力依赖相应服务 | AGPL-3.0 / MIT components |
| [herdrdev/herdr](https://github.com/herdrdev/herdr) | 45,785 | 持久化终端运行时；识别运行中 Agent 活动 | 进程/状态识别与安装扫描不同；模型由各 CLI 控制 | SSH；社区客户端 Ovis / Collie | Apache-2.0 |
| [manaflow-ai/cmux](https://github.com/manaflow-ai/cmux) | 28,397 | macOS 终端、工作区、浏览器与 Agent 通知 | 独立 CLI 进程；同聊天接力未证实；客户端/服务器许可不同 | 付费 iOS TestFlight beta | GPL-3.0-or-later client; BUSL server directories |
| [chenhg5/cc-connect](https://github.com/chenhg5/cc-connect) | 16,085 | 将已装 CLI Agent 桥接到消息平台 | /switch 选择会话；/provider 选择 API 服务，不代表 CLI 引擎交接 | 微信 / 飞书 / Telegram 等 | MIT |
| [smtg-ai/claude-squad](https://github.com/smtg-ai/claude-squad) | 8,666 | tmux + worktree 本机多 CLI 管理器 | 按会话选 profile；同聊天跨 Agent 接力未证实 | 未确认专用手机端 | AGPL-3.0 |
| [amantus-ai/vibetunnel](https://github.com/amantus-ai/vibetunnel) | 4,697 | 浏览器远程控制终端会话 | 包装任意命令；不提供结构化多 Agent 对话迁移 | 浏览器；最新发布仍为 beta | MIT |
| [SeemSeam/claude_codex_bridge](https://github.com/SeemSeam/claude_codex_bridge) | 3,594 | 通过 tmux / WezTerm 进行可见多 CLI 协作 | 切换 Agent/窗口并发消息；同会话换引擎未证实 | Android 控制器 APK | AGPL-3.0 |
| [agent-of-empires/agent-of-empires](https://github.com/agent-of-empires/agent-of-empires) | 3,381 | 多 CLI TUI + Web，集成 tmux、worktree 与 diff | 按会话选 Agent；跨 Agent 接力未证实；Windows 需 WSL2 | 手机浏览器 | MIT |
| [standardagents/dmux](https://github.com/standardagents/dmux) | 1,807 | 并行 CLI Agent 的 tmux/worktree 复用器 | 可同时启动多 Agent、原生续会话；跨 Agent 迁移未证实 | 未确认专用手机端 | MIT |
| [K9i-0/ccpocket](https://github.com/K9i-0/ccpocket) | 1,092 | 通过本机 Bridge 控制 Claude/Codex 的手机/桌面端 | Claude 订阅登录需显式启用 Bridge 选项；同会话换 Agent 未证实 | iOS / Android；macOS 应用 | MIT |

## 任务与团队控制台 (4)

| 项目 | 星数 | CLI 接入 / 定位 | Agent / 模型边界 | 手机 / 状态 | 许可 |
| --- | --- | --- | --- | --- | --- |
| [paperclipai/paperclip](https://github.com/paperclipai/paperclip) | 107,136 | 任务、角色、预算、审批与本机 CLI adapters | Agent 配置与续会话；同聊天换引擎未证实；聊天仍实验性 | 适配手机的管理界面 | MIT |
| [OpenHands/OpenHands](https://github.com/OpenHands/OpenHands) | 91,788 | Agent Canvas 运行 OpenHands 与第三方 CLI/ACP Agent | 本地 / Docker / 远程后端；模型 profiles；原 CLI 跨 Agent 迁移未证实 | Web 前端；原生手机端未证实 | MIT core; check enterprise components |
| [humanlayer/humanlayer](https://github.com/humanlayer/humanlayer) | 12,458 | 机器 daemon 与 Claude/Codex/OpenCode/Pi 团队工作台 | 任务/计划/审查；同会话换引擎未证实；自托管指南尚不完整 | 桌面 / Web；手机支持未证实 | Apache-2.0 |
| [builderz-labs/mission-control](https://github.com/builderz-labs/mission-control) | 6,395 | 自托管任务、运行审查、花费与运行时发现 | Adapter 深度不一；实时会话消息依赖 gateway；schema/API 仍 alpha | 专用手机支持未证实 | MIT |

## 邻近工具：执行模型或范围不同 (12)

| 项目 | 星数 | CLI 接入 / 定位 | Agent / 模型边界 | 手机 / 状态 | 许可 |
| --- | --- | --- | --- | --- | --- |
| [anomalyco/opencode](https://github.com/anomalyco/opencode) | 221,373 | 自有编程 Agent，提供终端、桌面与 IDE 界面 | 多模型后端，不是发现 Claude/Codex CLI 的包装器 | 服务器 / Web 路径，按部署核实 | MIT |
| [farion1231/cc-switch](https://github.com/farion1231/cc-switch) | 148,507 | CLI 安装、Provider、MCP、Skills 与会话工具 | 配置管理器；通过 CLI 命令恢复；配置同步不等于手机控制 | 未证实对话远程控制 | MIT |
| [aaif-goose/goose](https://github.com/aaif-goose/goose) | 55,685 | 自有 Agent 与 Claude/Codex ACP Provider | ACP 续会话/分叉有限制；当前桌面版已移除旧手机隧道 | Roaming 仍实验性，旧手机配对已移除 | Apache-2.0 |
| [CherryHQ/cherry-studio](https://github.com/CherryHQ/cherry-studio) | 52,961 | 聊天/知识库/Agent；Code Mate 检测并启动本机 CLI | Code Mate 打开系统终端；手机配对仅导入配置 | 有手机 App；配对不含历史或 Agent 遥控 | AGPL-3.0 |
| [different-ai/openwork](https://github.com/different-ai/openwork) | 24,252 | 基于 OpenCode 的 Cowork 桌面，支持 Skills、MCP 与多模型 | 外部 CLI 的 MCP 集成不等于本机多 CLI 编排 | 手机接续未证实 | MIT core; enterprise directory separate |
| [winfunc/opcode](https://github.com/winfunc/opcode) | 22,420 | Claude Code GUI；由 Claudia 改名 | 仅 Claude；v0.2.0 发布于 2025-08-31；勿与旧名重复计数 | 手机控制未证实 | AGPL-3.0 |
| [YishenTu/claudian](https://github.com/YishenTu/claudian) | 15,791 | Obsidian 内的多 CLI Agent 插件 | 依赖桌面 Obsidian；共享记忆不等于原生会话迁移 | 仅桌面 | MIT |
| [eigent-ai/eigent](https://github.com/eigent-ai/eigent) | 15,657 | 基于 CAMEL 的桌面 Cowork 与角色 Agent 团队 | 自有 Agent 框架；编排已装 Claude/Codex CLI 未证实 | 手机控制未证实 | Apache-2.0 |
| [NanmiCoder/cc-haha](https://github.com/NanmiCoder/cc-haha) | 15,159 | 自带 Agent 的桌面、worktree、团队与电脑操作 | 内置 claude-haha 引擎；商业软件/接单用途须核查授权 | H5 / 微信 / 飞书 / 钉钉 | Custom Community Source |
| [fathah/hermes-desktop](https://github.com/fathah/hermes-desktop) | 14,453 | 面向 Hermes Agent 的桌面伴侣 | 聚焦单一 Agent，不是通用本机 Claude/Codex CLI 工作台 | 本轮未核实 | MIT |
| [stagewise-io/stagewise](https://github.com/stagewise-io/stagewise) | 6,831 | 自带 Agent 的 IDE，集成实时浏览器与调试工具 | BYOK/API 模型；编排已装 Claude/Codex CLI 未证实 | 手机控制未证实 | AGPL-3.0 |
| [coder/xum](https://github.com/coder/xum) | 2,062 | Xum，原 Mux；本地/SSH 工作区与多模型 | 自有 Agent 执行循环，不是 Claude/Codex CLI 壳 | server mode 响应式 Web UI | AGPL-3.0 |

## 弃用、归档或停止商业维护的参考项目 (4)

| 项目 | 星数 | CLI 接入 / 定位 | Agent / 模型边界 | 手机 / 状态 | 许可 |
| --- | --- | --- | --- | --- | --- |
| [BloopAI/vibe-kanban](https://github.com/BloopAI/vibe-kanban) | 28,446 | 多编程 Agent 的任务/worktree/审查工作台 | 2026-04-10 宣布公司关闭；转社区/本地形态继续 | 旧托管远程服务退出 | Apache-2.0 |
| [21st-dev/1code](https://github.com/21st-dev/1code) | 5,574 | 使用内置运行时的 Claude/Codex 工作台 | 2026-07-07 归档；换 Agent 会携历史创建新聊天 | 云 Agent PWA，未证实接管本机会话 | Apache-2.0 |
| [stravu/crystal](https://github.com/stravu/crystal) | 3,133 | 原 Claude/Codex 会话与 worktree 管理器 | 2026 年 2 月弃用；后继为 Nimbalyst；未归档不等于仍维护 | 手机能力以新产品文档为准 | MIT |
| [sugyan/claude-code-webui](https://github.com/sugyan/claude-code-webui) | 1,137 | 仅 Claude 的浏览器界面 | 2026-05-29 归档；非当前多 CLI 替代品 | 浏览器 | MIT |

## 小众项目与观察工具：保留，但不冒充高星同类 (6)

| 项目 | 星数 | CLI 接入 / 定位 | Agent / 模型边界 | 手机 / 状态 | 许可 |
| --- | --- | --- | --- | --- | --- |
| [rebornix/Agmente](https://github.com/rebornix/Agmente) | 547 | ACP / Codex app-server 的 iOS 客户端 | 远程协议客户端；桌面 CLI 检测与引擎交接未证实 | iOS | See repository license |
| [kzahel/yepanywhere](https://github.com/kzahel/yepanywhere) | 539 | 检测本机 CLI 与会话的手机 Web 客户端 | 主要支持 Claude/Codex；其余实验性；跨 Agent 接力未证实 | Web；原生手机端开发/计划中 | MIT |
| [formulahendry/acp-ui](https://github.com/formulahendry/acp-ui) | 502 | 跨平台 ACP 客户端，桌面/Web/Android | 需单独配置 Adapter；手机/Web 需要远程 WebSocket | Android APK；iOS 需构建 | MIT |
| [pugliatechs/polpo](https://github.com/pugliatechs/polpo) | 46 | 多 CLI 手机控制台与会话浏览器 | 规模很小；跨 Agent 上下文迁移未证实 | Web 控制台 | MIT |
| [Ericonaldo/AgentMonitor](https://github.com/Ericonaldo/AgentMonitor) | 35 | Claude/Codex 执行与监控控制台 | 规模很小；GitHub 元数据未识别许可证 | 浏览器 / relay | License not identified |
| [CHATS-lab/VibeLens](https://github.com/CHATS-lab/VibeLens) | 21 | 本地多 Agent 日志回放与分析 | 仅观察分析，不是执行控制；低星辅助工具 | 未核实 | MIT |

## 关键证据与版本边界

1. **Agent Orchestrator：** [v0.14.6 release](https://github.com/OrchestratorInc/agent-orchestrator/releases/tag/v0.14.6) 已发布 Agent 切换并移除 Developer mode 限制。[切换规则](https://docs.orchestrator.inc/guides/per-role-agents/#switch-agents-mid-session) 要求本地会话空闲，云会话不能切。[标签内交接实现](https://github.com/OrchestratorInc/agent-orchestrator/blob/v0.14.6/backend/internal/domain/handoff_note.go) 会按预算截取历史，并可回查保存的记录；不是原生状态无损迁移。
2. **T3 Code：** [v0.1.2 交接契约](https://github.com/pingdotgg/t3code/blob/v0.1.2/docs/user/portable-handoffs.md) 在应用线程内移交选定历史，不复制推理、工具调用状态与附件。[该版本 README](https://github.com/pingdotgg/t3code/blob/v0.1.2/README.md) 已说明本机 CLI 与手机端。旧内部文档可能与这份更新后的用户契约不一致。
3. **Antumi / Happier / CodePilot：** [Antumi 架构](https://github.com/flyhero/antumi/blob/main/docs/ARCHITECTURE.md) 说明安装检测与可见历史交接；[Happier 专项文档](https://docs.happier.dev/sessions/continue-with-another-agent) 明确标注跨 Agent 接力尚未发布；[CodePilot v0.67.17 设计说明](https://github.com/op7418/CodePilot/blob/v0.67.17/docs/insights/runtime-thread-ownership-and-handoff.md) 明确首次执行后锁定运行时。
4. **Paseo / bb：** [Paseo Provider 文档](https://paseo.sh/docs/providers) 说明原生检测；其目录收录的 [第三方 switch-provider 插件](https://paseo.sh/plugins/anh-chu/switch-provider) 会创建新 Agent，并转换或摘要历史。[bb 稳定版交接实现](https://github.com/get-bb/bb/blob/desktop-v0.47.1/packages/client-core/src/prompt/thread-handoff-request.ts) 会创建引用旧 thread 的新 thread，复用环境。
5. **Multica：** [README](https://github.com/multica-ai/multica#readme) 说明桌面自动发现本机运行时/工具；[Provider 文档](https://multica.ai/docs/providers) 说明恢复各工具自己的 session，不能据此推断跨工具迁移。[Agent 配置](https://multica.ai/docs/agents-create) 中的模型调整影响后续 run。[手机文档](https://multica.ai/docs/mobile-app) 区分源码构建 iOS 与已上架 App。
6. **其他本机工作台：** [Emdash Providers](https://emdash.com/docs/providers)、[Ekko 本机 CLI 模式](https://github.com/EKKOLearnAI/ekko-studio/blob/main/docs/native-coding-agents.md)、[Nimbalyst 手机能力](https://nimbalyst.com/mobile-agent-management/)、[Maestro README](https://github.com/RunMaestro/Maestro#readme) 支撑各自接入与手机边界。Codeg、Ghostex 宣称支持交接，但本轮未核实其同会话语义。
7. **手机限制：** [Orca 手机端](https://www.onorca.dev/docs/mobile) 仍 beta；[Superset](https://github.com/superset-sh/superset#readme) 需 Pro 与 iOS/iPadOS 26+。[HAPI v0.30.7 契约](https://github.com/tiann/hapi/blob/v0.30.7/docs/api/client-contract/rest.md#session-config--mode--model--effort-per-flavor) 列出 Claude/Codex 模型控制限制。[Cherry 手机配对](https://github.com/CherryHQ/cherry-studio-app#-made-for-mobile-connected-to-cherry) 仅导入配置，不含桌面历史/控制。[goose 手机说明](https://goose-docs.ai/docs/experimental/remote-access/mobile-access/) 说明旧隧道已移除。[cmux 价格页](https://cmux.com/pricing) 将 iOS 列入付费早期访问。
8. **不同执行模型：** [Happy harness](https://happy.engineering/recepies/harnesses/) 区分默认自有 Agent 循环与原生引擎；[Cherry Code Mate](https://www.cherryai.com/docs/en/cherrystudio/preview/code-cli/) 检测本机 CLI 后打开系统终端；[cc-connect v1.5.0](https://github.com/chenhg5/cc-connect/blob/v1.5.0/README.md) 区分会话/API Provider 命令；[Herdr Agent 检测](https://herdr.dev/docs/agents/) 识别运行中的终端活动，不是安装扫描器。

## 许可证与生命周期核查

本清单的 MIT 许可不等于所链接工具都采用 MIT。GitHub 的 `licenseInfo` 仅作发现线索；判断授权时要看当前许可证正文、组件范围和版本标签。

- **源码可见或混合条款：** [Multica](https://github.com/multica-ai/multica/blob/main/LICENSE)、[Superset](https://github.com/superset-sh/superset/blob/main/LICENSE.md)、[Ekko](https://github.com/EKKOLearnAI/ekko-studio/blob/main/LICENSE)、[CodePilot](https://github.com/op7418/CodePilot/blob/v0.67.17/LICENSE)、[Supacode](https://github.com/supabitapp/supacode/blob/main/LICENSE)、[cmux](https://github.com/manaflow-ai/cmux/blob/main/LICENSE)、[cc-haha](https://github.com/NanmiCoder/cc-haha/blob/main/LICENSING.md) 存在用途限制或组件差异；cc-haha 还覆盖商业开发/接单用途。[Golutra](https://github.com/golutra/golutra/blob/master/LICENSE) 的 README 与许可商业表述有差异，不能仅凭宣传推断授权。
- **改名去重：** `getAsterisk/claudia` 跳转到 **winfunc/opcode**；`coder/mux` 跳转到 **coder/xum**；`block/goose` 跳转到 **aaif-goose/goose**。每个规范仓库只计一次。
- **维护状态：** [Crystal](https://github.com/stravu/crystal#readme) 虽未归档，但已弃用并转向 Nimbalyst；[1Code](https://github.com/21st-dev/1code) 已归档。[Vibe Kanban 关闭公告](https://www.vibekanban.com/blog/shutdown) 说明转社区/本地形态。[Opcode v0.2.0](https://github.com/winfunc/opcode/releases/tag/v0.2.0) 证明已有下载包，README 的“即将发布”过时，但该 release 本身已是 2025 年。历史项目保留供迁移参考，不列默认首选。

纯框架、Skills 集、API 网关、仅用量监控和通用远程桌面产品，原则上不进入核心对照；具有直接相关 UI 或桥接能力时才列为邻近类。小项目保留发现记录，但不作为高星推荐。
