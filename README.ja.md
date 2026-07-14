<div align="center">

# 🚀 Awesome Agent-Native IDE

### AIコーディングエージェント時代のために生まれたIDE＆オーケストレーターの総合比較

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

## 📖 Agent-Native IDEとは？

従来のIDE（Cursor、Windsurf、VS Code）はAI機能を既存のエディタに「後付け」するアプローチです。一方、**Agent-Native IDE**は、複数のCLIコーディングエージェント（Claude Code、Codex、Gemini CLIなど）を**並列で実行・管理・レビューするためにゼロから設計された**環境です。

主な特徴：

| 機能 | 説明 |
|---------|-------------|
| **Git Worktree分離** | 各エージェントが独自のブランチと作業ディレクトリを持ち、1つの`.git`データベースを共有 |
| **マルチエージェント並列実行** | 5〜20以上のエージェントを1画面で同時監視 |
| **Diffレビュー＋マージワークフロー** | エージェントが生成した変更を1箇所で確認後にマージ |
| **BYOA（Bring Your Own Agent）** | 自分のサブスクリプションで任意のCLIエージェントを実行 — ベンダーロックインなし |

> **対象外:** AI機能を後付けした従来IDE（Cursor、Windsurf、Copilot）。優れたツールですが、このリストは*エージェントオーケストレーションが主目的*のツールに焦点を当てています。

---

## 🏆 総合ランキング

| 順位 | ツール | スコア | プラットフォーム | ライセンス | Stars | 一言 |
|:----:|------|:-----:|----------|---------|:-----:|-----------|
| 🥇 | [**Orca**](https://github.com/stablyai/orca) | **8.6** | macOS·Win·Linux·📱 | MIT | 18.3K | フルクロスプラットフォーム＋モバイル、Design Mode、毎日リリース |
| 🥈 | [**Emdash**](https://github.com/generalaction/emdash) | **8.3** | macOS·Win·Linux | Apache-2.0 | 5.1K | ポートインジェクション、12チケット統合、34エージェント |
| 🥉 | [**Superset**](https://github.com/superset-sh/superset) | **7.5** | macOS | Other | 12.4K | CLI + SDK + MCP、自動化、最も広いエージェントサポート |
| 4 | [**cmux**](https://github.com/manaflow-ai/cmux) | **7.0** | macOS | Other | 24.4K | ネイティブSwift性能、最大コミュニティ、ターミナルファースト |
| 5 | [**Parallel Code**](https://github.com/johannesjo/parallel-code) | **6.7** | macOS·Linux | MIT | 0.8K | Dockerサンドボックス、AI Arena、カバレッジレーダー |
| 6 | [**Claude Squad**](https://github.com/smtg-ai/claude-squad) | **6.5** | macOS·Linux | AGPL-3.0 | 8.1K | 最高の安定性（0.6%）、最速セットアップ |
| 7 | [**Vibe Kanban**](https://github.com/BloopAI/vibe-kanban) | **6.3** | Web | Apache-2.0 | — | カンバン＋MCP自動分解（コミュニティ保守） |
| 8 | [**Nimbalyst**](https://nimbalyst.com/) | **6.2** | クロスプラットフォーム·📱 | MIT | — | Worktreeファーストクラス、ビジュアル編集、iOSコンパニオン |
| 9 | [**Intent**](https://www.intentapp.dev/) | **6.1** | macOS | クローズド | — | スペック駆動調整、Coordinator/Verifierエージェント |
| 10 | [**Conductor**](https://www.conductor.build/) | **5.7** | macOS | クローズド | — | Mac最高の洗練度、無料、BYOログイン |

---

## 📊 評価方法論

各ツールを**7つの指標**で評価（1〜10点）、重み付けして総合スコアを算出します。

| 指標 | 重み | 評価内容 |
|-----------|:------:|------------------|
| **技術力** | 20% | 分離モデル（worktree/container）、調整の深さ、アーキテクチャ品質、独自技術（Design Mode、Computer Use、ポートインジェクション） |
| **安定性** | 15% | イシュー/スター比、リリース頻度、コードベース成熟度、ランタイム安定性（ネイティブ vs Electron） |
| **UX / 利便性** | 15% | セットアップの容易さ、ビジュアルdiffレビュー、キーボードショートカット、通知システム、ワークフロー洗練度 |
| **エコシステム** | 15% | 対応エージェント、チケット統合（Linear/GitHub/Jira）、CLI/SDK/MCP提供、コミュニティ規模 |
| **スケーラビリティ** | 15% | リモート実行（SSH）、モバイルコンパニオン、並列容量、プログラマビリティ |
| **プラットフォーム対応** | 10% | OSカバレッジ（macOS / Windows / Linux / モバイル） |
| **オープンソース健全性** | 10% | ライセンスの自由度、ベンダー独立性、コミュニティ主導度 |

### 詳細スコア

| ツール | 技術力 (20%) | 安定性 (15%) | UX (15%) | エコシステム (15%) | スケーラビリティ (15%) | プラットフォーム (10%) | OSS (10%) | **総合** |
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

## 🔍 ツール別詳細分析

### 🥇 1. Orca — stablyai/orca

| | |
|---|---|
| **GitHub** | [stablyai/orca](https://github.com/stablyai/orca) |
| **Stars / Forks / Issues** | 18,327 / 1,448 / 1,361 (7.4%) |
| **言語** | TypeScript (Electron) |
| **ライセンス** | MIT |
| **プラットフォーム** | macOS · Windows · Linux · iOS · Android |
| **ウェブサイト** | [onorca.dev](https://www.onorca.dev/) |

**✅ 長所**
- **唯一のフルクロスプラットフォーム＋モバイル** — iOS/Androidコンパニオンアプリでどこからでもエージェント監視・フォローアップ
- **Design Mode** — 実際のChromiumウィンドウでUI要素をクリック、HTML/CSS/スクリーンショットをエージェントのプロンプトに直接送信。Orca独自の機能
- **SSH Worktrees** — リモートマシンでエージェント実行、自動再接続＋ポートフォワーディング
- **Computer Use** — エージェントがデスクトップアプリと実際のUIを操作可能
- **GitHub & Linearネイティブ** — PR/issue/ボードをアプリ内でブラウジング、タスクからworktreeを開く
- **Annotate AI Diffs** — diff行にコメントを追加しエージェントにフィードバック送信
- **毎日リリース** — 毎日機能を出荷、changelogが実質的な機能リスト
- Ghostty-classターミナル（WebGL）、無限分割、再起動後もスクロールバック保持

**❌ 短所**
- Electronベース — ネイティブ代替（cmux）よりメモリ/起動速度で劣る
- 1,361件の未解決イシュー — 活発だが管理負担が現実的
- MITだがstablyai主導 — 単一ベンダー依存

> **おすすめ:** モバイル監視、クロスプラットフォームサポート、最も豊富なagent-native機能セットが必要な分散チーム。

---

### 🥈 2. Emdash — generalaction/emdash

| | |
|---|---|
| **GitHub** | [generalaction/emdash](https://github.com/generalaction/emdash) |
| **Stars / Forks / Issues** | 5,149 / 534 / 132 (2.6%) |
| **言語** | TypeScript (Electron) |
| **ライセンス** | Apache-2.0 |
| **プラットフォーム** | macOS · Windows · Linux |
| **ウェブサイト** | [emdash.ai](https://emdash.ai/) |
| **バッキング** | YC W26 |

**✅ 長所**
- **最も広いチケット統合** — Linear、GitHub、Jira、GitLab、Asana、Monday.com、Trello、Plane、Forgejo、Featurebase、Plain、Notion（12プラットフォーム）
- **`$EMDASH_PORT`インジェクション** — ポート衝突問題を設定レベルで解決。他のツールが見落とす部分
- **最も広いエージェントサポート** — 34 CLIプロバイダーを自動検出（Claude Code、Codex、Cursor、OpenCode、Amp、Devin、Qwen Code、Droid、Copilot等）
- **SSH/SFTPリモートプロジェクト** — リモートコードベースで同じ並列ワークフロー、OSキーチェーン認証
- **Local-first + プライバシー** — SQLiteローカル保存、コード/チャットをEmdashサーバーに送信しない
- クロスプラットフォーム＋Apache-2.0 — 最も寛容なライセンス組み合わせ
- イシュー/スター比2.6% — 安定性指標優秀

**❌ 短所**
- モバイルコンパニオンアプリなし
- エージェント間調整（協調）不可 — 各エージェントが独立実行
- 2026年初頭ローンチ — コミュニティ成長段階

> **おすすめ:** チケット統合、ポート分離、クロスプラットフォームサポート、強力なプライバシー保証が必要なエンタープライズチーム。

---

### 🥉 3. Superset — superset-sh/superset

| | |
|---|---|
| **GitHub** | [superset-sh/superset](https://github.com/superset-sh/superset) |
| **Stars / Forks / Issues** | 12,399 / 1,076 / 323 (2.6%) |
| **言語** | TypeScript (Electron) |
| **ライセンス** | Other |
| **プラットフォーム** | macOS |
| **ウェブサイト** | [superset.sh](https://superset.sh/) |
| **バッキング** | YC |

**✅ 長所**
- **最も多様なアクセス面** — デスクトップアプリ＋CLI＋TypeScript SDK＋MCPサーバー。どこからでもワークスペース制御
- **最も広いエージェントサポート** — Amp、Claude Code、Codex、Cursor、Droid、Gemini、Copilot、Mastra、Mistral Vibe、OpenCode、Pi、Polygraph＋カスタムエージェント
- **自動化（Automations）** — スケジュールベースのエージェントセッション実行
- **Slack & Linear統合** — Slackメッセージ/Linear issueからワークスペース作成
- **アプリ内ブラウザ＋ポート検出** — ワークスペースごとのdevサーバープレビュー
- カスタムエージェントサポート（アイコン付き）、ワークスペースプリセット
- イシュー/スター比2.6% — 安定性良好

**❌ 短所**
- **macOS専用** — Windows/Linuxビルドなし。最も致命的な弱点
- Bunランタイム、Caddy等の外部依存関係が必要
- "Other"ライセンス — オープンソースの自由度が不明確
- iOSアプリはまだ「近日対応」

> **おすすめ:** 最大のプログラマビリティ（CLI + SDK + MCP）と最も広いエージェントエコシステムを求めるmacOS開発者。

---

### 4. cmux — manaflow-ai/cmux

| | |
|---|---|
| **GitHub** | [manaflow-ai/cmux](https://github.com/manaflow-ai/cmux) |
| **Stars / Forks / Issues** | 24,412 / 1,970 / 3,446 (14.1%) |
| **言語** | Swift (ネイティブmacOS) |
| **ライセンス** | Other (GPL-3.0 + 商用デュアル) |
| **プラットフォーム** | macOS |
| **ウェブサイト** | [cmux.com](https://cmux.com/) |

**✅ 長所**
- **GitHub Stars最多（24.4K）** — 最大コミュニティ
- **ネイティブ性能** — Swift/AppKit＋libghostty GPUレンダリング。Electronを起動速度・メモリで圧倒
- **明確な哲学** — 「プリミティブであってソリューションではない」。ワークフローを強制しない
- **通知システム** — OSC 9/99/777シーケンス検出、青いリング＋タブハイライト、`cmux notify` CLI
- **アプリ内ブラウザ** — agent-browser APIポーティング、アクセシビリティツリースナップショット・クリック・フォーム入力・JS実行
- **SSH** — `cmux ssh user@remote`でリモートワークスペース作成、ブラウザがリモートネットワーク経由
- **Claude Code Teams** — `cmux claude-teams`コマンド一つでteammateモード、tmux不要
- Ghostty config互換 — 既存のテーマ/フォント/カラーがそのまま使用可能
- CLI＋socket APIでフル自動化

**❌ 短所**
- **macOS専用** — プラットフォームスコア最低
- **ターミナルであってIDEではない** — worktree管理、diffビューアー、PR作成機能なし
- **イシュー3,446件（14.1%）** — 比率最高。複雑なネイティブアプリの管理負担
- モバイルなし

> **おすすめ:** ネイティブ性能とターミナルファースト、非強制的アプローチを求めるmacOSパワーユーザー。diffレビューはOrca/Emdash/Supersetと組み合わせ。

---

### 5. Parallel Code — johannesjo/parallel-code

| | |
|---|---|
| **GitHub** | [johannesjo/parallel-code](https://github.com/johannesjo/parallel-code) |
| **Stars / Forks / Issues** | 838 / 111 / 39 (4.7%) |
| **言語** | TypeScript (Electron + SolidJS) |
| **ライセンス** | MIT |
| **プラットフォーム** | macOS · Linux |
| **ウェブサイト** | [parallelcode.app](https://parallelcode.app/) |

**✅ 長所**
- **Dockerサンドボックス** — プロジェクト別`.parallel-code/Dockerfile`で完全分離。他のOSSツールにない機能
- **AI Arena** — エージェント間ヘッドツーヘッド競争、勝者をマージ
- **カバレッジレーダー** — 変更ファイルごとのテストカバレッジバッジ
- **Steps追跡パネル** — エージェント進行タイムライン
- モバイル監視（QRコード→Wi-Fi/Tailscale）
- 10テーマ、キーボードファースト、フォーカスモード
- MITライセンス、完全無料

**❌ 短所**
- コミュニティ最小（838★）— 長期保守が不確実
- Windows非対応
- SSH/リモートworktreeなし
- 単一開発者プロジェクト（johannesjo）

> **おすすめ:** Docker隔離エージェントとヘッドツーヘッドエージェント競争を実験する開発者。

---

### 6. Claude Squad — smtg-ai/claude-squad

| | |
|---|---|
| **GitHub** | [smtg-ai/claude-squad](https://github.com/smtg-ai/claude-squad) |
| **Stars / Forks / Issues** | 8,108 / 585 / 52 (0.6%) |
| **言語** | Go (TUI) |
| **ライセンス** | AGPL-3.0 |
| **プラットフォーム** | macOS · Linux (tmux必須) |
| **ウェブサイト** | [smtg-ai.github.io/claude-squad](https://smtg-ai.github.io/claude-squad/) |

**✅ 長所**
- **最高の安定性** — 0.6%イシュー/スター比、Goバイナリ、シンプルアーキテクチャ（tmux + worktree）
- **最速セットアップ** — `brew install claude-squad`→5秒で6セッション起動
- キーボードファーストTUI — vimスタイルナビゲーション
- Claude Code、Codex、Aider、Gemini、OpenCode、Amp対応
- `--autoyes`フラグで無人自動承認（実験的）

**❌ 短所**
- **ビジュアルdiffレビューが弱い** — 別ツールが必要
- **リモート/SSH/モバイルなし** — ローカル単一マシンのみ
- AGPL-3.0 — 商用組み込み時に法務レビュー必要
- Windows非対応（tmux依存）

> **おすすめ:** 並列エージェントへの最速かつ最も安定したパスを求めるターミナルパワーユーザー。macOS/Linuxソロ開発者。

---

### 7. Vibe Kanban — BloopAI/vibe-kanban

| | |
|---|---|
| **GitHub** | [BloopAI/vibe-kanban](https://github.com/BloopAI/vibe-kanban) |
| **言語** | Rust (ウェブアプリ) |
| **ライセンス** | Apache-2.0 |
| **プラットフォーム** | Web (クロスプラットフォーム) |
| **状態** | コミュニティ保守（Bloopは2026年4月にサービス終了） |

**✅ 長所**
- カンバンカード＝worktree＝エージェント — 直感的なメタファー
- MCPサーバーによるカード自動分解（自律的タスク分解に最も近い）
- 10+エージェント対応、アプリ内ブラウザ（デバイスエミュレーション付き）
- セルフホスト可能、チームフレンドリー

**❌ 短所**
- **Bloopサービス終了** — 有料サブスクリプション返金、クラウド機能縮小
- ハードタスク依存性（タスクBがタスクAを待つ）非対応
- worktree 20個でディスク負荷
- 今後の保守速度がコミュニティ貢献に完全依存

> **おすすめ:** 共有ビジュアルボードとMCP駆動タスク分解が必要で、コミュニティ保守ソフトウェアに寛容なチーム。

---

### 8. Nimbalyst — nimbalyst.com

| | |
|---|---|
| **ウェブサイト** | [nimbalyst.com](https://nimbalyst.com/) |
| **プラットフォーム** | クロスプラットフォームデスクトップ＋iOS＋Android |
| **前身** | Crystal（2026年2月非推奨） |

**✅ 長所**
- worktreeがセッションオブジェクトのファーストクラスプリミティブ — セッション開始時ワンクリックオプション
- インラインdiff、ビジュアルファイルサイドバー、GUIレビュー＆マージ
- クロスプラットフォーム＋iOSコンパニオン
- Markdown/Excalidraw/モックアップビジュアル編集内蔵

**❌ 短所**
- 最も若いプロジェクト（2026年2月Crystalからリブランディング）
- コミュニティ・ドキュメント・評価データ不足
- ベンダー主導、MITライセンス
- エージェントサポートが狭い（Claude Code、Codex）

> **おすすめ:** ビジュアル編集付きworktreeファーストセッション管理を求める開発者。プロジェクトが成熟する6ヶ月後に再評価推奨。

---

### 9. Intent — Augment Code

| | |
|---|---|
| **ウェブサイト** | [intentapp.dev](https://www.intentapp.dev/) |
| **プラットフォーム** | macOS（Windowsウェイティングリスト、Linux未発表） |
| **状態** | パブリックベータ |
| **価格** | Augmentクレジット（$0トライアル / $20〜$200/月; BYOA無料） |

**✅ 長所**
- **スペック駆動調整** — Living specが全エージェントの唯一の真実の情報源。スペックを一度編集すると全アクティブエージェントに伝播
- **Coordinator → Implementor → Verifier**の3エージェント分業
- クロスサービスリファクタリングで真価 — フィールド名変更等がスペック経由で伝播
- BYOA（Claude Code、Codex、OpenCode＋Auggie）
- Context EngineをMCPサーバーとして公開

**❌ 短所**
- **クローズドソース** — コード監査不可、ベンダーロックイン
- **macOS専用** — Windowsウェイティングリスト、Linux未発表
- Augmentクレジット使用 — 既存Claude/Cursorサブスクリプションとコスト重複
- パブリックベータ — 本番安定性未検証

> **おすすめ:** スペック駆動調整が価値のある複雑なクロスサービスリファクタリングを行うmacOSチーム。

---

### 10. Conductor — Melty Labs

| | |
|---|---|
| **ウェブサイト** | [conductor.build](https://www.conductor.build/) |
| **プラットフォーム** | macOS |
| **ライセンス** | クローズドソース |
| **価格** | 無料（BYOログイン） |

**✅ 長所**
- macOSで最も洗練されたダッシュボード — diff-firstレビュー、クリーンなUX
- 無料＋BYO Claude/Codex/Cursor/OpenCodeログイン
- 既存VS Code/JetBrainsの隣に置く最適なオーケストレーター

**❌ 短所**
- **クローズドソース** — コード監査不可、ベンダーロックイン
- **macOS専用** — クロスプラットフォーム「徐々に追加中」
- CLI/SDK/MCPなし — プログラマブルではない
- リモート/SSH/モバイルなし
- エージェントサポートが狭い（4種）

> **おすすめ:** 既存エディタの隣で並列エージェントオーケストレーションの最も簡単で洗練されたエントリポイントを求めるmacOS開発者。

---

## 🎯 ユースケース別推奨

| 状況 | 推奨ツール | 理由 |
|----------------|-------------------|-----|
| クロスプラットフォームチーム、モバイル監視必要 | **Orca** | 3 OS＋iOS/Android対応の唯一のツール |
| エンタープライズ、複数チケットシステム | **Emdash** | 12チケットプラットフォーム＋ポートインジェクション＋プライバシー |
| macOS＋プログラマブル自動化 | **Superset** | CLI + SDK + MCP、Automations |
| macOS＋ネイティブ性能＋ターミナルファースト | **cmux** | Swift/AppKit、GPUレンダリング、通知システム |
| ターミナルのみ、最速スタート | **Claude Squad** | 5秒セットアップ、最高安定性 |
| Docker隔離＋エージェント競争 | **Parallel Code** | AI Arena、プロジェクト別Dockerfile |
| スペック駆動クロスサービスリファクタリング | **Intent** | Living spec伝播、Coordinator/Verifier |
| 無料、最も簡単なMac導入 | **Conductor** | 無料＋BYOログイン、最高洗練度 |

---

## 📈 機能比較マトリクス

| ツール | Worktree | Diffレビュー | Remote/SSH | モバイル | ブラウザ | CLI/SDK/MCP | 自動化 | チケット統合 |
|------|:--------:|:-----------:|:----------:|:------:|:-------:|:-----------:|:-----------:|:-----------------:|
| **Orca** | ✅ | ✅ | ✅ | ✅ iOS+Android | ✅ Design Mode | ✅ CLI | ❌ | GitHub·Linear |
| **Emdash** | ✅ | ✅ | ✅ SSH/SFTP | ❌ | ❌ | ❌ | ❌ | 12プラットフォーム |
| **Superset** | ✅ | ✅ | ✅ | 🔄 iOS近日 | ✅ | ✅ CLI+SDK+MCP | ✅ | Slack·Linear |
| **cmux** | ❌ | ❌ | ✅ | ❌ | ✅ | ✅ CLI+Socket | ❌ | ❌ |
| **Parallel Code** | ✅ | ✅ | ❌ | ✅ QR | ❌ | ❌ | ❌ | ❌ |
| **Claude Squad** | ✅ | ⚠️ 弱い | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ |
| **Vibe Kanban** | ✅ | ✅ | ❌ | ❌ | ✅ | ✅ MCP | ❌ | ❌ |
| **Nimbalyst** | ✅ | ✅ | ❌ | ✅ iOS | ❌ | ❌ | ❌ | ❌ |
| **Intent** | ✅ | ✅ | ❌ | ❌ | ✅ | ✅ MCP | ❌ | ❌ |
| **Conductor** | ✅ | ✅ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ |

---

## 🌐 より広いエコシステム

これらはagent-native IDEではありませんが、worktree/並列エージェント機能を吸収しており、知っておく価値があります：

| ツール | カテゴリー | Agent-Native機能 |
|------|----------|---------------------|
| [Cursor 3](https://cursor.com/) | 専用IDE | `/worktree`および`/best-of-n`コマンド付きAgents Window（2026.04） |
| [Windsurf Wave 13](https://windsurf.com/) | 専用IDE | worktreeベース並列Cascadeセッション、専用エージェントターミナル |
| [Google Antigravity](https://antigravity.google/) | 専用IDE | マルチエージェント並列ワークスペース、無料、動的サブエージェント |
| [Cline](https://cline.bot/) | VS Code拡張 | モデル非依存、オープンソースエージェント |
| [Roo Code](https://roocode.com/) | VS Code拡張 | マルチペルソナエージェントシステム（Coder、Architect、Debugger） |
| [Claude Code](https://claude.com/product/claude-code) | ターミナルエージェント | サブエージェントfrontmatterの`isolation: worktree`組み込み |
| [Aider](https://aider.chat/) | ターミナルエージェント | エディタ非依存、GitネイティブCLIペアプログラミング |

---

## 📅 市場観察（2026年7月）

1. **OrcaとEmdashがトップティアを形成** — クロスプラットフォーム、オープンソース、豊富な機能、良好な安定性。
2. **cmuxはコミュニティ規模と性能で圧倒的** — ただしmacOS専用＋ターミナルのみ。
3. **Supersetは機能の深さが最高クラス** — ただしmacOS専用が致命的。
4. **クローズドソースツール（Conductor、Intent）が最低位** — オープンソースの自由度で構造的不利。
5. **Git worktreeがコンセンサスの分離プリミティブ** — すべてのserious toolが採用。
6. **ポート衝突が次のフロンティア** — Emdash（`$EMDASH_PORT`）のみが設定レベルで解決。
7. **モバイル監視が台頭** — Orca（iOS+Android）、Parallel Code（QR）、Nimbalyst（iOS）がリード。
8. **カテゴリー統合が進行中** — Crystal→Nimbalyst、Bloop→コミュニティVibe Kanban。2026年下半期に追加のM&Aと終了が予想。

---

## 🤝 コントリビュート

コントリビューションを歓迎します！ツールの追加、スコアの更新、不正確さの修正が必要な場合：

1. [イシュー](https://github.com/pinion05/awesome-agent-ide/issues)を開いて提案を残してください
2. または更新されたデータとソースを含むPRを提出してください

スコア変更時は**検証可能なソース**（GitHubリポジトリ、ドキュメント、レビュー記事）を含めてください。

---

## 📄 ライセンス

[CC0-1.0](LICENSE) — パブリックドメイン。ご自由にどうぞ。

---

<div align="center">

**[🌐 ウェブサイトを見る](https://pinion05.github.io/awesome-agent-ide/)** · **[⭐ GitHubでStar](https://github.com/pinion05/awesome-agent-ide)**

*最終更新：2026年7月 · 管理：[pinion05](https://github.com/pinion05)*

</div>
