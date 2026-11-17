### Hi, I'm Daniel 👋

Developer at **Input Consulting**. Most of what I build lives in private repos — client work, products and hobby projects — so here's what's behind the contribution graph.

---

### 🏢 Products & client work

**Kvarto** — [kvarto.se](https://kvarto.se)  
A full-stack platform for commercial leases and property portfolios: contracts, facility planning, budgets, space planning, inventory, internal rent and projects. AI-assisted extraction of lease data from PDFs.  
`React 19` `TypeScript` `MUI` `Vite` `NestJS` `TypeORM` `PostgreSQL` `Azure`

**Sales & financing platform (consulting)**  
The tools retailers use to sell and finance products: quotes, loans and leasing, insurance, service agreements in one flow, plus a wholesale portal for financing retailers' stock. Built for a large finance company.  
`React` `TypeScript` `TanStack Query` `Tailwind` `Vitest` `Azure Pipelines` `Helm`

---

### 🛠️ Side projects

**Sidlinjen** — team app for a kids' football team  
A mobile-first PWA for parents and coaches. It doesn't replace the club's tools or the group chat; it surfaces the posts that otherwise drown in it. Per-team permissions, push notifications, Swedish/English, built to run on free tiers.  
`Next.js 16` `Tailwind` `shadcn/ui` `Neon Postgres` `Drizzle` `Clerk` `Web Push`

**FallenShard** — co-op hero defense game  
A 3D hero defense game with a Defense → Intermission → Exploration loop. Online co-op for 2 players today, 2v2 as the goal. Stylized hand-painted look.  
`Unity 6` `C#` `URP` `Netcode for GameObjects` `Unity Relay`

**Borgen** — cozy idle city builder in the browser  
Build a town, make decisions in the throne room, send parties into dungeons — and never lose. The simulation is pure TypeScript so it can move to a server later.  
`three.js` `TypeScript` `Vite` `Vitest`

**AgentBoard** — a floating panel for AI coding sessions  
A native macOS panel, skinned like Mac OS 9, that shows every running Claude Code session: status, remaining context, weekly quota and today's tasks. Reads local state only, so it costs zero tokens.  
`Swift 6` `SwiftUI` `EventKit`

---

### 🧠 Second brain — my AI development setup

Most of my day runs through Claude Code, so I've built a personal system around it that remembers, routes work to the right model and guards against expensive mistakes.

- **Memory with hybrid retrieval** — curated Markdown notes (in Obsidian) plus nightly digests of every session. A hook injects the most relevant notes into each prompt using lexical + semantic search, with embeddings from a local Qwen3 model.
- **Nightly consolidation** — a scheduled job distills the day's sessions into episodic notes and proposes what should become long-term memory. I approve it.
- **Model routing** — cheap models search and read, a strong model plans and judges, and code is written and reviewed by dedicated agents (planner → coder → reviewer).
- **Guardrails as hooks** — read-only cloud CLI unless explicitly armed, a search budget per agent, a gate on multi-agent swarms, and protection against accidental merges.
- **PR babysitter** — a night job that sweeps open pull requests, checks scope and reviews new commits before the team wakes up.
- **`wt`** — one-command git worktrees with env files, dependencies and port slots, so several agents can work in parallel without touching my main checkout.
