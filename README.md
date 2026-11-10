<div align="center">

# 🚀 Awesome Agent-Native IDE

### A curated, ranked comparison of IDEs and orchestrators built for the AI coding agent era.

<p>
  <a href="README.md">English</a> ·
  <a href="README.ko.md">한국어</a> ·
  <a href="README.ja.md">日本語</a> ·
  <a href="README.zh-CN.md">简体中文</a> ·
  <a href="README.es.md">Español</a>
</p>

[![GitHub stars](https://img.shields.io/github/stars/pinion05/awesome-agent-ide?style=for-the-badge&logo=github)](https://github.com/pinion05/awesome-agent-ide)
[![License](https://img.shields.io/badge/CC0-1.0-blue?style=for-the-badge)](LICENSE)
[![Last Updated](https://img.shields.io/badge/Updated-2026--07-lightgrey?style=for-the-badge)](#)
[![Website](https://img.shields.io/badge/🌐%20Website-GitHub%20Pages-success?style=for-the-badge)](https://pinion05.github.io/awesome-agent-ide/)

</div>

---

## 📖 What is an Agent-Native IDE?

Traditional IDEs (Cursor, Windsurf, VS Code) bolt AI features onto an existing editor. **Agent-Native IDEs** are built from the ground up to run, manage, and review **multiple CLI coding agents** (Claude Code, Codex, Gemini CLI, etc.) in parallel.

The defining characteristics:

| Feature | Description |
|---------|-------------|
| **Git Worktree Isolation** | Each agent gets its own branch and working directory, sharing one `.git` database |
| **Multi-Agent Parallel Execution** | Run 5–20+ agents simultaneously, monitored from one screen |
| **Diff Review + Merge Workflow** | Review agent-generated changes in one place before merging |
| **BYOA (Bring Your Own Agent)** | Run any CLI agent with your own subscription — no vendor lock-in |

> **Not covered here:** Traditional IDEs with AI bolted on (Cursor, Windsurf, Copilot). Those are excellent tools, but this list focuses on tools whose *primary purpose* is agent orchestration.

---

## 🏆 Ranking Overview

| Rank | Tool | Score | Platform | License | Stars | One-Liner |
|:----:|------|:-----:|----------|---------|:-----:|-----------|
| 🥇 | [**Orca**](https://github.com/stablyai/orca) | **8.6** | macOS·Win·Linux·📱 | MIT | 18.3K | Full cross-platform + mobile, Design Mode, daily releases |
| 🥈 | [**Emdash**](https://github.com/generalaction/emdash) | **8.3** | macOS·Win·Linux | Apache-2.0 | 5.1K | Port injection, 12 ticket integrations, 34 agents |
| 🥉 | [**Superset**](https://github.com/superset-sh/superset) | **7.5** | macOS | Other | 12.4K | CLI + SDK + MCP, automations, broadest agent support |
| 4 | [**cmux**](https://github.com/manaflow-ai/cmux) | **7.0** | macOS | Other | 24.4K | Native Swift performance, largest community, terminal-first |
| 5 | [**Parallel Code**](https://github.com/johannesjo/parallel-code) | **6.7** | macOS·Linux | MIT | 0.8K | Docker sandboxing, AI Arena, coverage radar |
| 6 | [**Claude Squad**](https://github.com/smtg-ai/claude-squad) | **6.5** | macOS·Linux | AGPL-3.0 | 8.1K | Best stability (0.6% issue ratio), fastest setup |
| 7 | [**Vibe Kanban**](https://github.com/BloopAI/vibe-kanban) | **6.3** | Web | Apache-2.0 | — | Kanban + MCP auto-decomposition (community-maintained) |
| 8 | [**Nimbalyst**](https://nimbalyst.com/) | **6.2** | Cross-platform·📱 | MIT | — | Worktree-first sessions, visual editing, iOS companion |
| 9 | [**Intent**](https://www.intentapp.dev/) | **6.1** | macOS | Closed | — | Spec-driven coordination, Coordinator/Verifier agents |
| 10 | [**Conductor**](https://www.conductor.build/) | **5.7** | macOS | Closed | — | Best Mac polish, free, BYO login |

---

## 📊 Scoring Methodology

Each tool is scored on **7 dimensions** (1–10 scale), weighted to produce a composite score.

| Dimension | Weight | What We Evaluate |
|-----------|:------:|------------------|
| **Technical Depth** | 20% | Isolation model (worktree/container), coordination depth, architecture quality, unique tech (Design Mode, Computer Use, port injection) |
| **Stability** | 15% | Issue-to-star ratio, release cadence, codebase maturity, runtime stability (native vs Electron) |
| **UX / Convenience** | 15% | Setup ease, visual diff review, keyboard shortcuts, notification system, workflow polish |
| **Ecosystem** | 15% | Supported agents, ticket integrations (Linear/GitHub/Jira), CLI/SDK/MCP availability, community size |
| **Scalability** | 15% | Remote execution (SSH), mobile companion, parallel capacity, programmability |
| **Platform Support** | 10% | OS coverage (macOS / Windows / Linux / mobile) |
| **Open Source Health** | 10% | License freedom, vendor independence, community-driven development |

### Detailed Scores

| Tool | Technical (20%) | Stability (15%) | UX (15%) | Ecosystem (15%) | Scalability (15%) | Platform (10%) | OSS (10%) | **Total** |
|------|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| **Orca** | 9 | 7 | 9 | 8 | 9 | 10 | 8 | **8.6** |
| **Emdash** | 8 | 7 | 8 | 9 | 8 | 10 | 9 | **8.3** |
| **Superset** | 8 | 8 | 8 | 9 | 8 | 3 | 6 | **7.5** |
| **cmux** | 8 | 6 | 8 | 8 | 7 | 3 | 7 | **7.0** |
| **Parallel Code** | 7 | 7 | 7 | 6 | 6 | 6 | 8 | **6.7** |
| **Claude Squad** | 6 | 9 | 6 | 7 | 5 | 6 | 6 | **6.5** |
| **Vibe Kanban** | 7 | 4 | 7 | 7 | 5 | 8 | 6 | **6.3** |
| **Nimbalyst** | 7 | 5 | 7 | 5 | 6 | 8 | 5 | **6.2** |
| **Intent** | 9 | 5 | 7 | 6 | 7 | 3 | 2 | **6.1** |
| **Conductor** | 7 | 7 | 8 | 5 | 5 | 3 | 2 | **5.7** |

---

## 🔍 Detailed Analysis

### 🥇 1. Orca — stablyai/orca

| | |
|---|---|
| **GitHub** | [stablyai/orca](https://github.com/stablyai/orca) |
| **Stars / Forks / Issues** | 18,327 / 1,448 / 1,361 (7.4%) |
| **Language** | TypeScript (Electron) |
| **License** | MIT |
| **Platform** | macOS · Windows · Linux · iOS · Android |
| **Website** | [onorca.dev](https://www.onorca.dev/) |

**✅ Strengths**
- **Only full cross-platform + mobile** — iOS/Android companion app for monitoring and follow-ups from anywhere
- **Design Mode** — Click any UI element in a real Chromium window; HTML/CSS/screenshot sent straight to the agent's prompt. Unique to Orca.
- **SSH Worktrees** — Run agents on a beefy remote box with auto-reconnect and port forwarding
- **Computer Use** — Agents can operate desktop apps and visible UI
- **GitHub & Linear native** — Browse PRs, issues, and boards in-app; open a worktree from any task
- **Annotate AI Diffs** — Drop comments on any diff line, ship them back to the agent
- **Daily releases** — Ships every day; the changelog is the real feature list
- Ghostty-class terminals (WebGL), infinite splits, scrollback that survives restarts

**❌ Weaknesses**
- Electron-based — heavier than native alternatives (cmux)
- 1,361 open issues — active but management burden is real
- MIT but stablyai-led — single vendor dependency

> **Best for:** Distributed teams needing mobile monitoring, cross-platform support, and the richest agent-native feature set.

---

### 🥈 2. Emdash — generalaction/emdash

| | |
|---|---|
| **GitHub** | [generalaction/emdash](https://github.com/generalaction/emdash) |
| **Stars / Forks / Issues** | 5,149 / 534 / 132 (2.6%) |
| **Language** | TypeScript (Electron) |
| **License** | Apache-2.0 |
| **Platform** | macOS · Windows · Linux |
| **Website** | [emdash.ai](https://emdash.ai/) |
| **Backing** | YC W26 |

**✅ Strengths**
- **Broadest ticket integration** — Linear, GitHub, Jira, GitLab, Asana, Monday.com, Trello, Plane, Forgejo, Featurebase, Plain, Notion (12 platforms)
- **`$EMDASH_PORT` injection** — Solves the port-collision problem at the config level, which almost no other tool handles
- **Broadest agent support** — 34 CLI providers auto-detected (Claude Code, Codex, Cursor, OpenCode, Amp, Devin, Qwen Code, Droid, Copilot, etc.)
- **SSH/SFTP remote projects** — Same parallel workflow on remote codebases, OS keychain auth
- **Local-first + privacy** — SQLite local storage, no code/chat sent to Emdash servers
- Cross-platform + Apache-2.0 — most permissive license combination
- Issue/star ratio 2.6% — excellent stability indicator

**❌ Weaknesses**
- No mobile companion app
- No agent-to-agent coordination — each runs independently
- Launched early 2026; community still growing

> **Best for:** Enterprise teams needing ticket integration, port isolation, and cross-platform support with strong privacy guarantees.

---

### 🥉 3. Superset — superset-sh/superset

| | |
|---|---|
| **GitHub** | [superset-sh/superset](https://github.com/superset-sh/superset) |
| **Stars / Forks / Issues** | 12,399 / 1,076 / 323 (2.6%) |
| **Language** | TypeScript (Electron) |
| **License** | Other |
| **Platform** | macOS |
| **Website** | [superset.sh](https://superset.sh/) |
| **Backing** | YC |

**✅ Strengths**
- **Most access surfaces** — Desktop app + CLI + TypeScript SDK + MCP server. Control workspaces from anywhere.
- **Broadest agent support** — Amp, Claude Code, Codex, Cursor, Droid, Gemini, Copilot, Mastra, Mistral Vibe, OpenCode, Pi, Polygraph + custom agents
- **Automations** — Schedule agent sessions to run on a timer
- **Slack & Linear integration** — Spin up workspaces from Slack messages or Linear issues
- **In-app browser + port detection** — Preview dev servers per workspace
- Custom agent support with icons, workspace presets
- Issue/star ratio 2.6% — good stability

**❌ Weaknesses**
- **macOS only** — No Windows/Linux builds. The most critical weakness.
- Requires Bun runtime, Caddy, and other external dependencies
- "Other" license — open-source freedom unclear
- iOS app still "coming soon"

> **Best for:** macOS developers who want maximum programmability (CLI + SDK + MCP) and the broadest agent ecosystem.

---

### 4. cmux — manaflow-ai/cmux

| | |
|---|---|
| **GitHub** | [manaflow-ai/cmux](https://github.com/manaflow-ai/cmux) |
| **Stars / Forks / Issues** | 24,412 / 1,970 / 3,446 (14.1%) |
| **Language** | Swift (native macOS) |
| **License** | Other (GPL-3.0 + commercial dual) |
| **Platform** | macOS |
| **Website** | [cmux.com](https://cmux.com/) |

**✅ Strengths**
- **Most GitHub stars (24.4K)** — largest community
- **Native performance** — Swift/AppKit + libghostty GPU rendering. Blows Electron away on startup speed and memory.
- **Clear philosophy** — "A primitive, not a solution." Doesn't force a workflow on you.
- **Notification system** — OSC 9/99/777 sequence detection, blue ring + tab highlight, `cmux notify` CLI
- **In-app browser** — agent-browser API ported; accessibility tree snapshots, click, fill, JS eval
- **SSH** — `cmux ssh user@remote` creates remote workspaces; browser routes through remote network
- **Claude Code Teams** — `cmux claude-teams` one-command teammate mode, no tmux needed
- Ghostty config compatible — existing themes/fonts/colors just work
- Full CLI + socket API for automation

**❌ Weaknesses**
- **macOS only** — lowest platform score
- **It's a terminal, not an IDE** — no built-in worktree management, diff viewer, or PR creation
- **3,446 open issues (14.1%)** — highest ratio; complex native app management burden
- No mobile companion

> **Best for:** macOS power users who want native performance and a terminal-first, non-prescriptive approach. Pair with Orca/Emdash/Superset for diff review.

---

### 5. Parallel Code — johannesjo/parallel-code

| | |
|---|---|
| **GitHub** | [johannesjo/parallel-code](https://github.com/johannesjo/parallel-code) |
| **Stars / Forks / Issues** | 838 / 111 / 39 (4.7%) |
| **Language** | TypeScript (Electron + SolidJS) |
| **License** | MIT |
| **Platform** | macOS · Linux |
| **Website** | [parallelcode.app](https://parallelcode.app/) |

**✅ Strengths**
- **Docker sandboxing** — Project-specific `.parallel-code/Dockerfile` for full isolation. No other OSS tool has this.
- **AI Arena** — Race agents head-to-head, merge the winner
- **Coverage radar** — Per-file test-coverage badges in the Changed Files panel
- **Steps tracking panel** — Engineering-manager-style timeline of agent progress
- Mobile monitoring via QR code (Wi-Fi/Tailscale)
- 10 themes, keyboard-first, focus mode
- MIT license, completely free

**❌ Weaknesses**
- Smallest community (838★) — long-term maintenance uncertain
- No Windows support
- No SSH/remote worktrees
- Single-developer project (johannesjo)

> **Best for:** Developers experimenting with Docker-isolated agents and head-to-head agent competition.

---

### 6. Claude Squad — smtg-ai/claude-squad

| | |
|---|---|
| **GitHub** | [smtg-ai/claude-squad](https://github.com/smtg-ai/claude-squad) |
| **Stars / Forks / Issues** | 8,108 / 585 / 52 (0.6%) |
| **Language** | Go (TUI) |
| **License** | AGPL-3.0 |
| **Platform** | macOS · Linux (tmux required) |
| **Website** | [smtg-ai.github.io/claude-squad](https://smtg-ai.github.io/claude-squad/) |

**✅ Strengths**
- **Best stability** — 0.6% issue/star ratio, Go binary, simple architecture (tmux + worktree)
- **Fastest setup** — `brew install claude-squad` → 6 sessions in 5 seconds
- Keyboard-first TUI with vim-style navigation
- Supports Claude Code, Codex, Aider, Gemini, OpenCode, Amp
- `--autoyes` flag for unattended auto-accept (experimental)

**❌ Weaknesses**
- **Weak visual diff review** — need a separate tool for the review step
- **No remote/SSH/mobile** — local single machine only
- AGPL-3.0 — legal review needed for commercial embedding
- No Windows support (tmux dependency)

> **Best for:** Terminal power users who want the fastest, most stable path to parallel agents. Solo developers on macOS/Linux.

---

### 7. Vibe Kanban — BloopAI/vibe-kanban

| | |
|---|---|
| **GitHub** | [BloopAI/vibe-kanban](https://github.com/BloopAI/vibe-kanban) |
| **Language** | Rust (Web app) |
| **License** | Apache-2.0 |
| **Platform** | Web (cross-platform) |
| **Status** | Community-maintained (Bloop shut down April 2026) |

**✅ Strengths**
- Kanban card = worktree = agent — intuitive metaphor
- MCP server for autonomous card decomposition (closest to autonomous task decomposition)
- 10+ agents supported, in-app browser with device emulation
- Self-hostable, team-friendly

**❌ Weaknesses**
- **Bloop shut down** — paid subscriptions refunded, cloud features wound down
- No hard task dependencies (task B waiting for task A)
- 20 worktrees → disk bloat
- Future maintenance velocity entirely depends on community contributors

> **Best for:** Teams wanting a shared visual board with MCP-driven task decomposition, comfortable with community-maintained software.

---

### 8. Nimbalyst — nimbalyst.com

| | |
|---|---|
| **Website** | [nimbalyst.com](https://nimbalyst.com/) |
| **Platform** | Cross-platform desktop + iOS + Android |
| **Predecessor** | Crystal (deprecated Feb 2026) |

**✅ Strengths**
- Worktree as a first-class session primitive — one-click option when starting a session
- Inline diffs, visual files sidebar, GUI review-and-merge
- Cross-platform + iOS companion
- Built-in markdown/Excalidraw/mockup visual editing

**❌ Weaknesses**
- Youngest project (rebranded from Crystal in Feb 2026)
- Limited community, documentation, and reputation data
- Vendor-led, MIT licensed
- Narrow agent support (Claude Code, Codex)

> **Best for:** Developers who want worktree-first session management with visual editing. Re-evaluate in 6 months as the project matures.

---

### 9. Intent — Augment Code

| | |
|---|---|
| **Website** | [intentapp.dev](https://www.intentapp.dev/) |
| **Platform** | macOS (Windows waitlist, Linux not announced) |
| **Status** | Public beta |
| **Pricing** | Augment credits ($0 trial / $20–$200/mo; BYOA free) |

**✅ Strengths**
- **Spec-driven coordination** — A living spec is the single source of truth for every agent. Edit the spec once; updates propagate to all active agents.
- **Coordinator → Implementor → Verifier** three-agent division of labor
- Shines in cross-service refactors — field renames propagate via spec
- BYOA (Claude Code, Codex, OpenCode + Auggie)
- Context Engine exposed as MCP server

**❌ Weaknesses**
- **Closed source** — no code audit, vendor lock-in
- **macOS only** — Windows waitlist, Linux not announced
- Uses Augment credits — cost overlap with existing Claude/Cursor subscriptions
- Public beta — production stability unverified

> **Best for:** Teams doing complex cross-service refactors who benefit from spec-driven coordination and are on macOS.

---

### 10. Conductor — Melty Labs

| | |
|---|---|
| **Website** | [conductor.build](https://www.conductor.build/) |
| **Platform** | macOS |
| **License** | Closed source |
| **Pricing** | Free (BYO login) |

**✅ Strengths**
- Most polished Mac dashboard — diff-first review, clean UX throughout
- Free with BYO Claude/Codex/Cursor/OpenCode login
- Best orchestrator-only tool to sit beside your existing VS Code or JetBrains setup

**❌ Weaknesses**
- **Closed source** — no code audit, vendor lock-in
- **macOS only** — cross-platform "trickling in"
- No CLI/SDK/MCP — not programmable
- No remote/SSH/mobile
- Narrow agent support (4 agents)

> **Best for:** macOS developers wanting the easiest, most polished entry point to parallel agent orchestration beside their existing editor.

---

## 🎯 Decision Guide

| Your Situation | Recommended Tool | Why |
|----------------|-------------------|-----|
| Cross-platform team, need mobile monitoring | **Orca** | Only tool with 3 OS + iOS/Android |
| Enterprise, multiple ticket systems | **Emdash** | 12 ticket platforms + port injection + privacy |
| macOS + programmable automation | **Superset** | CLI + SDK + MCP, Automations |
| macOS + native performance + terminal-first | **cmux** | Swift/AppKit, GPU rendering, notifications |
| Terminal-only, fastest possible start | **Claude Squad** | 5-second setup, best stability |
| Docker isolation + agent competition | **Parallel Code** | AI Arena, project-specific Dockerfiles |
| Spec-driven cross-service refactors | **Intent** | Living spec propagation, Coordinator/Verifier |
| Free, easiest Mac onboarding | **Conductor** | Free + BYO login, best polish |

---

## 📈 Feature Comparison Matrix

| Tool | Worktree | Diff Review | Remote/SSH | Mobile | Browser | CLI/SDK/MCP | Automations | Ticket Integration |
|------|:--------:|:-----------:|:----------:|:------:|:-------:|:-----------:|:-----------:|:-----------------:|
| **Orca** | ✅ | ✅ | ✅ | ✅ iOS+Android | ✅ Design Mode | ✅ CLI | ❌ | GitHub·Linear |
| **Emdash** | ✅ | ✅ | ✅ SSH/SFTP | ❌ | ❌ | ❌ | ❌ | 12 platforms |
| **Superset** | ✅ | ✅ | ✅ | 🔄 iOS soon | ✅ | ✅ CLI+SDK+MCP | ✅ | Slack·Linear |
| **cmux** | ❌ | ❌ | ✅ | ❌ | ✅ | ✅ CLI+Socket | ❌ | ❌ |
| **Parallel Code** | ✅ | ✅ | ❌ | ✅ QR | ❌ | ❌ | ❌ | ❌ |
| **Claude Squad** | ✅ | ⚠️ weak | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ |
| **Vibe Kanban** | ✅ | ✅ | ❌ | ❌ | ✅ | ✅ MCP | ❌ | ❌ |
| **Nimbalyst** | ✅ | ✅ | ❌ | ✅ iOS | ❌ | ❌ | ❌ | ❌ |
| **Intent** | ✅ | ✅ | ❌ | ❌ | ✅ | ✅ MCP | ❌ | ❌ |
| **Conductor** | ✅ | ✅ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ |

---

## 🌐 Broader Ecosystem

These are **not** agent-native IDEs, but they coordinate parallel CLI agents or have absorbed worktree features and are worth knowing:

| Tool | Category | Agent-Native Feature |
|------|----------|---------------------|
| [Cursor 3](https://cursor.com/) | Dedicated IDE | Agents Window with `/worktree` and `/best-of-n` commands (Apr 2026) |
| [Windsurf Wave 13](https://windsurf.com/) | Dedicated IDE | Parallel Cascade sessions with worktrees, dedicated agent terminal |
| [Google Antigravity](https://antigravity.google/) | Dedicated IDE | Multi-agent parallel workspaces, free, dynamic subagents |
| [Cline](https://cline.bot/) | VS Code Extension | Model-agnostic, open-source agent in VS Code |
| [Roo Code](https://roocode.com/) | VS Code Extension | Multi-persona agent system (Coder, Architect, Debugger) |
| [Claude Code](https://claude.com/product/claude-code) | Terminal Agent | Built-in `isolation: worktree` in subagent frontmatter |
| [Aider](https://aider.chat/) | Terminal Agent | Editor-agnostic, Git-native CLI pair programming |
| [Orkas](https://github.com/Orkas-AI/Orkas) | Desktop Orchestrator | Local-first macOS/Windows app; its Commander coordinates built-in specialist agents + Claude Code, Codex and OpenCode CLI agents (MIT; no worktree isolation) |

---

## 📅 Market Observations (July 2026)

1. **Orca and Emdash form the top tier** — both cross-platform, open-source, rich features, good stability.
2. **cmux dominates community size and performance** but is macOS-only and terminal-only (not a full IDE).
3. **Superset has the deepest feature set** but macOS-only is a critical limitation.
4. **Closed-source tools (Conductor, Intent) score lowest** on open-source freedom — a structural disadvantage.
5. **Git worktrees are the consensus isolation primitive** — every serious tool now uses them.
6. **Port collision is the next frontier** — only Emdash (`$EMDASH_PORT`) solves it at the config level.
7. **Mobile monitoring is emerging** — Orca (iOS+Android), Parallel Code (QR), Nimbalyst (iOS) lead; others have nothing.
8. **The category is consolidating** — Crystal → Nimbalyst, Bloop → community Vibe Kanban. Expect more M&A and shutdowns in H2 2026.

---

## 🤝 Contributing

Contributions are welcome! If you'd like to add a tool, update scores, or fix an inaccuracy:

1. Open an [issue](https://github.com/pinion05/awesome-agent-ide/issues) with your suggestion
2. Or submit a PR with updated data and sources

Please include **verifiable sources** (GitHub repos, documentation, review articles) for any score changes.

---

## 📄 License

[CC0-1.0](LICENSE) — Public domain. Use it however you want.

---

<div align="center">

**[🌐 View as Website](https://pinion05.github.io/awesome-agent-ide/)** · **[⭐ Star on GitHub](https://github.com/pinion05/awesome-agent-ide)**

*Last updated: July 2026 · Maintained by [pinion05](https://github.com/pinion05)*

</div>
