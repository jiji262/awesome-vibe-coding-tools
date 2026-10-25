# Agent workbenches, CLI orchestration, and phone control

[中文](agent-workspaces_zh.md) · [Back to catalog](../README.md)

Snapshot: **2026-10-25**. GitHub stars were queried through the GitHub API; they are historical values, not live badges. The catalog contains **60 repositories**, including lower-star exceptions and historical projects.

## Scope and method

Discovery combined 12 GitHub queries and web searches across desktop GUI, CLI orchestration, task/team consoles, ACP clients, terminal multiplexers, and phone/IM bridges. GitHub search returned **665 distinct repository hits**; this is discovery coverage, not 665 installed or fully reviewed products. Candidate repository metadata was checked individually, and official documentation, releases, or source were used to calibrate capability claims. This is a dated survey, not a guarantee of every project on GitHub.

The closest matches reuse installed Claude Code/Codex CLIs. Keep these distinctions visible:

- **Discovery:** finding installed executables, finding running processes, and importing transcript files are separate capabilities.
- **Agent vs model:** changing an API provider/model does not establish switching the CLI agent that owns a conversation.
- **Handoff:** a shared app thread, a new agent/thread seeded with history, and a resumed native provider session are different contracts. Hidden reasoning, tool state, caches, and attachments are not generally portable.
- **Phone:** configuration import, a phone browser, a native app, and control of the same running desktop session are separate capabilities. Local execution normally requires an online host.
- **Evidence:** unverified means no sufficient support was found in the inspected sources; it does not prove impossibility. Documentation/source claims were not validated by installing each app. Release evidence is called out where checked.

For the original requirements, start with **Agent Orchestrator and T3 Code** for released in-app context handoff; **Orca, AionUI, and Paseo** for broader CLI/multi-device workspaces; **Multica and Paperclip** for task/team management. The tables preserve adjacent and small projects so that this shortlist does not hide discovery results.

## CLI workbenches and multi-device clients (24)

| Project | Stars | CLI integration / role | Agent / model boundary | Phone / status | License |
| --- | --- | --- | --- | --- | --- |
| [stablyai/orca](https://github.com/stablyai/orca) | 105,365 | Local multi-CLI IDE, worktrees, SSH and review | Model picker; cross-agent same-chat handoff unverified; chat experimental | iOS / Android beta | MIT |
| [multica-ai/multica](https://github.com/multica-ai/multica) | 53,752 | Desktop discovers installed CLIs; issue / squad / run management | Model changes affect later runs; cross-agent same-session handoff unverified | Web; iOS source only, no store release | Multica License, additional restrictions |
| [iOfficeAI/AionUi](https://github.com/iOfficeAI/AionUi) | 33,756 | Auto-discovers local CLIs; desktop / WebUI cowork | Per-agent model selection; independent sessions; cross-agent handoff unverified | WebUI / messaging channels | Apache-2.0 |
| [pingdotgg/t3code](https://github.com/pingdotgg/t3code) | 29,960 | Controls installed CLI agents using existing subscriptions | v0.1.2: same app thread, budgeted context handoff; model selection; early-stage | iOS / Android / Web | MIT |
| [slopus/happy](https://github.com/slopus/happy) | 24,304 | Desktop/mobile agent workspace; configurable native harnesses | Default own loop; incompatible harness switches rebuild context with handoff; original CLI in maintenance | iOS / Android / Web | MIT |
| [getpaseo/paseo](https://github.com/getpaseo/paseo) | 21,939 | Auto-discovers native CLI providers; multi-host workspace | Provider handoff creates a new agent; third-party conversion plugin available | iOS / Android / Web | Apache-2.0 |
| [superset-sh/superset](https://github.com/superset-sh/superset) | 15,540 | CLI IDE with worktrees, terminals, review and previews | Agent handoff starts a new session; macOS primary, Linux experimental, no Windows build | iPhone / iPad: Pro, OS 26+ | Elastic-2.0 |
| [siteboon/claudecodeui](https://github.com/siteboon/claudecodeui) | 14,278 | CloudCLI: Web UI over local Claude, Codex, Cursor and OpenCode | Discovers existing sessions; model selection; provider chosen for new chat | Browser / PWA | AGPL-3.0 |
| [OrchestratorInc/agent-orchestrator](https://github.com/OrchestratorInc/agent-orchestrator) | 13,606 | Auto-detects local CLIs; tasks, worktrees and review | v0.14.6: idle local sessions can switch agent/model; bounded handoff; no cloud-session switch | iOS / Android | Apache-2.0 |
| [EKKOLearnAI/ekko-studio](https://github.com/EKKOLearnAI/ekko-studio) | 11,540 | Detects and launches local CLIs; Global mode reuses CLI config | Multi-agent/model workspace; same-session cross-agent handoff unverified | App / Web relay | BUSL-1.1 |
| [omnigent-ai/omnigent](https://github.com/omnigent-ai/omnigent) | 11,036 | CLI meta-harness with UI and shared sessions | Mid-session model selection; multi-agent collaboration does not prove engine handoff; native wrappers not on Windows | Terminal / Web / phone | Apache-2.0 |
| [op7418/CodePilot](https://github.com/op7418/CodePilot) | 6,507 | Local Claude/Codex runtimes plus multi-provider assistant | v0.67.17 locks runtime after first execution; models/providers can change inside that runtime | Messaging bridges | BUSL-1.1 |
| [generalaction/emdash](https://github.com/generalaction/emdash) | 6,079 | Auto-discovers local CLIs; desktop, worktrees, review and SSH | Agent selected for task/chat; cross-agent history transfer unverified | Dedicated phone control unverified | Apache-2.0 |
| [tiann/hapi](https://github.com/tiann/hapi) | 5,298 | CLI wrapper and self-hosted remote session control | Claude/Codex model changes supported with mode limits; cross-agent handoff unverified | PWA / Telegram; native source builds | AGPL-3.0 |
| [get-bb/bb](https://github.com/get-bb/bb) | 4,600 | Multi-CLI IDE, shared server and execution hosts | Released handoff creates a new thread referring to the old thread; reuses workspace | Web; Android alpha | MIT |
| [spacering-net/codeg](https://github.com/spacering-net/codeg) | 4,091 | Multi-CLI ACP workspace; desktop / Web / Docker | Documents history import/resume/handoff; exact same-thread semantics unverified | iOS / Android APK | Apache-2.0 |
| [golutra/golutra](https://github.com/golutra/golutra) | 3,862 | Tauri desktop multi-CLI orchestration | Same-session handoff unverified; README and license commercial wording differ | Mobile listed as upcoming | BUSL-1.1 |
| [RunMaestro/Maestro](https://github.com/RunMaestro/Maestro) | 3,495 | Desktop local CLI sessions, worktrees, automation and group chat | Cross-agent consultation/group chat does not prove switching one native conversation | Web / LAN / tunnel | AGPL-3.0 |
| [supabitapp/supacode](https://github.com/supabitapp/supacode) | 2,398 | Native macOS terminal/worktree command center | Claude/Codex/Copilot hooks; macOS 26+; same-chat handoff unverified | Phone support unverified | FSL-1.1-ALv2 |
| [happier-dev/happier](https://github.com/happier-dev/happier) | 2,054 | Detects existing CLIs; encrypted multi-device control | Model controls available; same-session cross-agent continuation explicitly unreleased | iOS / Android / Web / Desktop | MIT |
| [nimbalyst/nimbalyst](https://github.com/nimbalyst/nimbalyst) | 1,972 | Visual local Claude/Codex workspace; successor to Crystal | Parallel sessions and model/provider choices; cross-agent same-thread handoff unverified | iPhone / iPad; Android planned | MIT |
| [maddada/Ghostex](https://github.com/maddada/Ghostex) | 1,425 | Rust/GPUI multi-CLI native workspace | Advertises task handoff; exact same-session context contract unverified | Android APK / iOS TestFlight | MIT |
| [kdlbs/kandev](https://github.com/kdlbs/kandev) | 1,008 | Kanban / pipeline workspace with multiple CLI runtimes | May use managed runtimes; per-step agent/model profiles; same-chat handoff unverified | Browser via VPN / tunnel | AGPL-3.0 |
| [flyhero/antumi](https://github.com/flyhero/antumi) | 24 | Local CLI detection, chat, task board and quotas | Agent handoff carries visible text; returning agent resumes its native session; model selection | No documented phone client | Apache-2.0 |

## Terminal workspaces and phone bridges (10)

| Project | Stars | CLI integration / role | Agent / model boundary | Phone / status | License |
| --- | --- | --- | --- | --- | --- |
| [warpdotdev/warp](https://github.com/warpdotdev/warp) | 65,692 | Agentic terminal with built-in agent and external CLI support | External CLI execution does not establish cross-agent native-session migration | Remote-access features depend on service | AGPL-3.0 / MIT components |
| [herdrdev/herdr](https://github.com/herdrdev/herdr) | 45,785 | Persistent terminal runtime; detects running agent activity | Process/state detection differs from installation scanning; model changes belong to each CLI | SSH; community clients Ovis / Collie | Apache-2.0 |
| [manaflow-ai/cmux](https://github.com/manaflow-ai/cmux) | 28,397 | macOS terminal, workspaces, browser and agent notifications | Separate CLI processes; same-chat handoff unverified; client/server licenses differ | Paid iOS TestFlight beta | GPL-3.0-or-later client; BUSL server directories |
| [chenhg5/cc-connect](https://github.com/chenhg5/cc-connect) | 16,085 | Bridges installed CLI agents to messaging services | /switch selects sessions; /provider selects API service, not CLI engine handoff | WeChat / Feishu / Telegram / others | MIT |
| [smtg-ai/claude-squad](https://github.com/smtg-ai/claude-squad) | 8,666 | tmux + worktree manager for multiple local CLI agents | Session profiles; cross-agent same-chat handoff unverified | No dedicated phone client confirmed | AGPL-3.0 |
| [amantus-ai/vibetunnel](https://github.com/amantus-ai/vibetunnel) | 4,697 | Browser remote control for terminal sessions | Wraps arbitrary commands; not structured multi-agent conversation migration | Browser; latest release is beta | MIT |
| [SeemSeam/claude_codex_bridge](https://github.com/SeemSeam/claude_codex_bridge) | 3,594 | Visible multi-CLI collaboration via tmux / WezTerm | Agent/window switching and messaging; same-session engine handoff unverified | Android controller APK | AGPL-3.0 |
| [agent-of-empires/agent-of-empires](https://github.com/agent-of-empires/agent-of-empires) | 3,381 | Multi-CLI TUI + Web with tmux, worktrees and diffs | Per-session agents; cross-agent handoff unverified; Windows via WSL2 | Mobile browser | MIT |
| [standardagents/dmux](https://github.com/standardagents/dmux) | 1,807 | tmux/worktree multiplexer for parallel CLI agents | Multi-agent launch and native resume; cross-agent migration unverified | No dedicated phone client confirmed | MIT |
| [K9i-0/ccpocket](https://github.com/K9i-0/ccpocket) | 1,092 | Phone/desktop client for local Claude and Codex bridge | Claude subscription login needs explicit bridge option; same-session cross-agent switch unverified | iOS / Android; macOS app | MIT |

## Task and team control planes (4)

| Project | Stars | CLI integration / role | Agent / model boundary | Phone / status | License |
| --- | --- | --- | --- | --- | --- |
| [paperclipai/paperclip](https://github.com/paperclipai/paperclip) | 107,136 | Tasks, roles, budgets, approvals and local CLI adapters | Agent configuration and session resume; same-chat engine switching unverified; chat experimental | Mobile-ready management UI | MIT |
| [OpenHands/OpenHands](https://github.com/OpenHands/OpenHands) | 91,788 | Agent Canvas runs OpenHands and third-party CLI/ACP agents | Local / Docker / remote backends; model profiles; no verified original-CLI cross-agent migration | Web frontend; native phone app unverified | MIT core; check enterprise components |
| [humanlayer/humanlayer](https://github.com/humanlayer/humanlayer) | 12,458 | Machine daemons and Claude/Codex/OpenCode/Pi team workspace | Tasks/plans/reviews; same-session engine switch unverified; self-host guide incomplete | Desktop / Web; phone support unverified | Apache-2.0 |
| [builderz-labs/mission-control](https://github.com/builderz-labs/mission-control) | 6,395 | Self-hosted tasks, run review, spend and runtime discovery | Adapter depth varies; live session messaging needs gateway; schema/API alpha | Dedicated phone support unverified | MIT |

## Adjacent tools: different execution models or scope (12)

| Project | Stars | CLI integration / role | Agent / model boundary | Phone / status | License |
| --- | --- | --- | --- | --- | --- |
| [anomalyco/opencode](https://github.com/anomalyco/opencode) | 221,373 | Own coding agent with terminal, desktop and IDE interfaces | Multi-model backend, not a wrapper discovering Claude/Codex CLIs | Server / Web paths; inspect deployment | MIT |
| [farion1231/cc-switch](https://github.com/farion1231/cc-switch) | 148,507 | CLI installation, providers, MCP, skills and session tools | Configuration manager; restore uses CLI commands; sync does not mean phone control | No verified conversation remote control | MIT |
| [aaif-goose/goose](https://github.com/aaif-goose/goose) | 55,685 | Own agent plus Claude/Codex ACP providers | ACP resume/fork limitations; old mobile tunnel removed from current Desktop | Roaming is experimental, not old mobile pairing | Apache-2.0 |
| [CherryHQ/cherry-studio](https://github.com/CherryHQ/cherry-studio) | 52,961 | Chat/knowledge/agents; Code Mate detects and launches local CLIs | Code Mate opens system terminals; mobile pairing imports configuration only | Mobile apps; no paired history or agent control | AGPL-3.0 |
| [different-ai/openwork](https://github.com/different-ai/openwork) | 24,252 | Cowork desktop built on OpenCode; skills, MCP and many models | External CLI MCP integration is not local multi-CLI orchestration | Phone continuity unverified | MIT core; enterprise directory separate |
| [winfunc/opcode](https://github.com/winfunc/opcode) | 22,420 | Claude Code GUI; renamed from Claudia | Claude-only; v0.2.0 release dates to 2025-08-31; do not count old name twice | No verified phone control | AGPL-3.0 |
| [YishenTu/claudian](https://github.com/YishenTu/claudian) | 15,791 | Multi-CLI agent plugin inside Obsidian | Desktop Obsidian dependency; shared memory is not native-session migration | Desktop only | MIT |
| [eigent-ai/eigent](https://github.com/eigent-ai/eigent) | 15,657 | CAMEL-powered desktop cowork and specialist agent workforce | Own agent framework; installed Claude/Codex CLI orchestration unverified | Phone control unverified | Apache-2.0 |
| [NanmiCoder/cc-haha](https://github.com/NanmiCoder/cc-haha) | 15,159 | Bundled agent desktop, worktrees, teams and computer use | Bundled claude-haha engine; commercial software/service work requires license review | H5 / WeChat / Feishu / DingTalk | Custom Community Source |
| [fathah/hermes-desktop](https://github.com/fathah/hermes-desktop) | 14,453 | Desktop companion focused on Hermes Agent | Single-agent focus; not a general installed Claude/Codex CLI workspace | Not verified in this survey | MIT |
| [stagewise-io/stagewise](https://github.com/stagewise-io/stagewise) | 6,831 | Own agentic IDE with live browser and debugging tools | BYOK/API models; installed Claude/Codex CLI orchestration unverified | Phone control unverified | AGPL-3.0 |
| [coder/xum](https://github.com/coder/xum) | 2,062 | Xum, formerly Mux; local/SSH workspaces and multiple models | Own agent loop, not a Claude/Codex CLI shell | Responsive server-mode Web UI | AGPL-3.0 |

## Deprecated, archived, or sunsetting references (4)

| Project | Stars | CLI integration / role | Agent / model boundary | Phone / status | License |
| --- | --- | --- | --- | --- | --- |
| [BloopAI/vibe-kanban](https://github.com/BloopAI/vibe-kanban) | 28,446 | Task/worktree/review workspace for multiple coding agents | Company shutdown announced 2026-04-10; community/local continuation | Old hosted remote services retired | Apache-2.0 |
| [21st-dev/1code](https://github.com/21st-dev/1code) | 5,574 | Claude/Codex workspace using bundled runtimes | Archived 2026-07-07; cross-agent action creates new chat with history | Cloud-agent PWA, not verified local-session control | Apache-2.0 |
| [stravu/crystal](https://github.com/stravu/crystal) | 3,133 | Former Claude/Codex session and worktree manager | Deprecated February 2026; successor is Nimbalyst; not archived does not mean maintained | Use successor's documented capabilities | MIT |
| [sugyan/claude-code-webui](https://github.com/sugyan/claude-code-webui) | 1,137 | Claude-only browser UI | Archived 2026-05-29; not a current multi-CLI alternative | Browser | MIT |

## Small projects and observability: retain, do not rank as high-star peers (6)

| Project | Stars | CLI integration / role | Agent / model boundary | Phone / status | License |
| --- | --- | --- | --- | --- | --- |
| [rebornix/Agmente](https://github.com/rebornix/Agmente) | 547 | iOS client for ACP / Codex app-server | Remote protocol client; desktop CLI discovery and engine handoff unverified | iOS | See repository license |
| [kzahel/yepanywhere](https://github.com/kzahel/yepanywhere) | 539 | Detects local CLIs and sessions; phone Web client | Claude/Codex primary; others experimental; cross-agent handoff unverified | Web; native mobile in development/plans | MIT |
| [formulahendry/acp-ui](https://github.com/formulahendry/acp-ui) | 502 | Cross-platform ACP client, desktop/Web/Android | Adapters configured separately; phone/Web require remote WebSocket | Android APK; iOS source build | MIT |
| [pugliatechs/polpo](https://github.com/pugliatechs/polpo) | 46 | Multi-CLI phone dashboard and session browser | Very small project; no verified cross-agent context migration | Web dashboard | MIT |
| [Ericonaldo/AgentMonitor](https://github.com/Ericonaldo/AgentMonitor) | 35 | Claude/Codex execution and monitoring dashboard | Very small project; no license identified by GitHub metadata | Browser / relay | License not identified |
| [CHATS-lab/VibeLens](https://github.com/CHATS-lab/VibeLens) | 21 | Local multi-agent transcript replay and analytics | Observability only; not execution/control; low-star auxiliary tool | Not verified | MIT |

## Critical evidence and version boundaries

1. **Agent Orchestrator:** [v0.14.6 release](https://github.com/OrchestratorInc/agent-orchestrator/releases/tag/v0.14.6) ships agent switching outside Developer mode. [Switching rules](https://docs.orchestrator.inc/guides/per-role-agents/#switch-agents-mid-session) require an idle local session; cloud sessions cannot switch. [Tagged handoff implementation](https://github.com/OrchestratorInc/agent-orchestrator/blob/v0.14.6/backend/internal/domain/handoff_note.go) budgets/truncates history and allows retrieval of saved history; it is not native-state migration.
2. **T3 Code:** [v0.1.2 handoff contract](https://github.com/pingdotgg/t3code/blob/v0.1.2/docs/user/portable-handoffs.md) carries selected conversation history within the app thread; reasoning, tool-call state, and attachments are excluded. [Tagged README](https://github.com/pingdotgg/t3code/blob/v0.1.2/README.md) documents local CLIs and mobile apps. Older internal summaries can disagree with this updated user contract.
3. **Antumi / Happier / CodePilot:** [Antumi architecture](https://github.com/flyhero/antumi/blob/main/docs/ARCHITECTURE.md) explains installed-CLI checks and visible-history handoff. [Happier's continuation page](https://docs.happier.dev/sessions/continue-with-another-agent) explicitly marks cross-agent continuation unreleased. [CodePilot v0.67.17 design](https://github.com/op7418/CodePilot/blob/v0.67.17/docs/insights/runtime-thread-ownership-and-handoff.md) explicitly locks runtime ownership after first execution.
4. **Paseo / bb:** [Paseo providers](https://paseo.sh/docs/providers) documents native discovery; its catalog's [third-party switch-provider plugin](https://paseo.sh/plugins/anh-chu/switch-provider) starts another agent and may convert or summarize history. [bb's stable handoff implementation](https://github.com/get-bb/bb/blob/desktop-v0.47.1/packages/client-core/src/prompt/thread-handoff-request.ts) creates a new thread with an old-thread reference and reused environment.
5. **Multica:** [README](https://github.com/multica-ai/multica#readme) covers automatic desktop runtime/tool discovery; [provider docs](https://multica.ai/docs/providers) describe resuming each tool's saved session, not confirmed cross-tool migration. [Agent configuration](https://multica.ai/docs/agents-create) applies model changes to later runs. [Mobile docs](https://multica.ai/docs/mobile-app) distinguish source-build iOS from an App Store release.
6. **Other local workspaces:** [Emdash providers](https://emdash.com/docs/providers), [Ekko native CLI modes](https://github.com/EKKOLearnAI/ekko-studio/blob/main/docs/native-coding-agents.md), [Nimbalyst mobile](https://nimbalyst.com/mobile-agent-management/), and [Maestro README](https://github.com/RunMaestro/Maestro#readme) support the integration/mobile distinctions in their rows. Codeg and Ghostex advertise handoff, but exact same-session semantics were not verified here.
7. **Phone limitations:** [Orca mobile](https://www.onorca.dev/docs/mobile) is beta; [Superset](https://github.com/superset-sh/superset#readme) requires Pro and iOS/iPadOS 26+. [HAPI v0.30.7 config contract](https://github.com/tiann/hapi/blob/v0.30.7/docs/api/client-contract/rest.md#session-config--mode--model--effort-per-flavor) documents Claude/Codex model-control restrictions. [Cherry mobile](https://github.com/CherryHQ/cherry-studio-app#-made-for-mobile-connected-to-cherry) imports configuration, not desktop history/control. [goose mobile](https://goose-docs.ai/docs/experimental/remote-access/mobile-access/) explains removal of the old tunnel. [cmux pricing](https://cmux.com/pricing) places iOS in paid early access.
8. **Alternative execution models:** [Happy harnesses](https://happy.engineering/recepies/harnesses/) distinguishes its default agent loop from native harnesses. [Cherry Code Mate](https://www.cherryai.com/docs/en/cherrystudio/preview/code-cli/) detects local CLIs but launches system terminals. [cc-connect v1.5.0](https://github.com/chenhg5/cc-connect/blob/v1.5.0/README.md) distinguishes session/API-provider commands. [Herdr agent detection](https://herdr.dev/docs/agents/) identifies running terminal activity; it is not an installation scanner.

## Licensing and lifecycle checks

The MIT license of this catalog does not license the linked tools. GitHub's `licenseInfo` is a discovery hint; read current license text, component scope, and tagged versions before treating a project as permissively licensed.

- **Source-available / mixed terms:** [Multica](https://github.com/multica-ai/multica/blob/main/LICENSE), [Superset](https://github.com/superset-sh/superset/blob/main/LICENSE.md), [Ekko](https://github.com/EKKOLearnAI/ekko-studio/blob/main/LICENSE), [CodePilot](https://github.com/op7418/CodePilot/blob/v0.67.17/LICENSE), [Supacode](https://github.com/supabitapp/supacode/blob/main/LICENSE), [cmux](https://github.com/manaflow-ai/cmux/blob/main/LICENSE), and [cc-haha](https://github.com/NanmiCoder/cc-haha/blob/main/LICENSING.md) have restrictions or component-specific terms. cc-haha's restrictions also cover commercial development/service work. [Golutra](https://github.com/golutra/golutra/blob/master/LICENSE) has commercial-wording differences between README and license; do not infer a grant from marketing copy.
- **Aliases and duplicates:** `getAsterisk/claudia` redirects to **winfunc/opcode**; `coder/mux` redirects to **coder/xum**; `block/goose` redirects to **aaif-goose/goose**. Count each canonical project once.
- **Maintenance:** [Crystal](https://github.com/stravu/crystal#readme) is deprecated in favor of Nimbalyst despite not being archived; [1Code](https://github.com/21st-dev/1code) is archived. [Vibe Kanban's shutdown announcement](https://www.vibekanban.com/blog/shutdown) describes community/local continuation. [Opcode v0.2.0](https://github.com/winfunc/opcode/releases/tag/v0.2.0) proves downloads exist despite stale README copy, but dates to 2025. Archived/sunset projects remain references, not default recommendations.

Frameworks, skill collections, API gateways, usage-only dashboards, and generic remote-desktop products were screened out of the core comparison unless a directly relevant UI or bridge justified an adjacent row. Small projects stay visible without being presented as high-star recommendations.
