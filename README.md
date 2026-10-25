# AI Projects

A collection of AI skills and workflows I use for business analysis, marketing and strategy work.

## Skills

### Competitive Brief

[`competitive-brief/SKILL.md`](competitive-brief/SKILL.md)

A Claude skill that turns an AI assistant into a structured competitive analyst. Given a competitor or a feature area, it scopes the question, researches the market (product pages, pricing, launches, press, customer reviews, job postings) and produces a decision-ready brief.

**What the brief covers**

| Section | What it answers |
|---|---|
| Competitor overview | Who they are, who they target, recent momentum |
| Feature comparison | Capability-by-capability matrix with a consistent rating scale (Strong / Adequate / Weak / Absent) |
| Positioning analysis | How each player positions itself — category, differentiator, value proposition, proof points |
| Strengths & weaknesses | Evidence-based, drawn from customer reviews rather than marketing claims |
| Opportunities & threats | Gaps to exploit, competitor bets, vulnerable positions |
| Strategic implications | What to build, differentiate on, reposition or monitor — the "so what" |

The skill also includes reference frameworks for competitive landscape mapping (direct, indirect, adjacent and substitute competitors), win/loss analysis, and market trend identification.

**Use cases:** product strategy, feature prioritisation, sales battle cards, board/investor materials, pricing reviews.

**How to use it:** add the `competitive-brief` folder as a skill in Claude, then ask for a brief, e.g. *"Write a competitive brief on Citroën's electric range vs. its main rivals in France, focusing on pricing and product features."*

**Example output:** [Citroën EV Competitive Brief — France, Oct 2026](competitive-brief/examples/citroen-ev-competitive-brief.md)

I used this skill to compare Citroën's four electric cars (ë-C3, ë-C3 Aircross, ë-C4, ë-C5 Aircross) against 12 rivals in the French market, including Renault, Dacia, Tesla, VW and Chinese newcomers. The brief covers:

- **Pricing and feature matrices** built from manufacturer price lists and the French motoring press
- **French EV incentives** (CEE prime, leasing social 2026) and how they shift competition
- **Sales momentum** from September 2026 registration data
- **Positioning and SWOT**, ending in five strategic recommendations for Citroën

Key finding: Citroën competes on headline price alone, a position rivals can easily copy, while its real advantage is space-per-euro.

---

*Author: [Rohaan Sunil](https://github.com/RohaanSunil29)*
