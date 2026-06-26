# Next Validation Sprint

Goal: falsify or strengthen the lead wedge in 5 working days.

Lead wedge under test: `neutral UX validation and diagnosis layer for app-building agents`

Backups still tracked:

1. `Pre-deploy UX gate for AI app builders`
2. `Human escalation brokerage for hard UX questions`

## Sprint Hypotheses

- `H1 | Assumption | confidence: low` Teams building or operating app-building agents have a painful, current need for pre-ship UX validation.
- `H2 | Assumption | confidence: low` They will trust a synthetic-user-based output enough to change what ships, especially if confidence and evidence are explicit.
- `H3 | Assumption | confidence: low` They prefer an API-like or structured service response over a generic dashboard.
- `H4 | Assumption | confidence: low` A hybrid fallback with human escalation materially increases trust without collapsing the whole product into services.
- `H5 | Assumption | confidence: low` A report that names its `calibration boundary` is more trustworthy than a report that simply presents synthetic findings as research truth.
- `H6 | Assumption | confidence: low` Teams shipping AI-generated apps want lightweight `safe-launch` flags inside UX validation, even if deep security review remains separate.

## Interview Targets

Aim for `12-15` conversations in one week:

1. `3` AI PMs or engineering leads at app-builder or coding-agent companies.
2. `3` founders, CTOs, or product leads at AI-native startups shipping customer-facing apps with AI-heavy build workflows.
3. `2` QA or test automation leads using Playwright, QA Wolf, Browserbase, or similar tooling.
4. `2` design or UX leads who currently have to approve AI-generated prototypes or apps.
5. `2` enterprise internal platform or automation leads as stretch interviews.
6. `2` builders actively using Replit, Lovable, v0, Bolt, or Base44 native testing/monitoring features.
7. `1-2` teams experimenting with Browserbase Evaluations, browser-agent verifiers, or computer-use agent benchmarks.

## Test Artifacts To Produce

Create these before or during the sprint:

1. A one-page concept brief for the lead wedge.
2. A one-page concept brief for each backup wedge.
3. A mocked request/response contract showing what an app-building agent sends and receives.
4. Two concierge-style sample reports generated on real or realistic staging apps.
5. A calibrated evidence mock showing synthetic probes, browser-agent evidence, human confirmation needs, and confidence levels side-by-side.
6. A simple comparison sheet: synthetic-only vs hybrid human escalation.
7. A competitive comparison against native builder testing, browser-agent evals, and human research platforms.
8. A lightweight safe-launch flag section that separates UX trust risks from security issues requiring expert review.

## 5-Day Plan

| Day | Objective | Activities | Outputs |
|---|---|---|---|
| Day 1 | Sharpen the ask and recruit | Finalize hypothesis deck, concept briefs, mock API response, outreach list, interview script | Interview script, outreach tracker, three wedge briefs |
| Day 2 | Test pain and buyer | Run 3-4 interviews focused on current workflow, pain severity, and trigger moments | Raw interview notes, first buyer-pattern summary |
| Day 3 | Test product shape | Show mock request/response and sample output; compare lead wedge vs backups in 3-4 more interviews | Preferred workflow format, objections list, trust concerns |
| Day 4 | Test trust and willingness to pilot | Run 3-4 interviews focused on trust thresholds, acceptable access model, and pilot willingness | Pilot signals, required safeguards, strongest ROI language |
| Day 5 | Decide | Synthesize findings, rescore wedges, document falsifiers hit or cleared | Proceed / pivot / pause memo |

## Interview Guide Focus

Each conversation should force answers to these questions:

1. What do you do today when an AI-built app "looks fine" but might still be bad UX?
2. Where does that failure create pain now: launch confidence, conversion, support, brand, or revision time?
3. If an agent could call a UX research service, what would you want it to send?
4. What would the service need to return for you to trust it?
5. Would you use this before launch, after launch, or both?
6. What access mode would you allow: screenshots, prototype, staging URL, authenticated staging, or production replay?
7. Would you pay for this as tooling, QA infrastructure, research, or premium platform capability?
8. Does seeing an explicit calibration boundary increase or decrease your trust in synthetic-user findings?
9. Should safe-launch risks, such as confusing auth, privacy surprises, fragile data handling, or obvious security red flags, live in the same report or a separate review?

## Success Criteria

Proceed signals:

1. `>= 6` interviewees describe the problem as current and painful, not merely interesting.
2. `>= 4` say they would use the service before shipping or as a deployment gate.
3. `>= 3` prefer a structured, agent-readable output over a generic dashboard.
4. `>= 2` volunteer a real prototype, staging app, or generated site for deeper evaluation.
5. `>= 2` identify a clear budget owner and a plausible budget path.
6. `>= 4` say the calibration boundary makes the report more credible rather than less credible.
7. `>= 3` want safe-launch flags included as a scoped section of the UX validation output.

Failure signals:

1. Most interviewees say generic E2E testing or human review is already enough.
2. Most interviewees reject synthetic-user evidence as too weak to influence shipping.
3. Buyers only want post-launch analytics, not research in the build loop.
4. Security or access constraints make the service unusable for real apps.
5. Calibration language makes the product feel less actionable rather than more trustworthy.
6. Safe-launch flags create category confusion that buyers expect their security or QA stack to handle separately.

## Exit Decision

### Proceed

Choose `proceed` if:

- the lead wedge wins clearly on pain and trust,
- pilot interest is real,
- and the input/output contract feels crisp enough to prototype.

### Pivot

Choose `pivot` if:

- pain is real but the preferred shape changes,
- or one of the backup wedges wins more strongly.

Likely pivots:

1. Shift to `pre-deploy UX gate` if buyers want a binary release decision more than a richer service.
2. Shift to `human escalation brokerage` if trust in synthetic results is the main blocker.

### Pause

Choose `pause` if:

- the pain is not urgent,
- no buyer emerges,
- or teams consistently view this as a nice-to-have layer on top of existing tools.

## Fastest Useful Deliverable At Week End

Produce a short memo with:

1. top 5 insights,
2. updated wedge scores,
3. strongest objections,
4. one recommended wedge,
5. one sentence on whether to proceed, pivot, or pause.
