# DevPulse

A lightweight, browser-based tool that calculates a health score for 
developer tool and API-based customer accounts.

---

## Why this exists

Customer Success teams managing developer tool accounts often track 
health signals across multiple systems — usage dashboards, support 
queues, CRM notes, NPS surveys. DevPulse brings six of the most 
meaningful signals into a single input form and produces an 
actionable score with plain-English reasoning and recommended next 
steps.

The goal isn't to replace judgment — it's to give CS teams a fast, 
consistent starting point for account reviews.

---

## How the score works

Six signals are evaluated and weighted based on their importance as 
health indicators for developer tool customers:

| Signal | Max points | Why it matters |
|---|---|---|
| API call volume trend | 25 | Strongest indicator of product value realization |
| Last login (days ago) | 20 | Direct measure of recent engagement |
| Support tickets (last 30 days) | 20 | Proxy for friction and unresolved problems |
| Docs page visits | 15 | Active learning signals healthy adoption |
| NPS / CSAT score (0–10) | 10 | Direct sentiment from the customer |
| Days until contract renewal | 10 | Urgency context for the CS team |

Scores map to four health tiers:

| Tier | Score range | Meaning |
|---|---|---|
| Healthy | 75–100 | Strong engagement, low risk |
| Needs attention | 50–74 | Mixed signals, proactive outreach recommended |
| At risk | 25–49 | Multiple weak signals, intervention needed |
| Critical | 0–24 | Immediate action required |

Each tier produces a tailored reasoning summary and three specific 
recommended actions for the CS team.

---

## How to run it

No installation required. This is a single HTML file with no 
dependencies.

1. Download `index.html`
2. Open it in any modern browser (Chrome, Firefox, Safari, Edge)
3. Fill in the six input fields
4. Click **Calculate health score**

That's it.

---

## Input reference

**API call volume trend**
Whether the account's API usage is growing, stable, or declining 
over the past 30 days. Growing usage is the strongest positive 
signal — it indicates the customer is getting value and expanding 
their use of the product.

**Support tickets (last 30 days)**
Total number of support tickets opened in the past month. High 
ticket volume often indicates unresolved friction. Zero tickets is 
positive but should be read alongside login activity — silence isn't 
always healthy.

**Last login (days ago)**
How many days since the account last logged in. More than 14 days 
without a login is a warning sign for developer tool accounts, where 
regular interaction is expected.

**Docs page visits**
Qualitative measure of how actively the customer is engaging with 
documentation. High docs engagement typically signals active 
onboarding, feature exploration, or healthy self-service behavior.

**Days until contract renewal**
Used as a context and urgency signal rather than a direct health 
indicator. A low health score combined with a renewal window under 
30 days should trigger immediate escalation.

**NPS / CSAT score (0–10)**
A normalized sentiment score from the most recent NPS or CSAT 
survey. Weighted lower than behavioral signals intentionally — what 
a customer does matters more than what they say. A declining API 
trend with a high NPS score is still a risk.

---

## Built with

- **Claude** (claude.ai) — used throughout for code generation, 
  scoring logic design, and README drafting
- **Claude Code** — AI-assisted development tool by Anthropic
- **CodeRabbit** — AI code review, installed on this repository
- **GitHub** — version control and pull request workflow
- Vanilla HTML, CSS, and JavaScript — no frameworks or dependencies

---

## Author

Built by [@andievorwerk5](https://github.com/andievorwerk5) as part 
of a technical exercise exploring AI-assisted development and 
automated code review.
```

---

### How to Add It to GitHub

1. Go to **github.com/andievorwerk5/vibecode**
2. Click on `README.md`
3. Click the **pencil icon** to edit
4. Select all the existing content and delete it
5. Paste everything above
6. Scroll down and commit with this message:
```
docs: add project README with scoring methodology
