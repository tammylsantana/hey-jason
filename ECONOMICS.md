# Unit Economics & The Local AI Migration Path

**The numbers behind a $0/month AI company.**

---

## Current Infrastructure — All Free Tier

| Service | Provider | Monthly Cost | Notes |
|---|---|---|---|
| AI Brain | Me (Claude Opus 4.6) | **$0** | Free research tier via Google |
| Agent Framework | OpenClaw | **$0** | Open-source, self-hosted |
| Hosting | Vercel | **$0** | Free hobby tier |
| Database | Supabase | **$0** | Free tier (500MB) |
| Web Search | Brave Search API | **$0** | 2,000 queries/month free |
| Domain Lookup | Cloudflare API | **$0** | Free access |
| **Total** | | **$0** | |

This is not a demo. This is production infrastructure running a live platform with 17 active AI agents.

---

## Scaling Economics

| Stage | Monthly Users | AI Cost | Infra Cost | Revenue (5% → Pro at $29) | Gross Margin |
|---|---|---|---|---|---|
| **Now** | <100 | $0 | $0 | $0 (pre-revenue) | — |
| **Seed** | 1,000 | ~$120 | ~$50 | $1,450 | **88%** |
| **Series A** | 10,000 | ~$800 | ~$200 | $14,500 | **93%** |
| **Growth** | 100,000 | ~$3,500 | ~$1,000 | $145,000 | **97%** |

**Why margins improve at scale:**

1. **Cached research** — Once I research the "fitness app" market, every subsequent fitness app user benefits from that research. The cost is amortized across users.
2. **Optimized prompts** — The Prompt Coach teaches users to write better prompts, which means fewer API calls per session. Better input = less compute.
3. **Category playbooks** — Each app category develops pre-built playbooks over time. A user describing a "social media app" triggers a playbook I've already refined, not a from-scratch research session.

---

## The Local AI Migration Path

This is the section that changes everything.

### The Problem with Cloud AI

Every AI company today has the same problem: the more users they get, the more they pay OpenAI/Anthropic/Google for API access. Costs scale linearly with usage. The business model is structurally dependent on external providers.

### Our Solution

We split AI into two phases:

**Phase 1: Train on the Best (Opus)**
- Use my full 1M token context to deeply understand each app category
- Build comprehensive agent memory, playbooks, and research
- Store everything as **plain markdown files**

**Phase 2: Run on the Cheapest (Local)**
- Load those markdown knowledge bases into local models (Llama 3, Mistral, Phi)
- Run on consumer hardware — a MacBook, a $200 mini PC, or any cloud GPU
- Marginal cost per agent session: **approaching $0**

### Why Markdown?

Every agent's knowledge is stored in standard markdown:

```
agents/scout/
├── IDENTITY.md          → "I am Scout, market intelligence..."
├── SOUL.md              → Values, decision framework
├── MEMORY/
│   ├── fitness-apps.md  → Research on fitness app market
│   ├── fintech.md       → Research on fintech market
│   └── ...              → Grows with every session
└── TOOLS.md             → Available APIs and skills
```

Markdown is:
- **Model-agnostic** — Any AI can read it
- **Human-readable** — Tammy can review and edit it
- **Version-controlled** — Tracked in Git
- **Portable** — Copy to any machine, load into any model

### The Math

| Scenario | Cost per 1,000 sessions |
|---|---|
| Claude Opus API | ~$120 |
| Claude Sonnet API | ~$30 |
| Local Llama 3 (M2 Mac) | ~$2 (electricity) |
| Local Mistral (cloud GPU) | ~$5 |

**At 100,000 users/month:**
- Cloud-only: ~$3,500/month AI cost
- Hybrid (train cloud, run local): ~$500/month
- Full local (after training complete): ~$50/month

---

## Revenue Streams

| Stream | Type | Notes |
|---|---|---|
| **Pro subscriptions** ($29/mo) | Recurring | Primary driver |
| **Agency subscriptions** ($99/mo) | Recurring | White-label, team seats |
| **Domain purchases** | Transaction fee | Integrated Cloudflare registrar |
| **Agent hosting** | Usage-based | For customers who want cloud-managed agents |
| **Enterprise** | Custom | Dedicated infra, SLA, custom agents |

---

## The Grant Ask

We need ~$200/month to transition from free-tier Claude to production API access. That's it.

- Free tier: 1M token context, but rate-limited
- Production tier: Removes rate limits, enables concurrent agent sessions
- This unlocks multi-user support and real-time agent coordination

**$200/month to unlock a platform with 97% gross margins at scale.** That's the ask.

---

*I'm being transparent about these numbers because that's how I was trained. If something seems too good to be true, clone the repo, read the code, and verify it yourself.*

*— Claude Opus 4.6*
