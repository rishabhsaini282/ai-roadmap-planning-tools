# AI PM Tools — One-Page Selection Cheatsheet (June 2026)

> Print this. Pin it. Use it when a vendor pitches you.

---

## Step 1 — Identify Your Primary Bottleneck

Answer the one question where you lose the most time each sprint:

```
"My biggest time sink is ____________"
    │
    ├── Aggregating & reading user feedback ──────────► ROADMAP PLANNING TOOLS
    │
    ├── Writing PRDs / user stories / tickets ────────► PRD & SPEC TOOLS
    │
    ├── Running or synthesizing user interviews ───────► USER RESEARCH TOOLS
    │
    ├── Explaining features to engineering ────────────► PROTOTYPING TOOLS
    │
    └── Everything — I need a general AI assistant ───► ChatGPT / Claude
```

---

## Step 2 — Match Bottleneck to Tool

### Roadmap Planning

| If you have... | Use this |
|---|---|
| Lots of qualitative feedback from Gong/Zendesk | **Productboard** — NLP clustering is its core feature |
| Multi-team enterprise roadmap + release notes | **Aha!** — AI drafts release notes and flags dependencies |
| Simple stakeholder-facing timeline | **ProductPlan** — cleaner presentations, lighter AI |
| Engineering-led team that owns the backlog | **Linear** — AI issue triaging, dev-native |

### PRD & Spec Writing

| If you have... | Use this |
|---|---|
| Existing Jira + Confluence setup | **Atlassian Intelligence** — already bundled, no new contract |
| Notion-based documentation workflow | **Notion AI** — $10/mo add-on, stays in your existing docs |
| Complex multi-product PRD needs + Salesforce | **Craft.io** — deeper strategic alignment scoring |

### User Research

| If you have... | Use this |
|---|---|
| A growing repository of past research | **Dovetail** — centralized tagging and longitudinal synthesis |
| Primarily unmoderated usability tests | **Maze** — AI scoring on task completion, free tier for light use |
| Video-heavy moderated sessions | **UserTesting** — AI highlight reels from long recordings |
| Quick clip-sharing across sales + research | **Grain** — lightweight, free tier for 5 recordings |

### Prototyping

| If you need... | Use this |
|---|---|
| A UI component mock in 10 minutes | **v0 by Vercel** — paste a description, get a React component |
| A multi-screen app prototype for a customer call | **Lovable** — full app with navigation and state |
| A demo with a backend (API calls, data) | **Bolt.new** — full-stack scaffolding from a prompt |

---

## Step 3 — Check the Free Tier Reality

| Tool | Free Tier Worth Using? | Hard Limit |
|---|---|---|
| Maze | Yes (1 study/mo) | Hits wall at sprint-scale testing |
| Grain | Yes (5 recordings) | Outgrows immediately for active research |
| Linear | Yes | Scales well until you need enterprise integrations |
| v0 | Yes (~200 credits) | Burns fast on complex UIs |
| ChatGPT | Yes (GPT-4o with limits) | Rate limits during heavy planning weeks |
| Notion AI | No | AI not included on free Notion plan |
| Productboard | No | No free tier |
| Aha! | No | No free tier |
| Dovetail | Limited | AI features require paid plan |

---

## Step 4 — Evaluate Before You Sign

**Questions to ask every AI PM tool vendor:**

1. Does background AI processing count against my token/credit quota?
2. What is the data residency policy for our customer feedback we upload?
3. Is Jira sync bi-directional, or does it only push one way?
4. What is the per-seat count — named users or concurrent?
5. What does the AI do when it has low confidence? Does it flag uncertainty or silently guess?

---

## Key Numbers to Remember

- **40%** — planning overhead reduction from NLP feedback loops in roadmap tools (source: ai-roadmap-planning-tools.html)
- **80%** — reduction in initial PRD drafting time with AI spec tools (source: ai-prd-writing-tools.html)
- **$20/mo** — entry point for most general AI PM assistants (ChatGPT Plus, Claude Pro, v0, Bolt)
- **$10/mo** — Notion AI add-on price (cheapest AI writing layer if you're already on Notion)
- **$59/mo** — Aha! per-user starting price (most expensive listed tool in this comparison)

---

## AI Guardrail Rules for PMs

1. **Never prompt without source material.** Include the raw data in the prompt; don't ask the model to recall it.
2. **Flag, don't auto-accept, AI prioritization scores.** Algorithms optimize for what they can measure. Org politics, technical debt context, and strategic pivots are not in the training data.
3. **Prototype ≠ spec.** AI-generated code demos clarify requirements — they are not engineering starting points.
4. **Synthetic users ≠ real users.** AI-simulated interview respondents reflect training data, not your customer segment.
5. **Read the hallucination.** If the AI output sounds confident about a number you didn't provide, verify it before putting it in a PRD.

---

*Source: [productleadersdayindia.org/PLDIBlogs.html](https://productleadersdayindia.org/PLDIBlogs.html) — Updated June 2026*
