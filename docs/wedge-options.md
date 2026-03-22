# Wedge Options

Framing: the product thesis here is a UX research service that app-building agents can call before or after shipping. The wedge should be narrow enough to validate in one week, but strong enough to point toward a defensible category.

Legend:
- `Evidence-backed`: grounded in cited market signals.
- `Inference`: strategic synthesis.
- `Assumption`: unverified hypothesis.

## Scoring Framework

Weighted score out of 100:

- Pain severity `30%`
- Urgency / frequency `20%`
- Willingness to pay `20%`
- Differentiation potential `15%`
- GTM reachability `15%`

Calculation used here:

- Pain score contribution = raw score x `6`
- Urgency contribution = raw score x `4`
- WTP contribution = raw score x `4`
- Differentiation contribution = raw score x `3`
- GTM contribution = raw score x `3`

## Score Table

| Wedge | Pain (30%) | Urgency (20%) | WTP (20%) | Diff. (15%) | GTM (15%) | Total / 100 | Basis | Confidence |
|---|---:|---:|---:|---:|---:|---:|---|---|
| 1. Task-based synthetic UX test API for app-building agents | 5 | 5 | 4 | 4 | 4 | 90 | Mostly `Inference`, supported by app-builder and synthetic-testing market evidence | Medium |
| 2. Pre-deploy UX gate for AI app builders | 4 | 4 | 4 | 4 | 4 | 80 | `Inference` | Medium |
| 3. Human escalation brokerage for hard UX questions | 4 | 3 | 5 | 5 | 3 | 80 | `Inference` | Medium-low |
| 4. Post-ship feedback-to-fix service | 4 | 4 | 4 | 3 | 4 | 77 | `Inference` | Medium |
| 5. Research memory layer for builders | 3 | 3 | 3 | 4 | 4 | 66 | `Assumption` heavy | Low |
| 6. Public UX benchmark / certification for AI-generated apps | 2 | 2 | 2 | 4 | 4 | 52 | `Assumption` heavy | Low |

## Wedge Readout

### 1. Task-based synthetic UX test API for app-building agents

- User: app-building agent plus the human team operating it.
- Painful moment: the agent can generate an app fast, but nobody knows whether a target user can actually complete the intended job confidently.
- Value proposition: send the app URL, audience, mission, and context; receive structured findings, evidence, severity, and suggested fixes.
- Most credible first instantiation: a `workflow validation loop` that combines automated browser QA baseline checks, a small number of human or synthetic task runs, and post-task ratings before handing a structured diagnosis back to the builder agent.
- Differentiator: API-first and agent-consumable, rather than a human-only dashboard or one-off study.
- Expected willingness to pay: `Inference` says medium-high to high, because this can sit on the critical path of app quality and trust. Plausible starting range: startup tooling budget or platform add-on budget rather than enterprise research budget.
- Business potential: High. Expansion path could include recurring validation, regression history, and human escalation.
- Defensibility thesis: proprietary corpus of app contexts, personas, issue patterns, fix suggestions, and acceptance behavior from agents and humans.
- Key risk: synthetic findings may not be trusted enough as a standalone shipping signal.

### 2. Pre-deploy UX gate for AI app builders

- User: builder platforms and teams that want a pass/fail check before publish.
- Painful moment: generated apps get deployed too quickly and fail obvious UX tests after users see them.
- Value proposition: lightweight UX quality gate with a score, must-fix issues, and a release recommendation.
- Differentiator: easier buying story than a full research platform; aligns with deployment workflows.
- Expected willingness to pay: `Inference` says high enough if attached to deployment confidence and reduction in failed launches.
- Business potential: High if embedded in builder platforms, medium if sold as a standalone gate.
- Defensibility thesis: release history, regression baselines, and accumulated threshold logic.
- Key risk: may be copied by app-builder platforms once the scoring logic becomes obvious.

### 3. Human escalation brokerage for hard UX questions

- User: teams or agents that hit ambiguous or high-stakes experience decisions.
- Painful moment: synthetic tests give weak or conflicting signals, but waiting weeks for formal human research is too slow.
- Value proposition: one request routes to a rapid human-assisted research packet with concise findings that an agent or operator can act on.
- Differentiator: bridges autonomous generation with real human judgment at the exact moment confidence is low.
- Expected willingness to pay: `Inference` says high ACV potential, because buyers already pay heavily for credible human research.
- Business potential: Medium-high, especially in higher-risk workflows.
- Defensibility thesis: service quality, speed, reviewer network, and structured handoff back into builder loops.
- Key risk: can become services-heavy and operationally complex.

### 4. Post-ship feedback-to-fix service

- User: teams shipping AI-built apps that now have traffic or internal usage.
- Painful moment: complaints, session replays, and support tickets exist, but nobody turns them into clear next fixes for the agent.
- Value proposition: ingest real-world feedback and convert it into prioritized UX issues and improvement requests.
- Differentiator: links live evidence to agent remediation.
- Expected willingness to pay: `Inference` says medium-high because it touches support load and retention.
- Business potential: Good expansion path, but less sharp as a first wedge.
- Defensibility thesis: learning loop from real user evidence to fixes.
- Key risk: looks too similar to analytics + issue triage tools.

### 5. Research memory layer for builders

- User: repeat builders, platforms, or internal teams generating many apps.
- Painful moment: every new app starts from shallow UX assumptions and repeats known mistakes.
- Value proposition: persistent memory of personas, prior tests, accepted fixes, and UX rules that agents can consult before building.
- Differentiator: long-term learning layer, not just a one-off test runner.
- Expected willingness to pay: `Assumption` says medium, but urgency is likely lower early on.
- Business potential: Strong moat later, weak initial wedge.
- Defensibility thesis: institutional memory across many builds and customers.
- Key risk: too abstract and not painful enough to win as the first product.

### 6. Public UX benchmark / certification for AI-generated apps

- User: builder platforms, agencies, or teams that want external proof of app quality.
- Painful moment: everyone claims their AI-generated apps are usable, but nobody trusts the claims.
- Value proposition: benchmark or certify generated app experiences against a shared standard.
- Differentiator: category-defining if it wins.
- Expected willingness to pay: likely weak early, since buyers care more about fixing issues than collecting badges.
- Business potential: potentially large later, but poor first wedge.
- Defensibility thesis: benchmark brand and standard-setting.
- Key risk: too far from urgent workflow pain.

## Recommendation

### Lead wedge

`Task-based synthetic UX test API for app-building agents`

Why this lead wedge:

- `Evidence-backed | confidence: medium` Both sides of the market now exist: app-building agents are real, and synthetic UX testing tools are real.
- `Inference | confidence: high` What is still missing is an agent-first service contract that turns UX validation into something callable, repeatable, and actionable inside the generation loop.
- `Inference | confidence: medium` This wedge is narrow enough to test quickly, yet broad enough to expand into gating, human escalation, and long-term research memory.

### Backup wedges

1. `Pre-deploy UX gate for AI app builders`
   Why keep it alive: if buyers do not want a broad API but do want a shipping decision, this is the cleanest simplification.
2. `Human escalation brokerage for hard UX questions`
   Why keep it alive: if synthetic-only trust is weak, a hybrid service may be the fastest path to credibility.

## Why Now

- `Evidence-backed | confidence: high` Tools like Replit Agent, v0, and Lovable are pushing app creation speed up dramatically.
- `Evidence-backed | confidence: medium` Synthetic testing entrants like Uxia, Crowdi, and Loop11 AI Browser Agents show growing willingness to let AI participate in usability evaluation.
- `Evidence-backed | confidence: medium` Browser infrastructure and agentic test execution layers like Browserbase, Stagehand, and Zencoder make automated interaction technically feasible.
- `Inference | confidence: high` The result is a timing window where app creation is getting automated faster than experience validation.

## Why This Team

- `Assumption | confidence: low` This team appears best suited if it can combine agent systems thinking, product judgment, and UX research taste.
- `Inference | confidence: medium` The opportunity is early enough that a small team can still win by defining the request/response contract and delivering obviously better outputs than improvised Playwright-plus-prompt hacks.
- `Assumption | confidence: low` If the team is comfortable doing a service-heavy first phase, it can learn faster than dashboard incumbents that are optimized for broader, slower workflows.

## Fast Falsifiers

If any of these happen in the next 7 days, the lead wedge should be reconsidered fast:

1. Buyers say synthetic UX evidence is interesting but not trustworthy enough to change what ships.
2. App-builder platforms say they would rather expose generic QA hooks than a dedicated UX research layer.
3. Teams want only post-launch analytics, not pre-launch validation.
4. The preferred output is a human narrative report, not an agent-readable response.
5. Security objections block teams from giving a service access to staging apps or generated builds.

## Risks And Failure Modes

| Risk | Why it matters | Mitigation |
|---|---|---|
| Synthetic fidelity gap | Weak trust kills adoption fast | Start with narrow tasks and confidence rules; keep human escalation as fallback |
| Category confusion with QA | Buyers may think this is just another testing tool | Keep messaging centered on usability, trust, and user-task success rather than functional correctness |
| Platform absorption risk | Builders may copy obvious gating logic | Win on speed of learning, issue corpus, and structured feedback loop, not just scorecards |
| Data access friction | Without app access, no service can run | Validate acceptable access modes early: screenshots, prototypes, staging URLs, or recordings |

## Not In Scope For The First Wedge

- Full observability platform: too broad and already crowded.
- General-purpose human research suite: too slow and operationally heavy.
- Public benchmark standard: interesting later, weak near-term urgency.
- Broad analytics dashboard: easy to drift into adjacent categories and lose the agent-first thesis.
