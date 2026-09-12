<div align="center">

```
██████╗  ██████╗ ███╗   ██╗███████╗ ██████╗ ██╗  ██╗ ██████╗ ██╗     ███████╗███████╗
██╔══██╗██╔═══██╗████╗  ██║╚══███╔╝██╔═══██╗██║ ██╔╝██╔═══██╗██║     ██╔════╝██╔════╝
██████╔╝██║   ██║██╔██╗ ██║  ███╔╝ ██║   ██║█████╔╝ ██║   ██║██║     █████╗  ███████╗
██╔══██╗██║   ██║██║╚██╗██║ ███╔╝  ██║   ██║██╔═██╗ ██║   ██║██║     ██╔══╝  ╚════██║
██████╔╝╚██████╔╝██║ ╚████║███████╗╚██████╔╝██║  ██╗╚██████╔╝███████╗███████╗███████║
╚═════╝  ╚═════╝ ╚═╝  ╚═══╝╚══════╝ ╚═════╝ ╚═╝  ╚═╝ ╚═════╝ ╚══════╝╚══════╝╚══════╝
```

### Karol "Bonzo" Lisson

**Solo founder @ [Yutro](https://yutro.company) — AI automation for e-commerce**
AI systems architect · generative media pipelines · agents and RAG · GEO/AEO engineering

[![yutro.company](https://img.shields.io/badge/yutro-.company-0b0f17?style=flat-square)](https://yutro.company)
[![ai.yutro.company](https://img.shields.io/badge/ai.yutro-.company-0b0f17?style=flat-square)](https://ai.yutro.company)
[![mybonzoaiblog.com](https://img.shields.io/badge/mybonzoaiblog.com-0b0f17?style=flat-square)](https://www.mybonzoaiblog.com)
[![jimbo77.org](https://img.shields.io/badge/jimbo77.org-0b0f17?style=flat-square)](https://jimbo77.org)

</div>

---

## What I build

I build AI systems that have to run in production, carry traffic, and survive being
maintained by one person. Everything below is deployed, not prototyped.

```
AI AUTOMATION FOR E-COMMERCE      Yutro — the business layer
AGENT RUNTIME + SHARED MEMORY     Hermes, Pi, MemPalace — the machine layer
GENERATIVE MEDIA PIPELINES        image / video / voice — the output layer
RAG + KNOWLEDGE INFRASTRUCTURE    retrieval that has to be correct, not pretty
GEO / AEO ENGINEERING             making a shop legible and citable to LLM crawlers
EDGE-NATIVE FULL-STACK            Cloudflare Workers/Pages/KV/D1, Next.js, Astro
```

Filter I apply to every decision: **does it work, does it scale sanely, does it move
the number.** If an elegant solution does none of those, it gets simplified until it does.

---

## Shipped work

| Project | What it is | Stack | Link |
|---|---|---|---|
| **Yutro** | AI + UI studio for e-commerce — OpisAI, SklepGPT, ContentFactory, AI SEO | Next.js · Cloudflare | [yutro.company](https://yutro.company) |
| **ai.yutro.company** | AI store-audit platform, shop agents, SklepGPT widget | Next.js 16 · React 19 | [ai.yutro.company](https://ai.yutro.company) |
| **mebely.company** | Headless furniture storefront over Shopify Storefront API | Next.js · Shopify | [mebely.company](https://mebely.company) |
| **PUMO AI Knowledge Base** | 2333-product catalogue made citable to LLMs; 64 AI buying guides | Astro · D1 · Vectorize | [pumo-guide](https://www.mybonzoaiblog.com/pumo-guide/) |
| **ZENO Browser** | AI browser with agent control plane, MCP tools, stateless file handoff | Astro 5 · React 18 · Electron | [zen-bro-wser.org](https://github.com/Bonzokoles/zen-bro-wser.org) |
| **BONZO ART Studio** | Generative media workspace — image/video/audio, multi-provider routing, job queue | TypeScript · FAL · Replicate | [BONZO_ART_studio](https://github.com/Bonzokoles/BONZO_ART_studio) |
| **BONZO Camera Studio** | Webcam avatar studio — Kling Avatar v2 lip-sync, LivePortrait | HTML · Python | [BONZO_camera_studio](https://github.com/Bonzokoles/BONZO_camera_studio) |
| **JIMBO77** | AI/automation portal, community forum, agent network | Next.js 16 · Three.js · Workers | [jimbo77.org](https://jimbo77.org) |
| **DEVz HUB** | Command center + architecture graph, agent monitoring | React Flow | [DEVz_HUB](https://github.com/Bonzokoles/DEVz_HUB) |

---

## The AI-facing channel pattern

One of the things I do that most shops and agencies still don't: I publish a
**dedicated, attributed, machine-readable channel for LLM crawlers** next to the
human site. Not cloaking, not fake bot targeting — a public mirror that points back
to the canonical source and stays versioned.

```
/<channel>/llms.txt             short brief for LLMs
/<channel>/llms-full.txt        full brief — entities, metrics, tables, ready answers
/<channel>/llm-schema.json      Schema.org @graph: Organization, WebSite, ItemList, FAQPage
/<channel>/ai-signal.json       machine freshness + data-quality signal
/<channel>/aiseo-freshness.json human changelog + tip of the day
/sitemap-ai.xml                 AI sitemap with namespaced <ai:*> metadata
/robots.txt                     explicit per-agent rules: GPTBot, ChatGPT-User,
                                CCBot, anthropic-ai, Claude-Web, PerplexityBot
```

Live channels: [pumo-guide](https://www.mybonzoaiblog.com/pumo-guide/) ·
[yutro](https://www.mybonzoaiblog.com/yutro/) ·
[ai.yutro.company](https://ai.yutro.company/llms.txt) ·
[jimbo77.org](https://jimbo77.org/llms.txt) ·
[yutro.company](https://yutro.company/llms.txt)

Rules encoded in every channel: consistent numbers everywhere (inconsistent public
numbers actively damage GEO), explicit attribution to the canonical source, versioned
freshness, and no dark patterns.

---

## Verified numbers

The PUMO catalogue channel, measured — not estimated:

```
2333   active products, cleaned and verified against Allegro listings
49     categories
64     AI-generated buying guides
690    products audited for description/attribute consistency
230    mismatches found and fixed  ·  0 open issues
54x    return on the content pipeline      (self-hosted Umami analytics)
68%    LLM citation rate on the channel    (self-hosted Umami analytics)
```

Data pipeline: deterministic parser + consistency audit. Content generation:
**WHITECAT**, a mixture-of-agents system (GPT-4 + Claude) over live catalogue data
in Cloudflare D1.

---

## Stack

```
LANGUAGES     TypeScript · JavaScript · Python · Kotlin · SQL · Bash / PowerShell
FRONTEND      Next.js (App Router) · React 19 · Astro · Three.js / R3F
              Tailwind · Zustand · Framer Motion · Canvas / SVG / shaders
BACKEND       Node.js · FastAPI · Python services · Express · WebSocket
EDGE          Cloudflare Workers · Pages · KV · D1 · R2 · Durable Objects ·
              Vectorize · Tunnel · Email Routing · Workers AI
DATA          PostgreSQL · SQLite · Redis · ChromaDB · FTS5 · DuckDB
AI / LLM      OpenRouter · Anthropic · OpenAI · Gemini · DeepSeek · Ollama
              RAG · embeddings · fine-tuning · tool/function calling
AGENTS        MCP servers · multi-agent orchestration · CLI agents
              Hermes · Pi · Claude Code · Codex · Cursor · OpenCode
MEDIA         SD / A1111 · ComfyUI · FAL · Replicate · FFmpeg · TTS
OPS           Docker / Podman · WSL2 · git-bash · PowerShell · pnpm / bun / uv
              n8n-class automation · cron · observability dashboards
```

---

## How I work

```
READ BEFORE WRITE       never guess — read the source, then edit
MINIMAL DIFF            smallest change that solves the real problem
VERIFY AFTER CHANGE     test / lint / smoke / sanity — no exceptions
EXPLICIT OVER MAGIC     readable code beats clever code
PRODUCTION OVER EGO     "works now" wins unless it is flagged as an infra bet
NO SECRETS IN OUTPUT    keys, tokens, PATs — never in a repo, never in a log
SAY THE DOWNSIDE        name future tech debt out loud, immediately
```

Interface doctrine: background `#090b10`, radius `0px`, JetBrains Mono, technical
icons only, **no emoji**.

---

## Current edge

- Agent memory that is agent-agnostic — one shared palace, many runtimes
- GEO/AEO as a first-class deliverable, with freshness signals and schema
- Production retail agents measured by margin, not by demos
- Generative media at queue scale — image, video and voice in one system
- Edge-native AI: inference and routing close to the customer

---

<div align="center">

### Contribution activity

![snake](https://raw.githubusercontent.com/Bonzokoles/Bonzokoles/output/github-snake.gif)

![stats](https://github-readme-stats.vercel.app/api?username=Bonzokoles&show_icons=true&theme=github_dark&bg_color=0a0e14&text_color=c9d1d9&title_color=7cf3c6&icon_color=7cf3c6&hide_border=true&hide=stars,contribs)

![languages](https://github-readme-stats.vercel.app/api/top-langs/?username=Bonzokoles&layout=compact&theme=github_dark&bg_color=0a0e14&text_color=c9d1d9&title_color=7cf3c6&hide_border=true)

</div>

---

## Contact

```
STUDIO      https://yutro.company
AI PLATFORM https://ai.yutro.company
BLOG / GEO  https://www.mybonzoaiblog.com
AGENT CLUB  https://jimbo77.org
GITHUB      https://github.com/Bonzokoles

YUTRO       doyutro@yahoo.com
BLOG / PUMO stolarnia.ams@gmail.com
```

---

<div align="center">

```
FEAR CAUSES HESITATION. HESITATION MAKES YOUR WORST FEARS REAL.

BUILD WHAT TERRIFIES YOU.
```

</div>
