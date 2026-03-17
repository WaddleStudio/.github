# Waddle Studio 🐧

Small steps, steady shipping. Building commercially-focused software products for the Taiwan market.

API-first architecture · Deterministic over probabilistic · Ship specs before code

---

## Products

**💳 CardSense** — Deterministic credit card recommendation API for Taiwan. Rule-based engine with auditable decisions. No LLM in the request path.
`cardsense-contracts` · `cardsense-extractor` · `cardsense-api`

**⭐ RTA (Review Trust Analyzer)** — AI-powered credibility scoring for Google Maps reviews. Hybrid pipeline: rules + embeddings + LLM reasoning.
`review-trust-analyzer`

**🌱 SEEDCRAFT 種子工藝** — AI family education platform on LINE. Original IP with six natural elements growth system.
`seedcraft`

**📰 TechTrend Briefing** — B2B tech intelligence newsletter for engineering leaders. NotebookLM-powered content pipeline.
`techtrend`

**🎲 SmartChoice** — AI-assisted daily decision helper (what to eat, where to go). Integrates with RTA and CardSense.
`smartchoice`

**🧊 FridgeManager** — Household ingredient management with expiry alerts and AI recipe suggestions.
`fridgemanager`

**🔗 Knoty** — Privacy-first social relationship graph tool for university students.
`knoty`

---

## Infrastructure

| Repo | Purpose |
|------|---------|
| `fleet-command` | Spec library — all project specifications, architecture docs, and knowledge base sources |
| `fleetbot` | Discord bot for fleet-command operations (deployed on Railway) |

Agent orchestration (OpenClaw) is an architectural concept spanning FleetBot + Notion cron jobs + MCP integrations, not a standalone repo.

---

## Tech Stack

**Languages:** TypeScript · Python · Java 21
**Frameworks:** Next.js · FastAPI · Spring Boot 4 · LINE Bot SDK
**Data:** PostgreSQL (Supabase) · pgvector · Drizzle / SQLAlchemy / Spring Data JPA
**AI/ML:** Claude · Gemini · Ollama + Qwen · Cohere Embed
**Deploy:** Vercel · Railway
**Automation:** n8n · Discord bots · NotebookLM

---

## Cross-Product Integration

```
SmartChoice → CardSense    Restaurant pick → best payment card
SmartChoice → RTA          Location pick → review trust verification
FridgeManager → CardSense  Grocery list → best supermarket card
SEEDCRAFT → RTA            Cram school → parent review credibility
```

---

*All projects target commercialization. Specs live in `fleet-command` — code follows spec.*
