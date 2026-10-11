<div align="center">

# Ritunjay Deo

### I build AI-powered products with real engineering underneath: private, tested, correct by design.

Full-Stack · Android · Applied AI &nbsp;|&nbsp; MBA Tech (Computer Engineering), NMIMS MPSTME, Mumbai

[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:ritunjay1201@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ritunjaydeo)

</div>

---

## At a glance

> **Hackathon Honors:** Adobe University Hackathon 2026 (Round 4 of 5, Top 45 of 100,000+ teams) · TechForge 2026 Hackathon

| 4 shipped projects | 1,270+ tests & verification checks | 0 video frames leave device |
|:---:|:---:|:---:|
| Web · Android · Agentic | Skillo 417 · BedLink 464 · Audit 335 · MADVerse 60 | Client-side Web Workers + ONNX Runtime Web |

---

## Featured projects

### 🤖 [Skillo AI](https://github.com/sylbornfurtado19/Skillo): technical interview simulator that grades what you say *and* how you present it
*Collaborative build (Lead Vision & Evaluation Engineering).*

`Next.js 16` `TypeScript` `Supabase` `Zod` `Jest` `Playwright` `Web Workers` `ONNX Runtime Web`

- **10 Core Research Engines:** 5 AI reasoning & memory engines (Prometheus-2 rubric & SUQ grader, LATS/MCTS adaptive interviewer, GraphRAG skill-gap mapping, Reflexion memory coach, SimPO FAANG comparator) + 5 vision, audio & document engines (LayoutLMv3 document AI, L2CS-Net gaze, HopeNet head pose, AffectNet composure, SyncNet AV sync)
- **Private by default:** zero-copy frame processing via transferable `ImageBitmap` in dedicated Web Workers with OffscreenCanvas and ONNX Runtime Web; 0 raw video frames or audio recordings leave the device (only extracted numerical telemetry and text answers are sent for scoring)
- **Test coverage:** 417 automated tests passing across 54 test suites

### 🔍 [Brand AI-Readiness Audit](https://github.com/AkkiSensei/brand-ai-readiness-audit): agent skill that audits web properties for AI discoverability
*Evaluates brand URLs against what AI search engines and crawler agents can ingest.* · **Adobe University Hackathon 2026: Round 4 of 5, top 45 of 100,000+ teams**

`Python` `Schema.org` `JSON Schema` `agentskills.io` `pytest`

- **30 deterministic defect checks** spanning 4 finding families: 8 CR (Crawler & Rendering: CR-001..CR-008), 8 ER (Extraction & Content: ER-001..ER-008), 8 SF (Schema & Format: SF-001..SF-008), and 6 TC (Technical & Connectivity: TC-001..TC-006); no LLM calls in the audit path, fully reproducible output
- **SSRF-hardened fetching:** DNS pinning, private-IP CIDR blocklist, and DNS rebinding protection with a strict 240 s bounded runtime budget
- **Rigorous validation:** 335 automated pytest tests passing; validated against 10 of 11 site archetypes (SPAs, e-commerce, paywalls, hydration, bot challenges) and 4 adversarial chaos scenarios (zero-byte bodies, garbage DOMs, redirect loops, hostile TCP blackholes)

### 🎬 [MADVerse](https://github.com/AkkiSensei/Mobile-Application-Development-Project): Android movie discovery with explainable recommendations
`Kotlin` `Jetpack Compose` `Material 3` `Hilt` `Room` `Retrofit` `Gemini` `TMDB`

- **Transparent recommendation scoring:** deterministic 100-point match engine evaluating genre (30), mood (20), era (15), quality (15), language (10), and runtime (10), paired with contextual Gemini explanations and local Room database caching
- **Modern Android architecture:** Clean Architecture + MVVM, Kotlin Coroutines, StateFlow, strict unidirectional data flow, and offline-first persistence
- **Test coverage:** 60 automated unit tests covering domain models, view models, and recommendation logic with 100% pass rate

### 🏥 [BedLink](https://github.com/AkkiSensei/T17-BedLink): real-time hospital bed coordination for emergency response
*Prevents ER diversion, phone-tag delays, and bed double-booking during critical transit.* · **TechForge 2026 Hackathon** · [Live Demo](https://bedlink-one.vercel.app)

`Next.js 15` `TypeScript` `Supabase Realtime` `PostgreSQL` `Vitest` `PGlite` `Vercel`

- **Double-booking impossible by design:** atomic bed reservations guaranteed by partial unique indexes at the PostgreSQL database layer
- **Deterministic emergency dispatch:** multi-factor hospital ranking based on Haversine travel time, bed telemetry freshness, and facility load penalty
- **Time-bound coordination:** 120-second authoritative hold countdown, role-scoped WebSocket channels, and automated cascading fallback upon expiration
- **Field-ready mobile craft:** automatic Lite Mode for low-spec hardware (RAM <= 2GB, CPU <= 4 cores, or Save-Data connections), haptics (`navigator.vibrate`), and Screen Wake Lock · 464 verification checks passing across 11 verification suites

### Also built
- **[MedFlow](https://github.com/AkkiSensei/medflow):** hospital management backend in Java 17, Spring Boot, Spring Data JPA, Flyway, and H2.
- **[Forge & Co](https://github.com/AkkiSensei/Forge-Co):** responsive D2C e-commerce storefront in React, TypeScript, Vite, and Tailwind CSS.

---

## Toolbox

| | |
|---|---|
| **Languages** | Kotlin · TypeScript · Python · JavaScript · Java |
| **Web** | Next.js · React · Vite · Tailwind CSS |
| **Android** | Jetpack Compose · Hilt · Room · Retrofit · Material 3 |
| **Data** | PostgreSQL · Supabase (Auth, Realtime) · SQLite |
| **AI** | Gemini · Claude · OpenAI · Agentic Workflows · RAG · MCTS |
| **Quality & DevOps** | Vitest · Jest · Playwright · pytest · Gradle · Git · Vercel |

---

## What I care about

- **Private by default AI:** Run inference on the client whenever hardware and model architecture allow it.
- **Correctness at the lowest layer:** Eliminate race conditions with database constraints and transactions, not application-level retries.
- **Research to production:** Translate academic papers into tested, gracefully degrading, production-ready software.

---

<div align="center">

[![GitHub Stats](https://github-readme-stats.vercel.app/api?username=AkkiSensei&show_icons=true&theme=tokyonight&hide_border=true&count_private=true)](https://github.com/AkkiSensei)
[![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=AkkiSensei&layout=compact&theme=tokyonight&hide_border=true&langs_count=6)](https://github.com/AkkiSensei)

[![Streak](https://streak-stats.demolab.com?user=AkkiSensei&theme=tokyonight&hide_border=true)](https://github.com/AkkiSensei)

</div>
