<div align="center">

# 🚀 Awesome Agent-Native IDE

### AI 코딩 에이전트 시대를 위해 태어난 IDE & 오케스트레이터 종합 비교

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

## 📖 Agent-Native IDE란?

전통적 IDE(Cursor, Windsurf, VS Code)가 AI 기능을 기존 에디터에 "붙이는" 접근이라면, **Agent-Native IDE**는 여러 CLI 코딩 에이전트(Claude Code, Codex, Gemini CLI 등)를 **병렬로 실행·관리·리뷰하기 위해 처음부터 설계된** 환경입니다.

핵심 특징:

| 기능 | 설명 |
|---------|-------------|
| **Git Worktree 격리** | 각 에이전트마다 독립된 브랜치와 작업 디렉토리. 하나의 `.git` 데이터베이스를 공유 |
| **멀티 에이전트 동시 실행** | 5~20개 이상의 에이전트를 한 화면에서 동시 모니터링 |
| **Diff 리뷰 + 머지 워크플로우** | 에이전트가 만든 변경사항을 한 곳에서 검토 후 머지 |
| **BYOA (Bring Your Own Agent)** | 자기 구독으로 어떤 CLI 에이전트든 실행 — 벤더 종속 없음 |

> **다루지 않는 범위:** AI 기능을 붙인 전통 IDE(Cursor, Windsurf, Copilot). 훌륭한 도구들이지만, 이 리스트는 *에이전트 오케스트레이션이 주 목적인* 도구에 집중합니다.

---

## 🏆 종합 순위

| 순위 | 도구 | 점수 | 플랫폼 | 라이선스 | Stars | 한줄평 |
|:----:|------|:-----:|----------|---------|:-----:|-----------|
| 🥇 | [**Orca**](https://github.com/stablyai/orca) | **8.6** | macOS·Win·Linux·📱 | MIT | 18.3K | 풀 크로스플랫폼 + 모바일, Design Mode, 일일 릴리스 |
| 🥈 | [**Emdash**](https://github.com/generalaction/emdash) | **8.3** | macOS·Win·Linux | Apache-2.0 | 5.1K | 포트 주입, 12개 티켓 통합, 34 에이전트 |
| 🥉 | [**Superset**](https://github.com/superset-sh/superset) | **7.5** | macOS | Other | 12.4K | CLI + SDK + MCP, 자동화, 최다 에이전트 지원 |
| 4 | [**cmux**](https://github.com/manaflow-ai/cmux) | **7.0** | macOS | Other | 24.4K | 네이티브 Swift 성능, 최대 커뮤니티, 터미널 퍼스트 |
| 5 | [**Parallel Code**](https://github.com/johannesjo/parallel-code) | **6.7** | macOS·Linux | MIT | 0.8K | Docker 샌드박싱, AI Arena, 커버리지 레이더 |
| 6 | [**Claude Squad**](https://github.com/smtg-ai/claude-squad) | **6.5** | macOS·Linux | AGPL-3.0 | 8.1K | 최고 안정성 (0.6% 이슈율), 최단 설정 |
| 7 | [**Vibe Kanban**](https://github.com/BloopAI/vibe-kanban) | **6.3** | Web | Apache-2.0 | — | 칸반 + MCP 자동 분해 (커뮤니티 유지보수) |
| 8 | [**Nimbalyst**](https://nimbalyst.com/) | **6.2** | 크로스플랫폼·📱 | MIT | — | Worktree 일급 시민, 시각 편집, iOS 동반 앱 |
| 9 | [**Intent**](https://www.intentapp.dev/) | **6.1** | macOS | 폐쇄 | — | 스펙 기반 조정, Coordinator/Verifier 에이전트 |
| 10 | [**Conductor**](https://www.conductor.build/) | **5.7** | macOS | 폐쇄 | — | Mac 최고 폴리싱, 무료, BYO 로그인 |

---

## 📊 평가 방법론

각 도구를 **7개 지표**로 평가 (1–10점), 가중치를 적용해 종합 점수를 산출합니다.

| 지표 | 가중치 | 평가 요소 |
|-----------|:------:|------------------|
| **기술력** | 20% | 격리 모델(worktree/container), 조정 깊이, 아키텍처 품질, 고유 기술(Design Mode, Computer Use, 포트 주입 등) |
| **안정성** | 15% | 이슈/스타 비율, 릴리스 주기, 코드베이스 성숙도, 런타임 안정성(native vs Electron) |
| **편의성** | 15% | 설치 용이성, 시각적 diff 리뷰, 키보드 단축키, 알림 시스템, 워크플로우 폴리싱 |
| **생태계** | 15% | 지원 에이전트, 티켓 통합(Linear/GitHub/Jira), CLI/SDK/MCP 제공, 커뮤니티 규모 |
| **확장성** | 15% | 원격 실행(SSH), 모바일 동반 앱, 병렬 용량, 프로그래밍 가능성 |
| **플랫폼 지원** | 10% | OS 지원 범위 (macOS / Windows / Linux / 모바일) |
| **오픈소스 건전성** | 10% | 라이선스 자유도, 벤더 독립성, 커뮤니티 주도도 |

### 상세 점수

| 도구 | 기술력 (20%) | 안정성 (15%) | 편의성 (15%) | 생태계 (15%) | 확장성 (15%) | 플랫폼 (10%) | 오픈소스 (10%) | **종합** |
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

## 🔍 도구별 상세 분석

### 🥇 1. Orca — stablyai/orca

| | |
|---|---|
| **GitHub** | [stablyai/orca](https://github.com/stablyai/orca) |
| **Stars / Forks / Issues** | 18,327 / 1,448 / 1,361 (7.4%) |
| **언어** | TypeScript (Electron) |
| **라이선스** | MIT |
| **플랫폼** | macOS · Windows · Linux · iOS · Android |
| **웹사이트** | [onorca.dev](https://www.onorca.dev/) |

**✅ 장점**
- **유일한 풀 크로스플랫폼 + 모바일** — iOS/Android 동반 앱으로 어디서나 에이전트 모니터링 및 후속 지시
- **Design Mode** — 실제 Chromium 창에서 UI 요소 클릭 시 HTML/CSS/스크린샷을 에이전트 프롬프트로 직송. Orca만의 고유 기능
- **SSH Worktrees** — 원격 머신에서 에이전트 실행, 자동 재연결 + 포트 포워딩
- **Computer Use** — 에이전트가 데스크톱 앱과 실제 UI 조작 가능
- **GitHub & Linear 네이티브** — PR/이슈/보드를 앱 내에서 브라우징, 태스크에서 워크트리 열기
- **Annotate AI Diffs** — diff 라인에 코멘트를 달아 에이전트에게 피드백 전송
- **일일 릴리스** — 매일 기능 출시, changelog가 사실상 기능 목록
- Ghostty-class 터미널 (WebGL 렌더링), 무한 분할, 재시작 후에도 스크롤백 보존

**❌ 단점**
- Electron 기반 — 네이티브 대안(cmux) 대비 메모리/시작 속도 열세
- 1,361개 미해결 이슈 — 활발하지만 관리 부담 존재
- MIT이지만 stablyai 단일 주도 — 벤더 의존도

> **추천:** 모바일 모니터링, 크로스플랫폼 지원, 최강의 agent-native 기능 세트가 필요한 분산 팀.

---

### 🥈 2. Emdash — generalaction/emdash

| | |
|---|---|
| **GitHub** | [generalaction/emdash](https://github.com/generalaction/emdash) |
| **Stars / Forks / Issues** | 5,149 / 534 / 132 (2.6%) |
| **언어** | TypeScript (Electron) |
| **라이선스** | Apache-2.0 |
| **플랫폼** | macOS · Windows · Linux |
| **웹사이트** | [emdash.ai](https://emdash.ai/) |
| **백킹** | YC W26 |

**✅ 장점**
- **가장 넓은 티켓 통합** — Linear, GitHub, Jira, GitLab, Asana, Monday.com, Trello, Plane, Forgejo, Featurebase, Plain, Notion (12개 플랫폼)
- **`$EMDASH_PORT` 주입** — 포트 충돌 문제를 설정 레벨에서 해결. 다른 도구가 놓치는 부분
- **가장 넓은 에이전트 지원** — 34 CLI 제공자 자동 감지 (Claude Code, Codex, Cursor, OpenCode, Amp, Devin, Qwen Code, Droid, Copilot 등)
- **SSH/SFTP 원격 프로젝트** — 원격 코드베이스에서 동일한 병렬 워크플로우, OS 키체인 인증
- **Local-first + 프라이버시** — SQLite 로컬 저장, 코드/채팅을 Emdash 서버로 전송하지 않음
- 크로스플랫폼 + Apache-2.0 — 가장 관대한 라이선스 조합
- 이슈/스타 비율 2.6% — 안정성 지표 우수

**❌ 단점**
- 모바일 동반 앱 없음
- 에이전트 간 조정(협업) 불가 — 각자 독립 실행
- 2026년 초 출시 — 커뮤니티 성장 단계

> **추천:** 티켓 통합, 포트 격리, 크로스플랫폼 지원, 강력한 프라이버시 보장이 필요한 엔터프라이즈 팀.

---

### 🥉 3. Superset — superset-sh/superset

| | |
|---|---|
| **GitHub** | [superset-sh/superset](https://github.com/superset-sh/superset) |
| **Stars / Forks / Issues** | 12,399 / 1,076 / 323 (2.6%) |
| **언어** | TypeScript (Electron) |
| **라이선스** | Other |
| **플랫폼** | macOS |
| **웹사이트** | [superset.sh](https://superset.sh/) |
| **백킹** | YC |

**✅ 장점**
- **가장 다양한 접근면** — 데스크톱 앱 + CLI + TypeScript SDK + MCP 서버. 어디서든 워크스페이스 제어
- **가장 넓은 에이전트 지원** — Amp, Claude Code, Codex, Cursor, Droid, Gemini, Copilot, Mastra, Mistral Vibe, OpenCode, Pi, Polygraph + 커스텀 에이전트
- **자동화(Automations)** — 스케줄 기반 에이전트 세션 실행
- **Slack & Linear 통합** — Slack 메시지/Linear 이슈에서 워크스페이스 생성
- **인앱 브라우저 + 포트 감지** — 워크스페이스별 dev 서버 미리보기
- 커스텀 에이전트 지원(아이콘 포함), 워크스페이스 프리셋
- 이슈/스타 비율 2.6% — 안정성 양호

**❌ 단점**
- **macOS 전용** — Windows/Linux 빌드 없음. 가장 치명적인 약점
- Bun 런타임, Caddy 등 외부 의존성 필요
- "Other" 라이선스 — 오픈소스 자유도 불투명
- iOS 앱 아직 "출시 예정"

> **추천:** 최대 프로그래밍 가능성(CLI + SDK + MCP)과 최다 에이전트 생태계를 원하는 macOS 개발자.

---

### 4. cmux — manaflow-ai/cmux

| | |
|---|---|
| **GitHub** | [manaflow-ai/cmux](https://github.com/manaflow-ai/cmux) |
| **Stars / Forks / Issues** | 24,412 / 1,970 / 3,446 (14.1%) |
| **언어** | Swift (네이티브 macOS) |
| **라이선스** | Other (GPL-3.0 + 상용 듀얼) |
| **플랫폼** | macOS |
| **웹사이트** | [cmux.com](https://cmux.com/) |

**✅ 장점**
- **GitHub 스타 수 최다 (24.4K)** — 최대 커뮤니티
- **네이티브 성능** — Swift/AppKit + libghostty GPU 렌더링. Electron 대비 압도적 시작 속도·메모리
- **명확한 철학** — "원시 도구(primitive)지 솔루션이 아니다." 워크플로우를 강제하지 않음
- **알림 시스템** — OSC 9/99/777 시퀀스 감지, 파란 링 + 탭 점등, `cmux notify` CLI
- **인앱 브라우저** — agent-browser API 포팅, 접근성 트리 스냅샷·클릭·폼 입력·JS 실행
- **SSH** — `cmux ssh user@remote`로 원격 워크스페이스, 브라우저가 원격 네트워크 경유
- **Claude Code Teams** — `cmux claude-teams` 한 명령으로 teammate 모드, tmux 불필요
- Ghostty config 호환 — 기존 테마/폰트/색상 그대로 사용
- CLI + socket API로 전체 자동화

**❌ 단점**
- **macOS 전용** — 플랫폼 점수 최하위
- **터미널이지 IDE가 아님** — worktree 관리, diff 뷰어, PR 생성 기능 없음
- **이슈 3,446개 (14.1%)** — 비율 최고. 복잡한 네이티브 앱 관리 부담
- 모바일 없음

> **추천:** 네이티브 성능과 터미널 퍼스트, 비강제적 접근을 원하는 macOS 파워 유저. diff 리뷰는 Orca/Emdash/Superset과 조합.

---

### 5. Parallel Code — johannesjo/parallel-code

| | |
|---|---|
| **GitHub** | [johannesjo/parallel-code](https://github.com/johannesjo/parallel-code) |
| **Stars / Forks / Issues** | 838 / 111 / 39 (4.7%) |
| **언어** | TypeScript (Electron + SolidJS) |
| **라이선스** | MIT |
| **플랫폼** | macOS · Linux |
| **웹사이트** | [parallelcode.app](https://parallelcode.app/) |

**✅ 장점**
- **Docker 샌드박싱** — 프로젝트별 `.parallel-code/Dockerfile`로 완전 격리. 다른 OSS 도구에 없는 기능
- **AI Arena** — 에이전트 간 헤드투헤드 경쟁, 승자 머지
- **커버리지 레이더** — 변경 파일별 테스트 커버리지 배지
- **Steps 추적 패널** — 에이전트 진행 타임라인
- 모바일 모니터링 (QR 코드 → Wi-Fi/Tailscale)
- 10개 테마, 키보드 퍼스트, 포커스 모드
- MIT 라이선스, 완전 무료

**❌ 단점**
- 커뮤니티 최소 (838★) — 장기 유지보수 불확실
- Windows 미지원
- SSH/원격 워크트리 없음
- 단일 개발자 프로젝트 (johannesjo)

> **추천:** Docker 격리 에이전트와 헤드투헤드 에이전트 경쟁을 실험하는 개발자.

---

### 6. Claude Squad — smtg-ai/claude-squad

| | |
|---|---|
| **GitHub** | [smtg-ai/claude-squad](https://github.com/smtg-ai/claude-squad) |
| **Stars / Forks / Issues** | 8,108 / 585 / 52 (0.6%) |
| **언어** | Go (TUI) |
| **라이선스** | AGPL-3.0 |
| **플랫폼** | macOS · Linux (tmux 필요) |
| **웹사이트** | [smtg-ai.github.io/claude-squad](https://smtg-ai.github.io/claude-squad/) |

**✅ 장점**
- **최고 안정성** — 0.6% 이슈/스타 비율, Go 바이너리, 단순 아키텍처 (tmux + worktree)
- **가장 빠른 설정** — `brew install claude-squad` → 5초 내 6개 세션 실행
- 키보드 퍼스트 TUI — vim 스타일 네비게이션
- Claude Code, Codex, Aider, Gemini, OpenCode, Amp 지원
- `--autoyes` 플래그로 무인 자동 수락 (실험적)

**❌ 단점**
- **시각적 diff 리뷰 약함** — 별도 도구 필요
- **원격/SSH/모바일 전무** — 로컬 단일 머신만
- AGPL-3.0 — 상업적 임베딩 시 법무 검토 필요
- Windows 미지원 (tmux 의존)

> **추천:** 병렬 에이전트로 가는 가장 빠르고 안정적인 경로를 원하는 터미널 파워 유저. macOS/Linux 솔로 개발자.

---

### 7. Vibe Kanban — BloopAI/vibe-kanban

| | |
|---|---|
| **GitHub** | [BloopAI/vibe-kanban](https://github.com/BloopAI/vibe-kanban) |
| **언어** | Rust (웹 앱) |
| **라이선스** | Apache-2.0 |
| **플랫폼** | Web (크로스플랫폼) |
| **상태** | 커뮤니티 유지보수 (Bloop 2026년 4월 서비스 종료) |

**✅ 장점**
- 칸반 카드 = worktree = 에이전트 — 직관적 메타포
- MCP 서버로 카드 자동 분해 (자율적 태스크 분해에 가장 근접)
- 10+ 에이전트 지원, 인앱 브라우저(디바이스 에뮬레이션 포함)
- 셀프 호스팅 가능, 팀 친화적

**❌ 단점**
- **Bloop 서비스 종료** — 유료 구독 환불, 클라우드 기능 중단
- 하드 태스크 의존성(B가 A를 기다림) 미지원
- 워크트리 20개 시 디스크 부담
- 향후 유지보수 속도가 커뮤니티 기여에 전적 의존

> **추천:** 공유 시각 보드와 MCP 기반 태스크 분해가 필요하고, 커뮤니티 유지보수 소프트웨어에 관대한 팀.

---

### 8. Nimbalyst — nimbalyst.com

| | |
|---|---|
| **웹사이트** | [nimbalyst.com](https://nimbalyst.com/) |
| **플랫폼** | 크로스플랫폼 데스크톱 + iOS + Android |
| **전신** | Crystal (2026년 2월 deprecated) |

**✅ 장점**
- worktree가 세션 객체의 일급 시민 — 세션 시작 시 원클릭 옵션
- 인라인 diff, 시각적 파일 사이드바, GUI 리뷰-머지
- 크로스플랫폼 + iOS 동반 앱
- 마크다운/Excalidraw/목업 시각 편집 내장

**❌ 단점**
- 가장 어린 프로젝트 (2026년 2월 Crystal에서 리브랜딩)
- 커뮤니티·문서·평판 데이터 부족
- 벤더 단일 주도, MIT 라이선스
- 에이전트 지원 좁음 (Claude Code, Codex)

> **추천:** 시각 편집과 함께 worktree 퍼스트 세션 관리를 원하는 개발자. 프로젝트가 성숙하는 6개월 후 재평가 권장.

---

### 9. Intent — Augment Code

| | |
|---|---|
| **웹사이트** | [intentapp.dev](https://www.intentapp.dev/) |
| **플랫폼** | macOS (Windows 대기자 명단, Linux 미발표) |
| **상태** | 공개 베타 |
| **가격** | Augment 크레딧 ($0 트라이얼 / $20–$200/월; BYOA 무료) |

**✅ 장점**
- **스펙 기반 조정** — Living spec이 모든 에이전트의 단일 진실 원천. 스펙을 한 번 수정하면 모든 활성 에이전트에 전파
- **Coordinator → Implementor → Verifier** 3단계 에이전트 분업
- 크로스 서비스 리팩토링에서 진가 — 필드명 변경 등 스펙 레벨 전파
- BYOA (Claude Code, Codex, OpenCode + Auggie)
- Context Engine을 MCP 서버로 노출

**❌ 단점**
- **폐쇄 소스** — 코드 감사 불가, 벤더 종속
- **macOS only** — Windows 대기자, Linux 미발표
- Augment 크레딧 사용 — 기존 Claude/Cursor 구독과 비용 중복
- 공개 베타 — 프로덕션 안정성 미검증

> **추천:** 스펙 기반 조정이 가치 있는 복잡한 크로스 서비스 리팩토링을 수행하는 macOS 팀.

---

### 10. Conductor — Melty Labs

| | |
|---|---|
| **웹사이트** | [conductor.build](https://www.conductor.build/) |
| **플랫폼** | macOS |
| **라이선스** | 폐쇄 소스 |
| **가격** | 무료 (BYO 로그인) |

**✅ 장점**
- macOS에서 가장 세련된 대시보드 — diff-first 리뷰, 깔끔한 UX
- 무료 + BYO Claude/Codex/Cursor/OpenCode 로그인
- 기존 VS Code/JetBrains 옆에 두고 쓰는 최적의 오케스트레이터

**❌ 단점**
- **폐쇄 소스** — 코드 감사 불가, 벤더 종속
- **macOS only** — 크로스플랫폼 "점진적 추가 중"
- CLI/SDK/MCP 없음 — 프로그래밍 불가
- 원격/SSH/모바일 전무
- 에이전트 지원 좁음 (4종)

> **추천:** 기존 에디터 옆에서 병렬 에이전트 오케스트레이션의 가장 쉽고 세련된 진입점을 원하는 macOS 개발자.

---

## 🎯 사용 사례별 추천

| 상황 | 추천 도구 | 이유 |
|----------------|-------------------|-----|
| 크로스플랫폼 팀, 모바일 모니터링 필요 | **Orca** | 3 OS + iOS/Android 지원하는 유일한 도구 |
| 엔터프라이즈, 다수 티켓 시스템 | **Emdash** | 12개 티켓 플랫폼 + 포트 주입 + 프라이버시 |
| macOS + 프로그래밍 가능한 자동화 | **Superset** | CLI + SDK + MCP, Automations |
| macOS + 네이티브 성능 + 터미널 퍼스트 | **cmux** | Swift/AppKit, GPU 렌더링, 알림 시스템 |
| 터미널만으로 빠르게 시작 | **Claude Squad** | 5초 설정, 최고 안정성 |
| Docker 격리 + 에이전트 경쟁 | **Parallel Code** | AI Arena, 프로젝트별 Dockerfile |
| 스펙 기반 크로스 서비스 리팩토링 | **Intent** | Living spec 전파, Coordinator/Verifier |
| 무료, 가장 쉬운 Mac 시작 | **Conductor** | 무료 + BYO 로그인, 최고 폴리싱 |

---

## 📈 기능 비교 매트릭스

| 도구 | Worktree | Diff 리뷰 | Remote/SSH | 모바일 | 브라우저 | CLI/SDK/MCP | 자동화 | 티켓 통합 |
|------|:--------:|:-----------:|:----------:|:------:|:-------:|:-----------:|:-----------:|:-----------------:|
| **Orca** | ✅ | ✅ | ✅ | ✅ iOS+Android | ✅ Design Mode | ✅ CLI | ❌ | GitHub·Linear |
| **Emdash** | ✅ | ✅ | ✅ SSH/SFTP | ❌ | ❌ | ❌ | ❌ | 12개 플랫폼 |
| **Superset** | ✅ | ✅ | ✅ | 🔄 iOS 예정 | ✅ | ✅ CLI+SDK+MCP | ✅ | Slack·Linear |
| **cmux** | ❌ | ❌ | ✅ | ❌ | ✅ | ✅ CLI+Socket | ❌ | ❌ |
| **Parallel Code** | ✅ | ✅ | ❌ | ✅ QR | ❌ | ❌ | ❌ | ❌ |
| **Claude Squad** | ✅ | ⚠️ 약함 | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ |
| **Vibe Kanban** | ✅ | ✅ | ❌ | ❌ | ✅ | ✅ MCP | ❌ | ❌ |
| **Nimbalyst** | ✅ | ✅ | ❌ | ✅ iOS | ❌ | ❌ | ❌ | ❌ |
| **Intent** | ✅ | ✅ | ❌ | ❌ | ✅ | ✅ MCP | ❌ | ❌ |
| **Conductor** | ✅ | ✅ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ |

---

## 🌐 더 넓은 생태계

이들은 agent-native IDE는 아니지만, worktree/병렬 에이전트 기능을 흡수하여 알아둘 가치가 있습니다:

| 도구 | 카테고리 | Agent-Native 기능 |
|------|----------|---------------------|
| [Cursor 3](https://cursor.com/) | 전용 IDE | `/worktree` 및 `/best-of-n` 명령이 있는 Agents Window (2026.04) |
| [Windsurf Wave 13](https://windsurf.com/) | 전용 IDE | worktree 기반 병렬 Cascade 세션, 전용 에이전트 터미널 |
| [Google Antigravity](https://antigravity.google/) | 전용 IDE | 멀티 에이전트 병렬 워크스페이스, 무료, 동적 서브에이전트 |
| [Cline](https://cline.bot/) | VS Code 확장 | 모델 독립적, 오픈소스 에이전트 |
| [Roo Code](https://roocode.com/) | VS Code 확장 | 멀티 페르소나 에이전트 시스템 (Coder, Architect, Debugger) |
| [Claude Code](https://claude.com/product/claude-code) | 터미널 에이전트 | 서브에이전트 frontmatter의 `isolation: worktree` 내장 |
| [Aider](https://aider.chat/) | 터미널 에이전트 | 에디터 독립적, Git 네이티브 CLI 페어 프로그래밍 |

---

## 📅 시장 관찰 (2026년 7월)

1. **Orca와 Emdash가 1티어 형성** — 크로스플랫폼, 오픈소스, 풍부한 기능, 양호한 안정성.
2. **cmux는 커뮤니티 규모와 성능으로 독보적** — 하지만 macOS 전용 + 터미널 한계.
3. **Superset은 기능 깊이 최상급** — 하지만 macOS 전용이 치명적.
4. **폐쇄 소스 도구(Conductor, Intent)가 최하위** — 오픈소스 자유도에서 근본적 불리.
5. **Git worktree가 합의된 격리 원시 도구** — 모든 serious tool이 채택.
6. **포트 충돌이 다음 프론티어** — Emdash(`$EMDASH_PORT`)만이 설정 레벨에서 해결.
7. **모바일 모니터링 부상** — Orca(iOS+Android), Parallel Code(QR), Nimbalyst(iOS) 선도.
8. **카테고리 통합 진행 중** — Crystal→Nimbalyst, Bloop→커뮤니티 Vibe Kanban. 2026 H2 추가 M&A와 종료 예상.

---

## 🤝 기여

기여를 환영합니다! 도구 추가, 점수 업데이트, 부정확성 수정이 필요하시면:

1. [이슈](https://github.com/pinion05/awesome-agent-ide/issues)를 열어 제안을 남겨주세요
2. 또는 업데이트된 데이터와 출처를 포함하여 PR을 제출해 주세요

점수 변경 시 **검증 가능한 출처**(GitHub 저장소, 문서, 리뷰 기사)를 포함해 주세요.

---

## 📄 라이선스

[CC0-1.0](LICENSE) — 퍼블릭 도메인. 자유롭게 사용하세요.

---

<div align="center">

**[🌐 웹사이트 보기](https://pinion05.github.io/awesome-agent-ide/)** · **[⭐ GitHub에서 Star](https://github.com/pinion05/awesome-agent-ide)**

*최종 업데이트: 2026년 7월 · 관리: [pinion05](https://github.com/pinion05)*

</div>
