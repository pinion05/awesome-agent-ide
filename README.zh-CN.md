<div align="center">

# 🚀 Awesome Agent-Native IDE

### 为 AI 编程代理时代而生的 IDE 与编排器综合对比

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

## 📖 什么是 Agent-Native IDE？

传统 IDE（Cursor、Windsurf、VS Code）是将 AI 功能"附加"到现有编辑器上。而 **Agent-Native IDE** 是从零开始设计的，用于**并行运行、管理和审查多个 CLI 编程代理**（Claude Code、Codex、Gemini CLI 等）的环境。

核心特征：

| 功能 | 描述 |
|---------|-------------|
| **Git Worktree 隔离** | 每个代理拥有独立的分支和工作目录，共享同一个 `.git` 数据库 |
| **多代理并行执行** | 在一个界面中同时监控 5–20+ 个代理 |
| **Diff 审查 + 合并工作流** | 在一处审查代理生成的变更后再合并 |
| **BYOA（自带代理）** | 用自己的订阅运行任何 CLI 代理 — 无供应商锁定 |

> **不在范围内：** 附加了 AI 的传统 IDE（Cursor、Windsurf、Copilot）。它们是优秀的工具，但本列表聚焦于*主要目的是代理编排*的工具。

---

## 🏆 综合排名

| 排名 | 工具 | 分数 | 平台 | 许可证 | Stars | 一句话 |
|:----:|------|:-----:|----------|---------|:-----:|-----------|
| 🥇 | [**Orca**](https://github.com/stablyai/orca) | **8.6** | macOS·Win·Linux·📱 | MIT | 18.3K | 全跨平台 + 移动端，Design Mode，每日发布 |
| 🥈 | [**Emdash**](https://github.com/generalaction/emdash) | **8.3** | macOS·Win·Linux | Apache-2.0 | 5.1K | 端口注入，12个工单集成，34 代理 |
| 🥉 | [**Superset**](https://github.com/superset-sh/superset) | **7.5** | macOS | Other | 12.4K | CLI + SDK + MCP，自动化，最广代理支持 |
| 4 | [**cmux**](https://github.com/manaflow-ai/cmux) | **7.0** | macOS | Other | 24.4K | 原生 Swift 性能，最大社区，终端优先 |
| 5 | [**Parallel Code**](https://github.com/johannesjo/parallel-code) | **6.7** | macOS·Linux | MIT | 0.8K | Docker 沙箱，AI Arena，覆盖率雷达 |
| 6 | [**Claude Squad**](https://github.com/smtg-ai/claude-squad) | **6.5** | macOS·Linux | AGPL-3.0 | 8.1K | 最佳稳定性（0.6%），最快设置 |
| 7 | [**Vibe Kanban**](https://github.com/BloopAI/vibe-kanban) | **6.3** | Web | Apache-2.0 | — | 看板 + MCP 自动分解（社区维护） |
| 8 | [**Nimbalyst**](https://nimbalyst.com/) | **6.2** | 跨平台·📱 | MIT | — | Worktree 一等公民，可视化编辑，iOS 伴侣 |
| 9 | [**Intent**](https://www.intentapp.dev/) | **6.1** | macOS | 闭源 | — | 规格驱动协调，Coordinator/Verifier 代理 |
| 10 | [**Conductor**](https://www.conductor.build/) | **5.7** | macOS | 闭源 | — | Mac 最佳打磨，免费，自带登录 |

---

## 📊 评分方法

每个工具按 **7 个维度**评分（1–10 分），加权计算综合分数。

| 维度 | 权重 | 评估内容 |
|-----------|:------:|------------------|
| **技术深度** | 20% | 隔离模型（worktree/container）、协调深度、架构质量、独特技术（Design Mode、Computer Use、端口注入） |
| **稳定性** | 15% | issue/star 比率、发布频率、代码库成熟度、运行时稳定性（原生 vs Electron） |
| **UX / 便利性** | 15% | 安装便捷性、可视化 diff 审查、键盘快捷键、通知系统、工作流打磨 |
| **生态系统** | 15% | 支持的代理、工单集成（Linear/GitHub/Jira）、CLI/SDK/MCP 可用性、社区规模 |
| **可扩展性** | 15% | 远程执行（SSH）、移动伴侣、并行容量、可编程性 |
| **平台支持** | 10% | OS 覆盖（macOS / Windows / Linux / 移动端） |
| **开源健康度** | 10% | 许可证自由度、供应商独立性、社区驱动程度 |

### 详细分数

| 工具 | 技术深度 (20%) | 稳定性 (15%) | UX (15%) | 生态系统 (15%) | 可扩展性 (15%) | 平台 (10%) | 开源 (10%) | **总分** |
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

## 🔍 工具详细分析

### 🥇 1. Orca — stablyai/orca

| | |
|---|---|
| **GitHub** | [stablyai/orca](https://github.com/stablyai/orca) |
| **Stars / Forks / Issues** | 18,327 / 1,448 / 1,361 (7.4%) |
| **语言** | TypeScript (Electron) |
| **许可证** | MIT |
| **平台** | macOS · Windows · Linux · iOS · Android |
| **网站** | [onorca.dev](https://www.onorca.dev/) |

**✅ 优点**
- **唯一全跨平台 + 移动端** — iOS/Android 伴侣应用，随时随地监控代理并发送后续指令
- **Design Mode** — 在真实 Chromium 窗口中点击任意 UI 元素，HTML/CSS/截图直接发送到代理提示词。Orca 独有功能
- **SSH Worktree** — 在远程机器上运行代理，自动重连 + 端口转发
- **Computer Use** — 代理可操作桌面应用和可见 UI
- **GitHub & Linear 原生** — 应用内浏览 PR/issue/看板，从任何任务打开 worktree
- **标注 AI Diff** — 在任意 diff 行添加评论，发送回代理
- **每日发布** — 每天发布功能，changelog 就是真正的功能列表
- Ghostty 级终端（WebGL），无限分屏，重启后保留滚动历史

**❌ 缺点**
- 基于 Electron — 比原生方案（cmux）内存更大、启动更慢
- 1,361 个未解决 issue — 活跃但管理负担确实存在
- MIT 但由 stablyai 主导 — 单一供应商依赖

> **推荐：** 需要移动监控、跨平台支持和最丰富 agent-native 功能集的分布式团队。

---

### 🥈 2. Emdash — generalaction/emdash

| | |
|---|---|
| **GitHub** | [generalaction/emdash](https://github.com/generalaction/emdash) |
| **Stars / Forks / Issues** | 5,149 / 534 / 132 (2.6%) |
| **语言** | TypeScript (Electron) |
| **许可证** | Apache-2.0 |
| **平台** | macOS · Windows · Linux |
| **网站** | [emdash.ai](https://emdash.ai/) |
| **支持** | YC W26 |

**✅ 优点**
- **最广工单集成** — Linear、GitHub、Jira、GitLab、Asana、Monday.com、Trello、Plane、Forgejo、Featurebase、Plain、Notion（12 个平台）
- **`$EMDASH_PORT` 注入** — 在配置层面解决端口冲突问题，几乎没有其他工具做到
- **最广代理支持** — 自动检测 34 CLI 提供商（Claude Code、Codex、Cursor、OpenCode、Amp、Devin、Qwen Code、Droid、Copilot 等）
- **SSH/SFTP 远程项目** — 在远程代码库上运行相同的并行工作流，OS 钥匙串认证
- **本地优先 + 隐私** — SQLite 本地存储，不向 Emdash 服务器发送代码/聊天
- 跨平台 + Apache-2.0 — 最宽松的许可证组合
- issue/star 比率 2.6% — 稳定性指标优秀

**❌ 缺点**
- 无移动伴侣应用
- 无代理间协调 — 各自独立运行
- 2026 年初发布 — 社区仍在成长

> **推荐：** 需要工单集成、端口隔离和跨平台支持及强隐私保障的企业团队。

---

### 🥉 3. Superset — superset-sh/superset

| | |
|---|---|
| **GitHub** | [superset-sh/superset](https://github.com/superset-sh/superset) |
| **Stars / Forks / Issues** | 12,399 / 1,076 / 323 (2.6%) |
| **语言** | TypeScript (Electron) |
| **许可证** | Other |
| **平台** | macOS |
| **网站** | [superset.sh](https://superset.sh/) |
| **支持** | YC |

**✅ 优点**
- **最丰富的访问面** — 桌面应用 + CLI + TypeScript SDK + MCP 服务器。从任何地方控制工作区
- **最广代理支持** — Amp、Claude Code、Codex、Cursor、Droid、Gemini、Copilot、Mastra、Mistral Vibe、OpenCode、Pi、Polygraph + 自定义代理
- **自动化** — 按计划运行代理会话
- **Slack & Linear 集成** — 从 Slack 消息或 Linear issue 创建工作区
- **应用内浏览器 + 端口检测** — 按工作区预览开发服务器
- 自定义代理支持（含图标），工作区预设
- issue/star 比率 2.6% — 稳定性良好

**❌ 缺点**
- **仅 macOS** — 无 Windows/Linux 构建。最致命的弱点
- 需要 Bun 运行时、Caddy 等外部依赖
- "Other" 许可证 — 开源自由度不明确
- iOS 应用仍"即将推出"

> **推荐：** 追求最大可编程性（CLI + SDK + MCP）和最广代理生态系统的 macOS 开发者。

---

### 4. cmux — manaflow-ai/cmux

| | |
|---|---|
| **GitHub** | [manaflow-ai/cmux](https://github.com/manaflow-ai/cmux) |
| **Stars / Forks / Issues** | 24,412 / 1,970 / 3,446 (14.1%) |
| **语言** | Swift (原生 macOS) |
| **许可证** | Other (GPL-3.0 + 商业双许可) |
| **平台** | macOS |
| **网站** | [cmux.com](https://cmux.com/) |

**✅ 优点**
- **GitHub Stars 最多（24.4K）** — 最大社区
- **原生性能** — Swift/AppKit + libghostty GPU 渲染。在启动速度和内存上碾压 Electron
- **明确的哲学** — "是原始工具，不是解决方案。"不强制工作流
- **通知系统** — OSC 9/99/777 序列检测，蓝色环 + 标签高亮，`cmux notify` CLI
- **应用内浏览器** — 移植 agent-browser API；无障碍树快照、点击、填充、JS 执行
- **SSH** — `cmux ssh user@remote` 创建远程工作区；浏览器通过远程网络路由
- **Claude Code Teams** — `cmux claude-teams` 一条命令启动 teammate 模式，无需 tmux
- Ghostty 配置兼容 — 现有主题/字体/颜色直接可用
- CLI + socket API 实现全面自动化

**❌ 缺点**
- **仅 macOS** — 平台分数最低
- **是终端，不是 IDE** — 无内置 worktree 管理、diff 查看器或 PR 创建
- **3,446 个未解决 issue（14.1%）** — 比率最高；复杂原生应用的管理负担
- 无移动端

> **推荐：** 追求原生性能和终端优先、非强制方式的 macOS 高级用户。diff 审查搭配 Orca/Emdash/Superset。

---

### 5. Parallel Code — johannesjo/parallel-code

| | |
|---|---|
| **GitHub** | [johannesjo/parallel-code](https://github.com/johannesjo/parallel-code) |
| **Stars / Forks / Issues** | 838 / 111 / 39 (4.7%) |
| **语言** | TypeScript (Electron + SolidJS) |
| **许可证** | MIT |
| **平台** | macOS · Linux |
| **网站** | [parallelcode.app](https://parallelcode.app/) |

**✅ 优点**
- **Docker 沙箱** — 项目特定 `.parallel-code/Dockerfile` 实现完全隔离。其他 OSS 工具没有的功能
- **AI Arena** — 代理间正面竞争，合并胜者
- **覆盖率雷达** — 变更文件面板中的每文件测试覆盖率徽章
- **步骤跟踪面板** — 代理进度的工程经理风格时间线
- 通过 QR 码移动监控（Wi-Fi/Tailscale）
- 10 个主题，键盘优先，聚焦模式
- MIT 许可证，完全免费

**❌ 缺点**
- 社区最小（838★）— 长期维护不确定
- 不支持 Windows
- 无 SSH/远程 worktree
- 单一开发者项目（johannesjo）

> **推荐：** 实验 Docker 隔离代理和正面代理竞争的开发者。

---

### 6. Claude Squad — smtg-ai/claude-squad

| | |
|---|---|
| **GitHub** | [smtg-ai/claude-squad](https://github.com/smtg-ai/claude-squad) |
| **Stars / Forks / Issues** | 8,108 / 585 / 52 (0.6%) |
| **语言** | Go (TUI) |
| **许可证** | AGPL-3.0 |
| **平台** | macOS · Linux（需要 tmux） |
| **网站** | [smtg-ai.github.io/claude-squad](https://smtg-ai.github.io/claude-squad/) |

**✅ 优点**
- **最佳稳定性** — 0.6% issue/star 比率，Go 二进制，简单架构（tmux + worktree）
- **最快设置** — `brew install claude-squad` → 5 秒内 6 个会话
- 键盘优先 TUI，vim 风格导航
- 支持 Claude Code、Codex、Aider、Gemini、OpenCode、Amp
- `--autoyes` 标志实现无人值守自动接受（实验性）

**❌ 缺点**
- **可视化 diff 审查弱** — 需要额外工具
- **无远程/SSH/移动端** — 仅本地单机
- AGPL-3.0 — 商业嵌入需法律审查
- 不支持 Windows（tmux 依赖）

> **推荐：** 追求并行代理最快、最稳定路径的终端高级用户。macOS/Linux 独立开发者。

---

### 7. Vibe Kanban — BloopAI/vibe-kanban

| | |
|---|---|
| **GitHub** | [BloopAI/vibe-kanban](https://github.com/BloopAI/vibe-kanban) |
| **语言** | Rust (Web 应用) |
| **许可证** | Apache-2.0 |
| **平台** | Web (跨平台) |
| **状态** | 社区维护（Bloop 于 2026 年 4 月关闭） |

**✅ 优点**
- 看板卡片 = worktree = 代理 — 直观的隐喻
- MCP 服务器实现卡片自动分解（最接近自主任务分解）
- 支持 10+ 代理，应用内浏览器（含设备模拟）
- 可自托管，团队友好

**❌ 缺点**
- **Bloop 已关闭** — 付费订阅退款，云功能缩减
- 不支持硬任务依赖（任务 B 等待任务 A）
- 20 个 worktree 导致磁盘膨胀
- 未来维护速度完全依赖社区贡献者

> **推荐：** 需要共享可视化看板和 MCP 驱动任务分解，对社区维护软件宽容的团队。

---

### 8. Nimbalyst — nimbalyst.com

| | |
|---|---|
| **网站** | [nimbalyst.com](https://nimbalyst.com/) |
| **平台** | 跨平台桌面 + iOS + Android |
| **前身** | Crystal（2026 年 2 月废弃） |

**✅ 优点**
- worktree 作为会话对象的一等公民 — 启动会话时一键选项
- 内联 diff，可视化文件侧栏，GUI 审查与合并
- 跨平台 + iOS 伴侣
- 内置 Markdown/Excalidraw/模型可视化编辑

**❌ 缺点**
- 最年轻的项目（2026 年 2 月从 Crystal 重命名）
- 社区、文档和声誉数据有限
- 供应商主导，MIT 许可证
- 代理支持窄（Claude Code、Codex）

> **推荐：** 需要可视化编辑和 worktree 优先会话管理的开发者。建议 6 个月后项目成熟时重新评估。

---

### 9. Intent — Augment Code

| | |
|---|---|
| **网站** | [intentapp.dev](https://www.intentapp.dev/) |
| **平台** | macOS（Windows 候补名单，Linux 未公布） |
| **状态** | 公开测试版 |
| **定价** | Augment 积分（$0 试用 / $20–$200/月; BYOA 免费） |

**✅ 优点**
- **规格驱动协调** — 活规格是每个代理的唯一真实来源。编辑一次规格，更新传播到所有活跃代理
- **Coordinator → Implementor → Verifier** 三代理分工
- 在跨服务重构中大放异彩 — 字段重命名通过规格传播
- BYOA（Claude Code、Codex、OpenCode + Auggie）
- Context Engine 作为 MCP 服务器公开

**❌ 缺点**
- **闭源** — 无法审计代码，供应商锁定
- **仅 macOS** — Windows 候补，Linux 未公布
- 使用 Augment 积分 — 与现有 Claude/Cursor 订阅费用重叠
- 公开测试版 — 生产稳定性未验证

> **推荐：** 受益于规格驱动协调并使用 macOS 的复杂跨服务重构团队。

---

### 10. Conductor — Melty Labs

| | |
|---|---|
| **网站** | [conductor.build](https://www.conductor.build/) |
| **平台** | macOS |
| **许可证** | 闭源 |
| **定价** | 免费（自带登录） |

**✅ 优点**
- macOS 上最打磨的仪表盘 — diff 优先审查，整体 UX 干净
- 免费 + 自带 Claude/Codex/Cursor/OpenCode 登录
- 放在现有 VS Code/JetBrains 旁边的最佳编排器

**❌ 缺点**
- **闭源** — 无法审计代码，供应商锁定
- **仅 macOS** — 跨平台"逐步加入中"
- 无 CLI/SDK/MCP — 不可编程
- 无远程/SSH/移动端
- 代理支持窄（4 种）

> **推荐：** 在现有编辑器旁边追求并行代理编排最简单、最打磨入口的 macOS 开发者。

---

## 🎯 按用例推荐

| 场景 | 推荐工具 | 原因 |
|----------------|-------------------|-----|
| 跨平台团队，需要移动监控 | **Orca** | 唯一支持 3 OS + iOS/Android 的工具 |
| 企业，多个工单系统 | **Emdash** | 12 个工单平台 + 端口注入 + 隐私 |
| macOS + 可编程自动化 | **Superset** | CLI + SDK + MCP，自动化 |
| macOS + 原生性能 + 终端优先 | **cmux** | Swift/AppKit，GPU 渲染，通知系统 |
| 仅终端，最快启动 | **Claude Squad** | 5 秒设置，最佳稳定性 |
| Docker 隔离 + 代理竞争 | **Parallel Code** | AI Arena，项目特定 Dockerfile |
| 规格驱动跨服务重构 | **Intent** | 活规格传播，Coordinator/Verifier |
| 免费，最简单的 Mac 入门 | **Conductor** | 免费 + 自带登录，最佳打磨 |

---

## 📈 功能对比矩阵

| 工具 | Worktree | Diff 审查 | Remote/SSH | 移动端 | 浏览器 | CLI/SDK/MCP | 自动化 | 工单集成 |
|------|:--------:|:-----------:|:----------:|:------:|:-------:|:-----------:|:-----------:|:-----------------:|
| **Orca** | ✅ | ✅ | ✅ | ✅ iOS+Android | ✅ Design Mode | ✅ CLI | ❌ | GitHub·Linear |
| **Emdash** | ✅ | ✅ | ✅ SSH/SFTP | ❌ | ❌ | ❌ | ❌ | 12 个平台 |
| **Superset** | ✅ | ✅ | ✅ | 🔄 iOS 即将 | ✅ | ✅ CLI+SDK+MCP | ✅ | Slack·Linear |
| **cmux** | ❌ | ❌ | ✅ | ❌ | ✅ | ✅ CLI+Socket | ❌ | ❌ |
| **Parallel Code** | ✅ | ✅ | ❌ | ✅ QR | ❌ | ❌ | ❌ | ❌ |
| **Claude Squad** | ✅ | ⚠️ 弱 | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ |
| **Vibe Kanban** | ✅ | ✅ | ❌ | ❌ | ✅ | ✅ MCP | ❌ | ❌ |
| **Nimbalyst** | ✅ | ✅ | ❌ | ✅ iOS | ❌ | ❌ | ❌ | ❌ |
| **Intent** | ✅ | ✅ | ❌ | ❌ | ✅ | ✅ MCP | ❌ | ❌ |
| **Conductor** | ✅ | ✅ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ |

---

## 🌐 更广泛的生态系统

这些**不是** agent-native IDE，但已吸收 worktree/并行代理功能，值得了解：

| 工具 | 类别 | Agent-Native 功能 |
|------|----------|---------------------|
| [Cursor 3](https://cursor.com/) | 专用 IDE | Agents Window，含 `/worktree` 和 `/best-of-n` 命令（2026.04） |
| [Windsurf Wave 13](https://windsurf.com/) | 专用 IDE | 基于 worktree 的并行 Cascade 会话，专用代理终端 |
| [Google Antigravity](https://antigravity.google/) | 专用 IDE | 多代理并行工作区，免费，动态子代理 |
| [Cline](https://cline.bot/) | VS Code 扩展 | 模型无关，开源代理 |
| [Roo Code](https://roocode.com/) | VS Code 扩展 | 多角色代理系统（Coder、Architect、Debugger） |
| [Claude Code](https://claude.com/product/claude-code) | 终端代理 | 子代理 frontmatter 内置 `isolation: worktree` |
| [Aider](https://aider.chat/) | 终端代理 | 编辑器无关，Git 原生 CLI 结对编程 |

---

## 📅 市场观察（2026 年 7 月）

1. **Orca 和 Emdash 构成第一梯队** — 跨平台、开源、功能丰富、稳定性好。
2. **cmux 在社区规模和性能上独占鳌头** — 但仅 macOS 且仅终端。
3. **Superset 功能深度最强** — 但仅 macOS 是致命限制。
4. **闭源工具（Conductor、Intent）排名最低** — 在开源自由度上结构性不利。
5. **Git worktree 是共识的隔离原语** — 所有严肃工具都已采用。
6. **端口冲突是下一个前沿** — 仅 Emdash（`$EMDASH_PORT`）在配置层面解决。
7. **移动监控正在兴起** — Orca（iOS+Android）、Parallel Code（QR）、Nimbalyst（iOS）领先。
8. **类别正在整合** — Crystal → Nimbalyst，Bloop → 社区 Vibe Kanban。预计 2026 下半年有更多并购和关闭。

---

## 🤝 贡献

欢迎贡献！如需添加工具、更新分数或修正不准确之处：

1. 开一个 [issue](https://github.com/pinion05/awesome-agent-ide/issues) 留下你的建议
2. 或提交包含更新数据和来源的 PR

更改分数时请附上**可验证的来源**（GitHub 仓库、文档、评测文章）。

---

## 📄 许可证

[CC0-1.0](LICENSE) — 公共领域。自由使用。

---

<div align="center">

**[🌐 查看网站](https://pinion05.github.io/awesome-agent-ide/)** · **[⭐ 在 GitHub 上 Star](https://github.com/pinion05/awesome-agent-ide)**

*最后更新：2026 年 7 月 · 维护：[pinion05](https://github.com/pinion05)*

</div>
