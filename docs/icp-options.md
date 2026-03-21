# ICP Options

Assumption: the AI agent is the primary product user, but the economic buyer is a human who owns app quality, shipping confidence, or platform trust.

Legend:
- `Evidence-backed`: grounded in cited market signals.
- `Inference`: synthesis from observed category behavior.
- `Assumption`: unverified hypothesis to test directly.

## Ranking Logic

Primary ranking here is driven by `pain severity + urgency/frequency`, then checked against budget ownership and adoption friction.

## ICP Candidates

| Rank | ICP | Jobs-to-be-done | Pain intensity | Buying trigger | Budget owner | Adoption friction | Basis | Confidence |
|---|---|---|---|---|---|---|---|---|
| 1 | AI app-builder platform teams | Increase shipped-app quality, reduce embarrassing UX failures, improve trust in the platform, and give their own agents a stronger validation loop | `5/5` severe and frequent; every bad generated app weakens product trust | Rising support tickets, poor showcase quality, pressure to move from “cool demo” to reliable production app builder | Head of Product, VP Engineering, platform GM | Medium: needs API-first workflow, low latency, security, and proof that tests improve output quality | App-builder demand is `Evidence-backed`; pain and triggers are `Inference` | Medium |
| 2 | AI-native startups using coding agents to ship customer-facing apps | Validate flows before launch without hiring a full research team; catch trust, usability, and conversion issues early | `5/5` severe and frequent; lean teams ship fast and cannot afford rework | First launch, conversion drop, onboarding complaints, failed demo, or founder distrust in AI-built UI quality | Founder, CTO, Head of Product | Low to medium: fewer procurement hurdles, but limited time and budget | Use of AI app builders is `Evidence-backed`; urgency is `Inference` | Medium |
| 3 | Enterprise internal platform teams building app-generation or workflow-building agents | Standardize UX checks before internal tools go live across many teams | `4/5` severe, `4/5` urgent; poor UX creates adoption failure and shadow IT | Executive push for internal AI tools, governance requirements, or failed rollout of generated internal apps | Internal platform lead, CIO org, head of automation | High: security review, staging access, integration burden, and slower sales cycle | Category need is `Inference` | Medium-low |
| 4 | Agencies and product studios using AI to deliver many apps or sites | Shorten review cycles, reduce revision churn, and prove quality to clients | `4/5` severe and frequent; every client handoff creates feedback loops | Margin pressure, client QA bottlenecks, or need to scale output with smaller teams | Agency founder, delivery lead, design director | Low: service firms can adopt quickly, but budgets vary widely | `Inference` | Medium |
| 5 | UX and design leads approving AI-generated prototypes before launch | Stop low-quality generated designs from reaching customers; inject user perspective into AI-heavy workflows | `3/5` severe, `3/5` urgent; meaningful but often not the strongest budget center | Design debt, stakeholder concern about brand quality, or repeated usability regressions | Design director, research lead, product design manager | Medium: may see this as complementary rather than core workflow | Substitute market evidence is `Evidence-backed`; ICP fit is `Inference` | Medium-low |

## Detailed Readout

### 1. AI app-builder platform teams

- Who they are: teams building products like app generators, site builders, or agent-first dev tools.
- Why they matter: if they embed a research layer, they can make the service a default part of the build loop rather than an optional add-on.
- Why the pain is acute: their users judge the whole platform by the quality of the generated result, not by the quality of the code alone.
- Fastest validation question: would they rather embed a UX research API into their agent loop or just expose generic E2E testing and let users improvise?
- Basis: app-builder market existence is `Evidence-backed`; buying behavior is `Assumption`.

### 2. AI-native startups using coding agents

- Who they are: small teams shipping real customer-facing apps with AI doing a large share of the implementation.
- Why they matter: this group feels the pain early and can adopt faster than large enterprises.
- Why the pain is acute: they create many fast iterations but lack dedicated research bandwidth.
- Fastest validation question: will they trust synthetic user evidence enough to gate launches or decide what to fix next?
- Basis: `Inference`.

### 3. Enterprise internal platform teams

- Who they are: central teams building internal tool generators, workflow agents, or app platforms used across a larger company.
- Why they matter: high ACV and repeat usage across many internal apps.
- Why the pain is acute: generated internal apps often fail not because they are technically broken, but because they are confusing, brittle, or inaccessible.
- Fastest validation question: is UX validation a must-have governance layer or still a nice-to-have?
- Basis: `Inference`.

### 4. Agencies and product studios

- Who they are: firms using AI builders to ship landing pages, MVPs, dashboards, or client microsites quickly.
- Why they matter: they have strong frequency and clear before/after value when revision rounds drop.
- Why the pain is acute: each round of “this feels off” feedback kills margin.
- Fastest validation question: do they want a self-serve agent workflow, or a concierge report they can white-label for clients?
- Basis: `Inference`.

### 5. UX and design approval teams

- Who they are: design leaders who now have to review AI-generated surfaces created outside traditional design workflows.
- Why they matter: they can become powerful champions even if they are not the first direct buyer.
- Why the pain is lower than the top three: they feel quality risk, but may not control the build loop or budget.
- Fastest validation question: would they buy directly, or only advocate internally for another team to buy?
- Basis: `Inference`.

## Priority Recommendation

- `Lead ICP`: AI app-builder platform teams.
  Why: highest combination of pain, urgency, repeat usage, and strategic leverage.
- `Fast-adoption ICP`: AI-native startups using coding agents.
  Why: quickest feedback loop and lowest organizational friction.
- `High-ACV follow-on ICP`: enterprise internal platform teams.
  Why: good expansion path once security, auditability, and reliability are stronger.

## What This Suggests About Positioning

- `Inference | confidence: high` Do not position this as “AI UX analytics.”
- `Inference | confidence: high` Position it as “a UX research service your app-building agent can call before shipping.”
- `Assumption | confidence: medium-low` The most compelling message to buyers may be less about “research” and more about “preventing low-trust app output from reaching users.”
