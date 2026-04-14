<div align="center">

# Hi, I'm Kaden 👋

### ML Engineer | BCI &amp; Real-Time Systems

<a href="https://vhtech.me"><img src="https://readme-typing-svg.demolab.com/?font=JetBrains+Mono&weight=500&size=20&duration=3200&pause=900&color=38BDF8&center=true&vCenter=true&multiline=false&width=720&height=44&lines=Not%20a%20CS%20degree.%20Credentials%20to%20match.;Production%20AI%20systems%20that%20run%20daily.;BCI%20%2B%20real-time%20systems%20focus.;Targeting%20Neuralink." alt="tagline" /></a>

</div>

---

> I build production AI systems that automate expert workflows. Not demos, not prototypes. Systems that run daily under real operational constraints.

## 🧰 Tech Stack

![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white) ![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white) ![React](https://img.shields.io/badge/-React-61DAFB?style=flat-square&logo=react&logoColor=white) ![Node.js](https://img.shields.io/badge/-Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white) ![Express](https://img.shields.io/badge/-Express-000000?style=flat-square&logo=express&logoColor=white) ![FastAPI](https://img.shields.io/badge/-FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white) ![PyTorch](https://img.shields.io/badge/-PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white) ![Docker](https://img.shields.io/badge/-Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![n8n](https://img.shields.io/badge/-n8n-EA4B71?style=flat-square&logo=n8n&logoColor=white) ![SQLite](https://img.shields.io/badge/-SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/-PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![Supabase](https://img.shields.io/badge/-Supabase-3FCF8E?style=flat-square&logo=supabase&logoColor=white) ![Tailscale](https://img.shields.io/badge/-Tailscale-242424?style=flat-square&logo=tailscale&logoColor=white) ![Vite](https://img.shields.io/badge/-Vite-646CFF?style=flat-square&logo=vite&logoColor=white)

*Also:* C#, C/C++, SQL, .NET / COM Interop, YOLO, ChromaDB, Git / GitHub, SOLIDWORKS, Computer Vision, Automation, CAD / Mechanical Engineering

## 🚀 Featured Projects

### CloudBooks

> 25-table multi-tenant Supabase SaaS with RLS, Stripe feature-gated billing, BYOK AI insights, and QuickBooks Online OAuth2 sync. Live on Cloudflare Pages.

Multi-tenant task tracking and business management SaaS for informal employers: property owners, parents, and anyone running real work without a formal business entity. React 18 + TypeScript + Tailwind on Vite 6, backed by Supabase Cloud with RLS on 25 tables, Realtime subscriptions, and 9 Edge Functions. 21 domain service modules, pgcrypto-encrypted AI keys and OAuth tokens, Stripe subscription billing gated at the database via the check_feature_limit RPC, and QuickBooks Online OAuth2 with bidirectional sync. 288 unit and 61 Playwright E2E tests, GitHub Actions CI/CD, PWA installable, deployed to Cloudflare Pages.

**Stack:** React 18, TypeScript, Tailwind CSS, Vite, Zustand, TanStack Query, React Router v6, Supabase Auth · PostgreSQL, Vitest, Playwright, pg_cron

🌐 [cb.vhtech.me](https://cb.vhtech.me)

### McQueenyML

> Production HVAC estimating platform running daily on McQueeny Group's Windows servers. 5 manufacturer parsers, 195 scope templates, 419 tracked projects, Ollama lifecycle analyzer, real-time R:\ drive watcher.

Parses manufacturer pricing sheets (Armstrong XML, WaterFurnace, Condair, Marlo, Johnson Controls PDFs) into formatted Excel workbooks, matches line items against 195 product scope templates through a deterministic-first pipeline (pattern, fuzzy, pgvector embedding, then AI fallback), and generates MGI or JCI Word scope documents. React 18 + TypeScript frontend, Python 3.11 + FastAPI backend, PostgreSQL via Supabase with pg_trgm and pgvector, and Ollama Qwen3 14B for project lifecycle analysis. A real-time R:\ drive filesystem watcher correlates events to 419 SharePoint-synced projects, 3063 PSR equipment orders, and a 394K-row network drive file index. 7 NSSM Windows services run the stack in production, fronted by Cloudflare Tunnel with LAN-routing bypass for uploads over 100MB. ~111 API endpoints across 21 routers, 223 pytest and 55 vitest tests.

**Stack:** Frontend: React · TypeScript · Vite · Tailwind CSS. Backend: Python 3.11 · FastAPI · uvicorn. Database: PostgreSQL via Supabase (pg_trgm · pgvector). ML: Ollama (qwen3:14b, nomic-embed-text). Infrastructure: 7 NSSM services on Windows 11, Cloudflare Tunnel.

### Adze — AI for SOLIDWORKS

> Native in-process AI assistant for SOLIDWORKS with 19 typed grounding tools and governed write safety

AI design assistant that runs inside SOLIDWORKS as a COM add-in, not alongside it. 19 typed grounding tools read live CAD sessions (dimensions, mates, mass properties, BOM). 8-step governed safety lifecycle for write operations ensures AI modifications are reversible and auditable. Built in C# on .NET with the SOLIDWORKS API. SOLIDWORKS Solution Partner Program application in progress.

**Stack:** C# .NET 4.8, SOLIDWORKS COM API, NUnit 3, MSBuild, PowerShell, WinForms WebBrowser

🌐 [github.com/kadenvh/adze-cad](https://github.com/kadenvh/adze-cad) &nbsp;·&nbsp; 💻 [adze-cad](https://github.com/adze-cad)

### Oracle (Trade Signal)

> Learned its own BUY signals are anti-predictive and inverted them into a 62.8% win rate contrarian short engine: 5 cortexes, 2,987 predictions, $499K paper portfolio

Self-directed market analysis system that generates testable hypotheses, backtests them against historical data, and manages a $499K paper portfolio behind 8 risk gates. Five cortexes (LSTM, FinBERT sentiment, Perplexity LLM deep analysis, rules-based momentum, and a local indicator ensemble) feed an adaptive-weight Oracle brain that reweights across 12 market regimes. The distinctive finding, surfaced by 2,987 logged predictions with outcome tracking, is that the system's own BUY signals are anti-predictive for going long at 27% accuracy but produce a 62.8% win rate as contrarian shorts with 2:1 W/L ratio. A multi-venue adapter layer (Alpaca equities wired live, plus verified fee models for Coinbase, Polymarket, and Kalshi) routes signals to whichever venue fits. Python 3.13, FastAPI, SQLite WAL, systemd daemons, Sentry observability, 506 tests across 22 files.

**Stack:** Python 3.13 (miniconda3), FastAPI, SQLite, TensorFlow, PyTorch, transformers (FinBERT), React/TypeScript/Tailwind (ava_hub UI)

## 📊 Stats

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=Kadenvh&theme=tokyonight&hide_border=true&include_all_commits=true&count_private=true&show_icons=true" height="165" alt="stats" />
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Kadenvh&theme=tokyonight&hide_border=true&layout=compact&langs_count=8" height="165" alt="top-langs" />

<img src="https://streak-stats.demolab.com/?user=Kadenvh&theme=tokyonight&hide_border=true" height="165" alt="streak" />

</div>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=Kadenvh&theme=tokyo-night&hide_border=true&area=true" width="100%" alt="activity" />

## 🔭 Currently Building

- SPDRbot closed-loop gait controller.
- OpenBCI EEG pipeline.
- Adze public repo + case study (portfolio piece, SOLIDWORKS partnership).

## 📫 Contact

- 🌐 **Portfolio** · [vhtech.me](https://vhtech.me)
- ✉️ **Email** · [contact@vhtech.me](mailto:contact@vhtech.me)
- 💼 **LinkedIn** · [linkedin.com/in/kadenvh](https://linkedin.com/in/kadenvh)
- 📍 **Based in** · Kansas, United States

---
<div align="center"><sub>Generated from <a href="https://vhtech.me">vhtech.me</a> · Last updated 2026-04-14</sub></div>
