<div align="center">

# 🚀 Awesome Agent-Native IDE

### Una comparación clasificada de IDEs y orquestadores construidos para la era de los agentes de codificación con IA

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

## 📖 ¿Qué es un IDE Agent-Native?

Los IDEs tradicionales (Cursor, Windsurf, VS Code) añaden funciones de IA a un editor existente. Los **IDEs Agent-Native** están diseñados desde cero para ejecutar, gestionar y revisar **múltiples agentes de codificación CLI** (Claude Code, Codex, Gemini CLI, etc.) en paralelo.

Características principales:

| Función | Descripción |
|---------|-------------|
| **Aislamiento con Git Worktree** | Cada agente tiene su propia rama y directorio de trabajo, compartiendo una base de datos `.git` |
| **Ejecución paralela multi-agente** | Monitorea 5–20+ agentes simultáneamente desde una pantalla |
| **Revisión de Diff + Flujo de Merge** | Revisa los cambios generados por el agente en un solo lugar antes de fusionar |
| **BYOA (Bring Your Own Agent)** | Ejecuta cualquier agente CLI con tu propia suscripción — sin dependencia de proveedor |

> **Fuera de alcance:** IDEs tradicionales con IA añadida (Cursor, Windsurf, Copilot). Son herramientas excelentes, pero esta lista se centra en herramientas cuyo *propósito principal* es la orquestación de agentes.

---

## 🏆 Ranking General

| Puesto | Herramienta | Puntuación | Plataforma | Licencia | Stars | Resumen |
|:------:|------|:----------:|----------|---------|:-----:|-----------|
| 🥇 | [**Orca**](https://github.com/stablyai/orca) | **8.6** | macOS·Win·Linux·📱 | MIT | 18.3K | Multiplataforma completa + móvil, Design Mode, lanzamientos diarios |
| 🥈 | [**Emdash**](https://github.com/generalaction/emdash) | **8.3** | macOS·Win·Linux | Apache-2.0 | 5.1K | Inyección de puertos, 8 integraciones de tickets, 28+ agentes |
| 🥉 | [**Superset**](https://github.com/superset-sh/superset) | **7.5** | macOS | Other | 12.4K | CLI + SDK + MCP, automatizaciones, mayor soporte de agentes |
| 4 | [**cmux**](https://github.com/manaflow-ai/cmux) | **7.0** | macOS | GPL | 24.4K | Rendimiento nativo Swift, comunidad más grande, terminal-first |
| 5 | [**Parallel Code**](https://github.com/johannesjo/parallel-code) | **6.7** | macOS·Linux | MIT | 0.8K | Sandbox Docker, AI Arena, radar de cobertura |
| 6 | [**Claude Squad**](https://github.com/smtg-ai/claude-squad) | **6.5** | macOS·Linux | AGPL-3.0 | 8.1K | Mejor estabilidad (0.6%), configuración más rápida |
| 7 | [**Vibe Kanban**](https://github.com/BloopAI/vibe-kanban) | **6.3** | Web | Apache-2.0 | — | Kanban + descomposición MCP (mantenido por la comunidad) |
| 8 | [**Nimbalyst**](https://nimbalyst.com/) | **6.2** | Multiplataforma·📱 | — | — | Worktree de primera clase, edición visual, compañero iOS |
| 9 | [**Intent**](https://www.intentapp.dev/) | **6.1** | macOS | Cerrado | — | Coordinación basada en specs, agentes Coordinator/Verifier |
| 10 | [**Conductor**](https://www.conductor.build/) | **5.7** | macOS | Cerrado | — | Mejor pulido en Mac, gratis, BYO login |

---

## 📊 Metodología de Puntuación

Cada herramienta se evalúa en **7 dimensiones** (escala 1–10), ponderadas para producir una puntuación compuesta.

| Dimensión | Peso | Qué evaluamos |
|-----------|:----:|------------------|
| **Profundidad Técnica** | 20% | Modelo de aislamiento (worktree/container), profundidad de coordinación, calidad de arquitectura, tecnología única (Design Mode, Computer Use, inyección de puertos) |
| **Estabilidad** | 15% | Ratio issue/star, frecuencia de lanzamientos, madurez del código, estabilidad de ejecución (nativo vs Electron) |
| **UX / Conveniencia** | 15% | Facilidad de instalación, revisión visual de diff, atajos de teclado, sistema de notificaciones, pulido del flujo de trabajo |
| **Ecosistema** | 15% | Agentes soportados, integraciones de tickets (Linear/GitHub/Jira), disponibilidad de CLI/SDK/MCP, tamaño de comunidad |
| **Escalabilidad** | 15% | Ejecución remota (SSH), compañero móvil, capacidad paralela, programabilidad |
| **Soporte de Plataforma** | 10% | Cobertura de SO (macOS / Windows / Linux / móvil) |
| **Salud Open Source** | 10% | Libertad de licencia, independencia del proveedor, desarrollo impulsado por la comunidad |

### Puntuaciones Detalladas

| Herramienta | Técnica (20%) | Estabilidad (15%) | UX (15%) | Ecosistema (15%) | Escalabilidad (15%) | Plataforma (10%) | OSS (10%) | **Total** |
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

## 🔍 Análisis Detallado por Herramienta

### 🥇 1. Orca — stablyai/orca

| | |
|---|---|
| **GitHub** | [stablyai/orca](https://github.com/stablyai/orca) |
| **Stars / Forks / Issues** | 18,327 / 1,448 / 1,361 (7.4%) |
| **Lenguaje** | TypeScript (Electron) |
| **Licencia** | MIT |
| **Plataforma** | macOS · Windows · Linux · iOS · Android |
| **Sitio web** | [onorca.dev](https://www.onorca.dev/) |

**✅ Fortalezas**
- **Único multiplataforma completo + móvil** — App companion iOS/Android para monitoreo y seguimiento desde cualquier lugar
- **Design Mode** — Clic en cualquier elemento UI en una ventana real de Chromium; HTML/CSS/screenshot enviado directamente al prompt del agente. Único de Orca
- **SSH Worktrees** — Ejecuta agentes en una máquina remota potente con reconexión automática y reenvío de puertos
- **Computer Use** — Los agentes pueden operar aplicaciones de escritorio e interfaces visibles
- **GitHub & Linear nativo** — Explora PRs, issues y tableros en la app; abre un worktree desde cualquier tarea
- **Anotar AI Diffs** — Deja comentarios en cualquier línea de diff y envíalos al agente
- **Lanzamientos diarios** — Publica cada día; el changelog es la verdadera lista de funciones
- Terminales clase Ghostty (WebGL), divisiones infinitas, historial que sobrevive reinicios

**❌ Debilidades**
- Basado en Electron — más pesado que alternativas nativas (cmux)
- 1,361 issues abiertos — activo pero la carga de gestión es real
- MIT pero liderado por stablyai — dependencia de un solo proveedor

> **Ideal para:** Equipos distribuidos que necesitan monitoreo móvil, soporte multiplataforma y el conjunto de funciones agent-native más rico.

---

### 🥈 2. Emdash — generalaction/emdash

| | |
|---|---|
| **GitHub** | [generalaction/emdash](https://github.com/generalaction/emdash) |
| **Stars / Forks / Issues** | 5,149 / 534 / 132 (2.6%) |
| **Lenguaje** | TypeScript (Electron) |
| **Licencia** | Apache-2.0 |
| **Plataforma** | macOS · Windows · Linux |
| **Sitio web** | [emdash.sh](https://emdash.sh/) |
| **Respaldo** | YC W26 |

**✅ Fortalezas**
- **Integración de tickets más amplia** — Linear, GitHub, Jira, GitLab, Asana, Monday.com, Forgejo, Plain (8 plataformas)
- **Inyección `$EMDASH_PORT`** — Resuelve el problema de colisión de puertos a nivel de configuración, lo que casi ninguna otra herramienta maneja
- **Soporte de agentes más amplio** — 28+ proveedores CLI detectados automáticamente (Claude Code, Codex, Cursor, OpenCode, Amp, Devin, Qwen Code, Droid, Copilot, etc.)
- **Proyectos remotos SSH/SFTP** — Mismo flujo de trabajo paralelo en bases de código remotas, autenticación con llavero del SO
- **Local-first + privacidad** — Almacenamiento SQLite local, no envía código/chat a servidores Emdash
- Multiplataforma + Apache-2.0 — combinación de licencia más permisiva
- Ratio issue/star 2.6% — indicador de estabilidad excelente

**❌ Debilidades**
- Sin app companion móvil
- Sin coordinación entre agentes — cada uno funciona independientemente
- Lanzado a principios de 2026; comunidad aún creciendo

> **Ideal para:** Equipos empresariales que necesitan integración de tickets, aislamiento de puertos y soporte multiplataforma con fuertes garantías de privacidad.

---

### 🥉 3. Superset — superset-sh/superset

| | |
|---|---|
| **GitHub** | [superset-sh/superset](https://github.com/superset-sh/superset) |
| **Stars / Forks / Issues** | 12,399 / 1,076 / 323 (2.6%) |
| **Lenguaje** | TypeScript (Electron) |
| **Licencia** | Other |
| **Plataforma** | macOS |
| **Sitio web** | [superset.sh](https://superset.sh/) |
| **Respaldo** | YC |

**✅ Fortalezas**
- **Mayor variedad de superficies de acceso** — App de escritorio + CLI + TypeScript SDK + servidor MCP. Controla workspaces desde cualquier lugar
- **Soporte de agentes más amplio** — Amp, Claude Code, Codex, Cursor, Droid, Gemini, Copilot, Mastra, Mistral Vibe, OpenCode, Pi, Polygraph + agentes personalizados
- **Automatizaciones** — Programa sesiones de agentes con temporizador
- **Integración Slack & Linear** — Crea workspaces desde mensajes de Slack o issues de Linear
- **Navegador integrado + detección de puertos** — Vista previa de servidores dev por workspace
- Soporte de agentes personalizados con iconos, presets de workspace
- Ratio issue/star 2.6% — buena estabilidad

**❌ Debilidades**
- **Solo macOS** — Sin builds para Windows/Linux. La debilidad más crítica
- Requiere runtime Bun, Caddy y otras dependencias externas
- Licencia "Other" — libertad open source poco clara
- App iOS aún "próximamente"

> **Ideal para:** Desarrolladores en macOS que quieren máxima programabilidad (CLI + SDK + MCP) y el ecosistema de agentes más amplio.

---

### 4. cmux — manaflow-ai/cmux

| | |
|---|---|
| **GitHub** | [manaflow-ai/cmux](https://github.com/manaflow-ai/cmux) |
| **Stars / Forks / Issues** | 24,412 / 1,970 / 3,446 (14.1%) |
| **Lenguaje** | Swift (macOS nativo) |
| **Licencia** | GPL |
| **Plataforma** | macOS |
| **Sitio web** | [cmux.com](https://cmux.com/) |

**✅ Fortalezas**
- **Más estrellas en GitHub (24.4K)** — comunidad más grande
- **Rendimiento nativo** — Swift/AppKit + renderizado GPU libghostty. Supera a Electron en velocidad de inicio y memoria
- **Filosofía clara** — "Una primitiva, no una solución." No te impone un flujo de trabajo
- **Sistema de notificaciones** — Detección de secuencias OSC 9/99/777, anillo azul + resaltado de pestaña, CLI `cmux notify`
- **Navegador integrado** — API agent-browser portada; snapshots de árbol de accesibilidad, clic, llenado de formularios, evaluación JS
- **SSH** — `cmux ssh user@remote` crea workspaces remotos; el navegador se enruta a través de la red remota
- **Claude Code Teams** — `cmux claude-teams` activa el modo teammate con un comando, sin tmux
- Compatible con config de Ghostty — tus temas/fuentes/colores existentes funcionan
- CLI + socket API para automatización completa

**❌ Debilidades**
- **Solo macOS** — puntuación de plataforma más baja
- **Es un terminal, no un IDE** — sin gestión de worktree, visor de diff o creación de PR integrados
- **3,446 issues abiertos (14.1%)** — ratio más alto; carga de gestión de app nativa compleja
- Sin compañero móvil

> **Ideal para:** Power users de macOS que quieren rendimiento nativo y un enfoque terminal-first, no prescriptivo. Combina con Orca/Emdash/Superset para revisión de diff.

---

### 5. Parallel Code — johannesjo/parallel-code

| | |
|---|---|
| **GitHub** | [johannesjo/parallel-code](https://github.com/johannesjo/parallel-code) |
| **Stars / Forks / Issues** | 838 / 111 / 39 (4.7%) |
| **Lenguaje** | TypeScript (Electron + SolidJS) |
| **Licencia** | MIT |
| **Plataforma** | macOS · Linux |
| **Sitio web** | [parallelcode.app](https://parallelcode.app/) |

**✅ Fortalezas**
- **Sandbox Docker** — `.parallel-code/Dockerfile` específico del proyecto para aislamiento completo. Ningún otro OSS lo tiene
- **AI Arena** — Competencia cabeza a cabeza entre agentes, fusiona al ganador
- **Radar de cobertura** — Insignias de cobertura de pruebas por archivo en el panel de archivos modificados
- **Panel de seguimiento de pasos** — Línea de tiempo de progreso del agente estilo gerente de ingeniería
- Monitoreo móvil vía código QR (Wi-Fi/Tailscale)
- 10 temas, teclado primero, modo enfoque
- Licencia MIT, completamente gratis

**❌ Debilidades**
- Comunidad más pequeña (838★) — mantenimiento a largo plazo incierto
- Sin soporte Windows
- Sin worktrees SSH/remotos
- Proyecto de un solo desarrollador (johannesjo)

> **Ideal para:** Desarrolladores que experimentan con agentes aislados en Docker y competencia entre agentes.

---

### 6. Claude Squad — smtg-ai/claude-squad

| | |
|---|---|
| **GitHub** | [smtg-ai/claude-squad](https://github.com/smtg-ai/claude-squad) |
| **Stars / Forks / Issues** | 8,108 / 585 / 52 (0.6%) |
| **Lenguaje** | Go (TUI) |
| **Licencia** | AGPL-3.0 |
| **Plataforma** | macOS · Linux (requiere tmux) |
| **Sitio web** | [smtg-ai.github.io/claude-squad](https://smtg-ai.github.io/claude-squad/) |

**✅ Fortalezas**
- **Mejor estabilidad** — ratio issue/star 0.6%, binario Go, arquitectura simple (tmux + worktree)
- **Configuración más rápida** — `brew install claude-squad` → 6 sesiones en 5 segundos
- TUI teclado primero con navegación estilo vim
- Soporta Claude Code, Codex, Aider, Gemini, OpenCode, Amp
- Flag `--autoyes` para aceptación automática desatendida (experimental)

**❌ Debilidades**
- **Revisión visual de diff débil** — necesita herramienta separada
- **Sin remoto/SSH/móvil** — solo máquina local
- AGPL-3.0 — revisión legal necesaria para uso comercial embebido
- Sin soporte Windows (dependencia de tmux)

> **Ideal para:** Power users de terminal que quieren el camino más rápido y estable a agentes en paralelo. Desarrolladores individuales en macOS/Linux.

---

### 7. Vibe Kanban — BloopAI/vibe-kanban

| | |
|---|---|
| **GitHub** | [BloopAI/vibe-kanban](https://github.com/BloopAI/vibe-kanban) |
| **Lenguaje** | TypeScript (Web app) |
| **Licencia** | Apache-2.0 |
| **Plataforma** | Web (multiplataforma) |
| **Estado** | Mantenido por la comunidad (Bloop cerró en abril 2026) |

**✅ Fortalezas**
- Tarjeta Kanban = worktree = agente — metáfora intuitiva
- Servidor MCP para descomposición autónoma de tarjetas (lo más cercano a descomposición autónoma de tareas)
- 10+ agentes soportados, navegador integrado con emulación de dispositivos
- Auto-hosteable, amigable para equipos

**❌ Debilidades**
- **Bloop cerró** — suscripciones reembolsadas, funciones en la nube descontinuadas
- Sin dependencias estrictas de tareas (tarea B esperando a tarea A)
- 20 worktrees → sobrecarga de disco
- La velocidad de mantenimiento futuro depende completamente de contribuyentes de la comunidad

> **Ideal para:** Equipos que quieren un tablero visual compartido con descomposición de tareas vía MCP, cómodos con software mantenido por la comunidad.

---

### 8. Nimbalyst — nimbalyst.com

| | |
|---|---|
| **Sitio web** | [nimbalyst.com](https://nimbalyst.com/) |
| **Plataforma** | Escritorio multiplataforma + iOS |
| **Predecesor** | Crystal (descatalogado feb 2026) |

**✅ Fortalezas**
- Worktree como primitiva de primera clase en el objeto de sesión — opción de un clic al iniciar
- Diffs en línea, barra lateral visual de archivos, revisión y fusión en GUI
- Multiplataforma + compañero iOS
- Edición visual de Markdown/Excalidraw/mockups integrada

**❌ Debilidades**
- Proyecto más joven (renombrado de Crystal en feb 2026)
- Comunidad, documentación y datos de reputación limitados
- Liderado por proveedor, licencia poco clara
- Soporte de agentes limitado (Claude Code, Codex)

> **Ideal para:** Desarrolladores que quieren gestión de sesiones worktree-first con edición visual. Reevaluar en 6 meses cuando el proyecto madure.

---

### 9. Intent — Augment Code

| | |
|---|---|
| **Sitio web** | [intentapp.dev](https://www.intentapp.dev/) |
| **Plataforma** | macOS (Windows en lista de espera, Linux no anunciado) |
| **Estado** | Beta pública |
| **Precio** | Créditos Augment ($0 prueba / $20–$60/mes) |

**✅ Fortalezas**
- **Coordinación basada en specs** — Una spec viva es la fuente única de verdad para cada agente. Edita la spec una vez; las actualizaciones se propagan a todos los agentes activos
- **Coordinator → Implementor → Verifier** división de trabajo de tres agentes
- Brilla en refactors entre servicios — los cambios de nombres de campos se propagan vía spec
- BYOA (Claude Code, Codex, OpenCode + Auggie)
- Context Engine expuesto como servidor MCP

**❌ Debilidades**
- **Código cerrado** — sin auditoría de código, dependencia de proveedor
- **Solo macOS** — Windows en lista de espera, Linux no anunciado
- Usa créditos Augment — solapamiento de costos con suscripciones existentes de Claude/Cursor
- Beta pública — estabilidad de producción no verificada

> **Ideal para:** Equipos en macOS que hacen refactors complejos entre servicios y se benefician de la coordinación basada en specs.

---

### 10. Conductor — Melty Labs

| | |
|---|---|
| **Sitio web** | [conductor.build](https://www.conductor.build/) |
| **Plataforma** | macOS |
| **Licencia** | Código cerrado |
| **Precio** | Gratis (BYO login) |

**✅ Fortalezas**
- Dashboard más pulido en Mac — revisión diff-first, UX limpia en general
- Gratis con BYO login de Claude/Codex/Cursor/OpenCode
- Mejor herramienta solo-orquestador junto a tu VS Code o JetBrains existente

**❌ Debilidades**
- **Código cerrado** — sin auditoría de código, dependencia de proveedor
- **Solo macOS** — multiplataforma "llegando gradualmente"
- Sin CLI/SDK/MCP — no programable
- Sin remoto/SSH/móvil
- Soporte de agentes limitado (4 agentes)

> **Ideal para:** Desarrolladores en macOS que quieren el punto de entrada más fácil y pulido a la orquestación paralela de agentes junto a su editor existente.

---

## 🎯 Guía de Decisión por Caso de Uso

| Situación | Herramienta Recomendada | Por qué |
|----------------|-------------------|-----|
| Equipo multiplataforma, necesita monitoreo móvil | **Orca** | Única herramienta con 3 SO + iOS/Android |
| Empresa, múltiples sistemas de tickets | **Emdash** | 8 plataformas de tickets + inyección de puertos + privacidad |
| macOS + automatización programable | **Superset** | CLI + SDK + MCP, Automatizaciones |
| macOS + rendimiento nativo + terminal-first | **cmux** | Swift/AppKit, renderizado GPU, notificaciones |
| Solo terminal, inicio más rápido | **Claude Squad** | Configuración de 5 segundos, mejor estabilidad |
| Aislamiento Docker + competencia de agentes | **Parallel Code** | AI Arena, Dockerfiles específicos del proyecto |
| Refactors entre servicios basados en specs | **Intent** | Propagación de spec viva, Coordinator/Verifier |
| Gratis, incorporation más fácil en Mac | **Conductor** | Gratis + BYO login, mejor pulido |

---

## 📈 Matriz de Comparación de Funciones

| Herramienta | Worktree | Revisión Diff | Remoto/SSH | Móvil | Navegador | CLI/SDK/MCP | Automatizaciones | Integración Tickets |
|------|:--------:|:-----------:|:----------:|:------:|:-------:|:-----------:|:-----------:|:-----------------:|
| **Orca** | ✅ | ✅ | ✅ | ✅ iOS+Android | ✅ Design Mode | ✅ CLI | ❌ | GitHub·Linear |
| **Emdash** | ✅ | ✅ | ✅ SSH/SFTP | ❌ | ❌ | ❌ | ❌ | 8 plataformas |
| **Superset** | ✅ | ✅ | ✅ | 🔄 iOS pronto | ✅ | ✅ CLI+SDK+MCP | ✅ | Slack·Linear |
| **cmux** | ❌ | ❌ | ✅ | ❌ | ✅ | ✅ CLI+Socket | ❌ | ❌ |
| **Parallel Code** | ✅ | ✅ | ❌ | ✅ QR | ❌ | ❌ | ❌ | ❌ |
| **Claude Squad** | ✅ | ⚠️ débil | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ |
| **Vibe Kanban** | ✅ | ✅ | ❌ | ❌ | ✅ | ✅ MCP | ❌ | ❌ |
| **Nimbalyst** | ✅ | ✅ | ❌ | ✅ iOS | ❌ | ❌ | ❌ | ❌ |
| **Intent** | ✅ | ✅ | ❌ | ❌ | ✅ | ✅ MCP | ❌ | ❌ |
| **Conductor** | ✅ | ✅ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ |

---

## 🌐 Ecosistema Más Amplio

Estos **no** son IDEs agent-native, pero han absorbido funciones de worktree/agentes paralelos y vale la pena conocerlos:

| Herramienta | Categoría | Función Agent-Native |
|------|----------|---------------------|
| [Cursor 3](https://cursor.com/) | IDE dedicado | Agents Window con comandos `/worktree` y `/best-of-n` (abr 2026) |
| [Windsurf Wave 13](https://windsurf.com/) | IDE dedicado | Sesiones Cascade paralelas con worktrees, terminal de agente dedicado |
| [Google Antigravity](https://antigravity.google/) | IDE dedicado | Workspaces paralelos multi-agente, gratis, subagentes dinámicos |
| [Cline](https://cline.bot/) | Extensión VS Code | Agente open-source agnóstico de modelo |
| [Roo Code](https://roocode.com/) | Extensión VS Code | Sistema de agentes multi-persona (Coder, Architect, Debugger) |
| [Claude Code](https://claude.com/product/claude-code) | Agente terminal | `isolation: worktree` integrado en subagent frontmatter |
| [Aider](https://aider.chat/) | Agente terminal | Agnóstico de editor, pair programming CLI nativo de Git |

---

## 📅 Observaciones del Mercado (Julio 2026)

1. **Orca y Emdash forman el tier superior** — multiplataforma, open-source, funciones ricas, buena estabilidad.
2. **cmux domina en tamaño de comunidad y rendimiento** — pero solo macOS y solo terminal.
3. **Superset tiene el conjunto de funciones más profundo** — pero solo macOS es una limitación crítica.
4. **Las herramientas de código cerrado (Conductor, Intent) puntúan más bajo** — desventaja estructural en libertad open source.
5. **Git worktree es la primitiva de aislamiento de consenso** — todas las herramientas serias lo usan.
6. **La colisión de puertos es la próxima frontera** — solo Emdash (`$EMDASH_PORT`) la resuelve a nivel de configuración.
7. **El monitoreo móvil está emergiendo** — Orca (iOS+Android), Parallel Code (QR), Nimbalyst (iOS) lideran.
8. **La categoría se está consolidando** — Crystal → Nimbalyst, Bloop → comunidad Vibe Kanban. Se esperan más M&A y cierres en H2 2026.

---

## 🤝 Contribuir

¡Las contribuciones son bienvenidas! Si deseas añadir una herramienta, actualizar puntuaciones o corregir una inexactitud:

1. Abre un [issue](https://github.com/pinion05/awesome-agent-ide/issues) con tu sugerencia
2. O envía un PR con datos y fuentes actualizados

Por favor incluye **fuentes verificables** (repositorios de GitHub, documentación, artículos de revisión) para cualquier cambio de puntuación.

---

## 📄 Licencia

[CC0-1.0](LICENSE) — Dominio público. Úsalo como quieras.

---

<div align="center">

**[🌐 Ver como sitio web](https://pinion05.github.io/awesome-agent-ide/)** · **[⭐ Star en GitHub](https://github.com/pinion05/awesome-agent-ide)**

*Última actualización: Julio 2026 · Mantenido por [pinion05](https://github.com/pinion05)*

</div>
