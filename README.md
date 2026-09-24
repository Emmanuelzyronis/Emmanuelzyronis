<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=CC3024&height=200&section=header&text=Emmanuel%20Ibiezugbe&fontSize=42&fontColor=ffffff&fontAlignY=38&desc=Independent%20Engineer%20%C2%B7%20Correctness%20First&descAlignY=58&descSize=16&descColor=ffffff99&animation=fadeIn" width="100%"/>

<br/>

<a href="https://emmanuelibiezugbe.com"><img src="https://img.shields.io/badge/Portfolio-emmanuelibiezugbe.com-CC3024?style=for-the-badge&logo=vercel&logoColor=white&labelColor=0a0a0a" /></a>
&nbsp;
<a href="mailto:ibiezugbeemmanuel@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white&labelColor=0a0a0a" /></a>

<br/><br/>

![Typing SVG](https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=15&pause=1000&color=CC3024&center=true&vCenter=true&width=650&lines=I+build+software+you+can+audit%2C+explain%2C+and+trust.;Financial+systems+%C2%B7+Real-time+pipelines+%C2%B7+AI+tooling;Correctness+is+an+engineering+property%2C+not+a+quality.)

</div>

<br/>

---

## ◈ &nbsp;About

> *I take on work where correctness matters — where a wrong answer has real consequences and a right answer requires careful engineering.*

I'm an independent engineer working across product, systems, automation, and AI. Most of what I build is at the intersection of complexity and constraint: financial systems that need to be auditable, pipelines that need to be fast and correct, automations that need to work reliably without supervision.

Available for focused, **[project-based work](mailto:ibiezugbeemmanuel@gmail.com)**. I reply within one business day.

<br/>

---

## ◈ &nbsp;How I Work

| | |
|---|---|
| **Start from the constraint** | Before choosing tools or architecture, I want to understand what correctness means for the problem — what the failure modes are, how they would be detected, and what the cost of getting it wrong is. |
| **Evidence over assertion** | I measure what I claim. If a change is supposed to make something faster, I benchmark it. If a system is supposed to handle edge cases, I write tests that hit them. Claims without evidence are not engineering. |
| **Simplicity is a feature** | Complex systems fail in complex ways. I prefer the simpler solution that can be understood, audited, and debugged over the clever one that requires remembering how it works. |
| **Write it down** | Good decisions lose value if they can't be explained. I document architecture, tradeoffs, and reasoning — not because it's required, but because it's part of the work. |

<br/>

---

## ◈ &nbsp;Selected Work

<br/>

**◈ &nbsp;[LEDGER](https://github.com/Emmanuelzyronis/Ledger)** &nbsp;—&nbsp; *Deterministic Transaction Reconciliation Engine*

Production reconciliation engine. Ingests two independent financial record sets, classifies every record pair across seven exhaustive outcomes (MATCHED / MISMATCHED / AMBIGUOUS / UNMATCHED / DUPLICATE / INVALID), and produces an immutable, auditable decision for each — deterministically. Append-only audit log in-transaction with every state write. Generated TypeScript client from OpenAPI 3.1 — the frontend cannot call an endpoint that does not exist.

`254 tests` &nbsp;·&nbsp; `42/42 product proof checks` &nbsp;·&nbsp; `0 security findings` &nbsp;·&nbsp; `95.5 rec/s` &nbsp;·&nbsp; `p95 11 ms` &nbsp;·&nbsp; `RPO ≤ 15 min · RTO ≤ 30 min` &nbsp;·&nbsp; `v1.0.0 · 2026-09-19`

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![OpenAPI](https://img.shields.io/badge/OpenAPI_3.1-6BA539?style=flat-square&logo=openapiinitiative&logoColor=white)

<br/>

**◈ &nbsp;[FreshIndex](https://github.com/Emmanuelzyronis/FreshIndex)** &nbsp;—&nbsp; *PostgreSQL CDC Pipeline with a p99 Staleness Guarantee*

WAL-based change-data-capture pipeline: PostgreSQL logical replication → Redis Streams → Meilisearch, with an independent staleness monitor that measures commit-to-search visibility from the outside — sharing no code or infrastructure with the indexer. p99 of 221 ms against a 1,000 ms target. 4.5× inside the objective. 300 mutations. Zero violations. Zero dead-letter messages.

`p50 151 ms` &nbsp;·&nbsp; `p95 207 ms` &nbsp;·&nbsp; `p99 221 ms / 1,000 ms target` &nbsp;·&nbsp; `300 mutations · 0 violations` &nbsp;·&nbsp; `0 dead-letter messages`

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis_Streams-FF4438?style=flat-square&logo=redis&logoColor=white)
![Meilisearch](https://img.shields.io/badge/Meilisearch-FF5CAA?style=flat-square&logo=meilisearch&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

<br/>

**◈ &nbsp;MailFlow AI** &nbsp;—&nbsp; *Human-supervised AI Email Operations* &nbsp;`private`

Six-stage pipeline (receive → triage → draft → evaluate → approve → send). Structured output slots — the model fills defined fields rather than composing freely, which makes the evaluate step tractable. An adversarial self-review prompt before any human sees the draft. A required approve gate enforced structurally in code — there is no pathway that sends an email before reaching the approved state. Full audit trail per email including all model outputs and the approval decision.

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![Azure OpenAI](https://img.shields.io/badge/Azure_OpenAI-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)
![Google Gemini](https://img.shields.io/badge/Google_Gemini-8E75B2?style=flat-square&logo=googlegemini&logoColor=white)
![ChromaDB](https://img.shields.io/badge/ChromaDB-FF6B35?style=flat-square&logoColor=white)
![Gmail API](https://img.shields.io/badge/Gmail_API-EA4335?style=flat-square&logo=gmail&logoColor=white)

<br/>

**◈ &nbsp;[ArkZen](https://github.com/Emmanuelzyronis/Arkzen)** &nbsp;—&nbsp; *AI-assisted Lead Acquisition Workbench*

Nine-stage pipeline (DISCOVER → FILTER → SCORE → RESEARCH → QUALIFY → STRATEGIZE → ENGAGE → CLOSE → OUTCOME). Explainable 0–100 score built from named checks — Fit, Intent, Urgency, Reachability — each resolved as pass / warn / **unknown**. Unknown is a first-class outcome, never collapsed into false confidence. Human in control of every engagement decision. Deterministic fallback if the model is unavailable; interface is identical either way.

`126 Vitest tests · 12 files` &nbsp;·&nbsp; `dual SQLite / Postgres backend` &nbsp;·&nbsp; `browser verification gate (1440px + 390px · both themes)`

![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Azure OpenAI](https://img.shields.io/badge/Azure_OpenAI-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)
![Tailwind 4](https://img.shields.io/badge/Tailwind_4-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)

<br/>

**◈ &nbsp;[ArkOne](https://github.com/Emmanuelzyronis/ArkOne)** &nbsp;—&nbsp; *AI-Native CRM* &nbsp;[↗ live](https://arkone-ten.vercel.app)

Sales CRM where the AI copilot is grounded in live deal data before every response — so "what should I focus on this week?" gets a real answer, not a guess. Kanban pipeline with optimistic drag-and-drop. CSV import with column auto-mapping. One-click demo seed (15 realistic deals, 6 companies, $947K pipeline, 67% win rate). Org-scoped auth via Clerk; Supabase RLS enforces team-level data isolation at the database layer.

![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=white)
![Clerk](https://img.shields.io/badge/Clerk-6C47FF?style=flat-square&logo=clerk&logoColor=white)
![Azure OpenAI](https://img.shields.io/badge/Azure_OpenAI-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)

<br/>

**◈ &nbsp;[CollabCanvas](https://github.com/Emmanuelzyronis/CollabCanvas)** &nbsp;—&nbsp; *Human × Agent Shared Canvas*

Real-time collaborative canvas where a human and an AI agent (Aria) edit the same live board through WebMCP. Symmetric architecture: human and agent use identical Zustand store actions; only the author field (`'human'` | `'agent'`) differs. 33 WebMCP tools on `document.modelContext`. 15-layer Design Graph backed by PostgreSQL. Built for the OpenAI WebMCP Challenge.

`197 Vitest tests` &nbsp;·&nbsp; `33 WebMCP tools` &nbsp;·&nbsp; `15-layer Design Graph`

![React 18](https://img.shields.io/badge/React_18-61DAFB?style=flat-square&logo=react&logoColor=black)
![Vite 8](https://img.shields.io/badge/Vite_8-646CFF?style=flat-square&logo=vite&logoColor=white)
![Zustand](https://img.shields.io/badge/Zustand-433E38?style=flat-square&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![WebMCP](https://img.shields.io/badge/WebMCP-000000?style=flat-square&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)

<br/>

---

## ◈ &nbsp;Open Source

Patches submitted upstream to libraries I run in production. All CI green, awaiting maintainer review. Each was mutation-tested before submission — reverting only the changed file makes the new test fail.

<br/>

**🧙 &nbsp;tRPC** &nbsp;—&nbsp; *End-to-end typesafe APIs*

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)

- **[#7608](https://github.com/trpc/trpc/pull/7608)** &nbsp;*(feat)* — Adds `broadcastReconnectNotification` to the Fastify adapter, so a Fastify server can ask every connected client to reconnect before it shuts down. Previously the hook only existed on the standalone WebSocket adapter.
- **[#7609](https://github.com/trpc/trpc/pull/7609)** &nbsp;*(fix)* — Fixes a silent session-loss bug in the official WebSockets + Prisma starter: server-side code was calling the *client*-side `getSession` helper, which makes an internal HTTP round-trip per request and drops the session when it fails.

<br/>

**🔍 &nbsp;Meilisearch** &nbsp;—&nbsp; *Search engine client*

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)

- **[#2241](https://github.com/meilisearch/meilisearch-js/pull/2241)** &nbsp;*(fix)* — `deleteIndexIfExists()` reported success for indexes that never existed, and returned before the deletion task had been processed. Filed [#2240](https://github.com/meilisearch/meilisearch-js/issues/2240) to document the investigation before submitting the PR. 1,670 existing tests still passing.

<br/>

**🧩 &nbsp;Payload CMS** &nbsp;—&nbsp; *Next.js CMS*

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)

- **[#18248](https://github.com/payloadcms/payload/pull/18248)** &nbsp;*(fix)* — A nested Local API call that passed its own `req` with a different `locale` leaked that locale onto the caller's request, so `beforeChange` merged values into the wrong locale. Fixes the data-corruption path from [#18246](https://github.com/payloadcms/payload/issues/18246). 9/9 CI checks green.

<br/>

---

## ◈ &nbsp;Tech Stack

<div align="center">

**Languages**

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)

<br/>

**Frontend**

![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)
![Zustand](https://img.shields.io/badge/Zustand-433E38?style=flat-square&logoColor=white)
![Framer Motion](https://img.shields.io/badge/Framer_Motion-0055FF?style=flat-square&logo=framer&logoColor=white)
![Radix UI](https://img.shields.io/badge/Radix_UI-161618?style=flat-square&logo=radixui&logoColor=white)
![Recharts](https://img.shields.io/badge/Recharts-22b5bf?style=flat-square&logoColor=white)
![TanStack Query](https://img.shields.io/badge/TanStack_Query-FF4154?style=flat-square&logo=reactquery&logoColor=white)

<br/>

**Backend & Infrastructure**

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![Redis](https://img.shields.io/badge/Redis_Streams-FF4438?style=flat-square&logo=redis&logoColor=white)
![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-D71F00?style=flat-square&logo=sqlalchemy&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=white)
![Clerk](https://img.shields.io/badge/Clerk-6C47FF?style=flat-square&logo=clerk&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white)

<br/>

**AI & Search**

![Azure OpenAI](https://img.shields.io/badge/Azure_OpenAI-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)
![Google Gemini](https://img.shields.io/badge/Google_Gemini-8E75B2?style=flat-square&logo=googlegemini&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![ChromaDB](https://img.shields.io/badge/ChromaDB-FF6B35?style=flat-square&logoColor=white)
![Meilisearch](https://img.shields.io/badge/Meilisearch-FF5CAA?style=flat-square&logo=meilisearch&logoColor=white)
![WebMCP](https://img.shields.io/badge/WebMCP-000000?style=flat-square&logoColor=white)

</div>

<br/>

---

## ◈ &nbsp;GitHub Stats

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=Emmanuelzyronis&show_icons=true&theme=transparent&title_color=CC3024&icon_color=CC3024&text_color=ffffff&border_color=CC302430&include_all_commits=true&count_private=true" height="165"/>

<br/><br/>

<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Emmanuelzyronis&layout=compact&theme=transparent&title_color=CC3024&text_color=ffffff&border_color=CC302430&langs_count=6" height="140"/>

</div>

<br/>

---

<div align="center">

**Independent Engineer**

*Available for focused, project-based work. I reply within one business day.*

<br/>

<a href="mailto:ibiezugbeemmanuel@gmail.com">
  <img src="https://img.shields.io/badge/→%20ibiezugbeemmanuel%40gmail.com-CC3024?style=for-the-badge&logoColor=white&labelColor=0a0a0a&color=CC3024" />
</a>

<br/><br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=CC3024&height=120&section=footer&animation=fadeIn" width="100%"/>

</div>
