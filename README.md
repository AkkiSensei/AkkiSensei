<div align="center">

# Ritunjay Deo

### I build private AI products and race-free systems where failure has consequences.

Full-Stack · Android · Applied AI &nbsp;|&nbsp; MBA Tech (Computer Engineering), NMIMS MPSTME, Mumbai

[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:ritunjay1201@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ritunjaydeo)

</div>

I am an MBA Tech Computer Engineering student at NMIMS MPSTME, Mumbai. I engineer software for domains where failure carries real operational stakes, from emergency clinical triage and hospital bed dispatch to privacy-preserving computer vision. My work is backed by 1,630+ verified tests and checks, and placed in the top 45 of 100,000+ teams in the Adobe University Hackathon 2026.

---

## At a glance

> **Hackathon Recognition:** Adobe University Hackathon 2026 (Round 4 of 5, Top 45 of 100,000+ teams) · TechForge 2026 Hackathon

| 5 shipped systems | 1,630+ tests and checks | 0 video frames leave your device |
|:---:|:---:|:---:|
| Full-stack web, Android, and agentic tools | Verified across runners: Skillo 417, TriageRAG 358, Audit 335, MADVerse 60, BedLink 464 | In-browser CV via Web Workers and ONNX Runtime |

---

## Featured projects

### 🤖 [Skillo AI](https://github.com/sylbornfurtado19/Skillo): An interview simulator that reads composure without your face reaching a server
*Team project with Sylborn Furtado and Yug Dhaigude.*

`Next.js 16` `TypeScript` `Supabase` `Zod` `Jest` `Playwright` `Web Workers` `ONNX Runtime Web`

- **The problem:** Technical interview platforms stream webcam video and microphone audio to remote servers, creating latency and biometric privacy risks.
- **What was built:** Zero-copy in-browser computer vision. The client transfers raw video frames as transferable `ImageBitmap` objects directly to dedicated Web Workers, executing MediaPipe landmark extraction and ONNX Runtime Web off the main thread with zero frame-dropping jank and zero raw video uploads.
- **Proof:** 417 automated tests passing across 54 test suites.

<details>
<summary>How it works</summary>

- 10 Core Research Engines: 5 reasoning and memory engines (Prometheus-2 rubric grader with semantic uncertainty quantification, LATS/MCTS adaptive branching interviewer, GraphRAG skill-gap mapping, Reflexion memory coach, SimPO FAANG comparator) and 5 vision, audio, and document engines (LayoutLMv3 document AI, L2CS-Net 3D gaze, HopeNet head pose, AffectNet composure, SyncNet audio-visual lip sync).
- All facial landmarks, head pose angles, gaze vectors, and audio energy metrics are calculated locally on the client machine; only computed numeric telemetry and text transcripts are sent for scoring.
</details>

### 🩺 [TriageRAG](https://github.com/AkkiSensei/TriageRAG): Emergency triage decision support that never lets a language model make safety-critical decisions
*Research prototype for clinical decision support.*

`Python 3.11` `FastAPI` `React 18` `Vite` `TypeScript` `Pydantic` `BM25` `pytest`

- **The problem:** Language models in clinical workflows can hallucinate lethal drug doses, overlook contraindications, or invent protocol steps when evaluating emergency patients.
- **What I built:** A two-pass deterministic safety architecture. Dose calculations run on exact Decimal arithmetic with 10x magnitude tripwires, contraindication interlocks enforce an inviolable BLOCK with zero override code paths, and retrieved clinical protocol chunks require verbatim substring citations before any drafted step reaches a clinician.
- **Proof:** 358 automated tests (322 pytest, 36 Vitest), 100% mutant kill score (52/52 code and rule mutants), and 100% pass rate across golden (65/65) and adversarial injection (19/19) suites.

<details>
<summary>How it works</summary>

- Pass 1 Deterministic Engine: Evaluates NEWS2/PEWS physiological scoring, population rules, and fatal drug-drug interactions (such as Sildenafil and Nitrates) before protocol retrieval ever runs.
- Pass 2 Machine Verification: Verifies proposed clinical orders against formulary dosage ceilings, approved administration routes, verbatim guideline chunk substrings, and prose drug leaks.
- Cryptographic Audit Trail: Records every assessment input, rule trigger, clinician override attempt, and decision verdict in an append-only, SHA-256 hash-chained audit log.
</details>

### 🔍 [Brand AI-Readiness Audit](https://github.com/AkkiSensei/brand-ai-readiness-audit): An auditor that tests whether AI search engines can read your site without calling an LLM
*Adobe University Hackathon 2026: Round 4 of 5, Top 45 of 100,000+ teams*

`Python` `Schema.org` `JSON Schema` `agentskills.io` `pytest`

- **The problem:** AI search agents (ChatGPT, Claude, Perplexity) fail on misconfigured SPAs, blocked robots.txt rules, and broken schemas, leaving brand content invisible to generative search.
- **What I built:** An automated auditor that runs without LLM hallucinations. I built an SSRF-hardened HTTP engine with DNS pinning against rebinding attacks, RFC-1918 private-IP blocklists, and deterministic DOM and schema verification within a strict 240-second execution budget.
- **Proof:** 335 automated pytest tests passing; validated across 10 of 11 site archetypes and 4 adversarial chaos scenarios.

<details>
<summary>How it works</summary>

- 30 deterministic defect checks across 4 finding families: 8 CR (Crawler and Rendering: CR-001..CR-008), 8 ER (Extraction and Content: ER-001..ER-008), 8 SF (Schema and Format: SF-001..SF-008), and 6 TC (Technical and Connectivity: TC-001..TC-006).
- Validated against 10 of 11 site archetypes (SPAs, e-commerce, paywalls, hydration, bot challenges) and 4 chaos scenarios (zero-byte bodies, garbage DOMs, redirect loops, hostile TCP blackholes).
- No LLM calls in the audit path; every finding is reproducible and grounded in schema specifications.
</details>

### 🎬 [MADVerse](https://github.com/AkkiSensei/Mobile-Application-Development-Project): Android movie discovery that explains its recommendations instead of hiding behind a black box
`Kotlin` `Jetpack Compose` `Material 3` `Hilt` `Room` `Retrofit` `Gemini` `TMDB`

- **The problem:** Most recommendation feeds lock users into opaque algorithms that cannot explain why a title was suggested or adjust when tastes change.
- **What I built:** An auditable, deterministic 100-point scoring engine (genre 30, mood 20, era 15, quality 15, language 10, runtime 10) paired with contextual Gemini explanations and local Room persistence for offline discovery.
- **Proof:** 60 automated unit tests passing across 7 suites with 100% success rate.

<details>
<summary>How it works</summary>

- Built with Clean Architecture, MVVM, Kotlin Coroutines, and StateFlow for strict unidirectional data flow.
- Deterministic stable tie-breaking on score ties (vote average -> vote count -> popularity -> movie ID).
- Operates locally on cached catalog data when the device loses network connectivity.
</details>

### 🏥 [BedLink](https://github.com/AkkiSensei/T17-BedLink): Live hospital bed coordination where two ambulances can never book the same bed
*TechForge 2026 Hackathon* · [Live Demo](https://bedlink-one.vercel.app)

`Next.js 15` `TypeScript` `Supabase Realtime` `PostgreSQL` `Vitest` `PGlite` `Vercel`

- **The problem:** ER diversion and manual phone calls waste critical transit minutes, while concurrent ambulance dispatches risk double-booking the last available bed.
- **What I built:** Database-level uniqueness over application-level retries. I enforced partial unique indexes in PostgreSQL (`WHERE status = 'held'`) so concurrent reservations physically cannot double-book a bed, coupled with a 120-second authoritative hold timer and automated fallback cascade.
- **Proof:** 464 verification checks passing across 11 verification suites; live production app verified at [bedlink-one.vercel.app](https://bedlink-one.vercel.app).

<details>
<summary>How it works</summary>

- Multi-factor dispatch ranking calculated from Haversine travel time, bed telemetry freshness, and hospital load penalties.
- Role-scoped Supabase Realtime channels isolate nurse and dispatcher updates with zero cross-tenant event bleed.
- Field-ready mobile performance: feature-detected Lite Mode for devices with RAM <= 2GB (`navigator.deviceMemory <= 2`), CPU <= 4 cores, or Save-Data modes; haptic feedback (`navigator.vibrate`); and Screen Wake Lock during active transit.
</details>

### Also built
- **[MedFlow](https://github.com/AkkiSensei/medflow):** Hospital management backend built with Java 17, Spring Boot, Spring Data JPA, Flyway, and H2.
- **[Forge & Co](https://github.com/AkkiSensei/Forge-Co):** Responsive direct-to-consumer storefront built with React, TypeScript, Vite, and Tailwind CSS.

---

## Why you might hire me

- **I verify systems before shipping:** I do not rely on manual smoke tests or happy-path assumptions. I build test suites that push domain models, race conditions, and error boundaries until they break. (1,630+ automated tests and verification checks across 5 projects, all passing 100%).
- **I engineer for real failure modes:** I solve concurrency collisions, network drops, and malicious inputs at the system layer rather than patching symptoms in production. (PostgreSQL partial unique indexes preventing bed double-booking, absolute BLOCK drug interlocks with zero override paths, DNS pinning blocking SSRF rebinding, and 4 chaos suites surviving adversarial blackholes).
- **I ship under tight deadlines:** I translate complex specifications and research concepts into working software that deploys cleanly under hackathon and sprint pressure. (Adobe University Hackathon 2026 top 45 of 100,000+ teams, TechForge 2026 Hackathon, and live BedLink deployment on Vercel).
- **I build private-by-default software:** I keep sensitive user data off third-party servers by running compute directly on client devices whenever hardware allows. (Skillo processes computer vision locally in Web Workers with zero video frames transmitted over the network).

---

## Toolbox

| | |
|---|---|
| **Languages** | Kotlin · TypeScript · Python · JavaScript · Java |
| **Web & Backend** | Next.js · React · FastAPI · Vite · Spring Boot · Tailwind CSS |
| **Android** | Jetpack Compose · Hilt · Room · Retrofit · Material 3 |
| **Data & Storage** | PostgreSQL · Supabase (Auth, Realtime) · SQLite · Room |
| **AI & Vision** | Gemini · Claude · OpenAI · MediaPipe · ONNX Runtime Web |
| **Testing & Quality** | Vitest · Jest · Playwright · pytest · Gradle · Git · Vercel |

---

## Let's connect

If you are building systems that require rigorous engineering, race-free concurrency, or private-first AI, I would love to talk. Drop me an email at [ritunjay1201@gmail.com](mailto:ritunjay1201@gmail.com) or connect on [LinkedIn](https://www.linkedin.com/in/ritunjaydeo).

---

<div align="center">

[![GitHub Stats](https://github-readme-stats.vercel.app/api?username=AkkiSensei&show_icons=true&theme=tokyonight&hide_border=true&count_private=true)](https://github.com/AkkiSensei)
[![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=AkkiSensei&layout=compact&theme=tokyonight&hide_border=true&langs_count=6)](https://github.com/AkkiSensei)

[![Streak](https://streak-stats.demolab.com?user=AkkiSensei&theme=tokyonight&hide_border=true)](https://github.com/AkkiSensei)

</div>
