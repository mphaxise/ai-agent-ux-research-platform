# Community Website Plan

Working title: `AI Agent UX Research Landscape`

Purpose: a public map of the emerging AI agent UX research landscape. We will research the space weekly, but publish a more considered website update monthly so the site remains useful rather than noisy.

## Landing Page Concept

The landing page should lead with a four-quadrant landscape map. Each point can represent a `product`, `workflow`, or `experimental approach`.

Recommended axes:

- X-axis: `Autonomous signals` to `Human trust / handoff maturity`
- Y-axis: `Task execution / capability checks` to `UX learning / validation maturity`

Why this works:

- It separates browser-task execution from actual UX research judgment.
- It makes synthetic users visible without overstating them as human replacements.
- It gives native builder tools, research platforms, observability systems, and papers all a place on the same map.
- It creates a natural opening for our thesis: the most interesting whitespace is calibrated diagnosis that connects agent/browser evidence with human-grounded confidence.

## Three Buckets

| Bucket | Definition | Examples |
|---|---|---|
| `Product` | A tool, platform, or commercial service people can adopt | Uxia, Crowdi, Loop11 AI Browser Agents, UserTesting, Maze, Browserbase, Replit, Lovable, v0 |
| `Workflow` | A repeatable workflow or operational pattern | Workflow validation, launch readiness check, human review handoff, app-builder feedback loop |
| `Experimental approach` | A paper, benchmark, research technique, or early method | PerceptUI, What Would GPT Click, UXBench, WebTestBench, OpenComputer, AgentFixer, Qux360 |

## Differentiation

The site should not compete with:

- AI design guidebooks such as Microsoft HAX, Google PAIR, or IBM Design for AI.
- AI-agent directories such as Agent.ai or Awesome AI Agents.
- Browser-agent benchmark suites such as WebArena or OSWorld.
- Vendor pages for synthetic-user or AI-moderated research products.
- Engineering observability tools such as Langfuse or LangSmith.

The differentiated promise is narrower: `which AI-agent product and workflow approaches are becoming launchable, trustworthy, observable, and user-validated?`

Confidence: `Inference | medium-high`, based on the external scan finding many adjacent resources but no obvious public resource combining monthly landscape map, UX validation taxonomy, source-backed dot pages, launch readiness, handoff, observability, and calibration.

## Initial Information Architecture

1. `Home`
   - Four-quadrant map
   - Monthly landscape update
   - Featured thesis
   - New additions

2. `Landscape`
   - Filter by bucket, segment, evidence quality, and date added
   - Each item gets a short page

3. `Monthly Landscape Updates`
   - Dated update posts, published monthly from weekly research notes
   - What changed, why it matters, confidence level, and sources

4. `Methods`
   - Synthetic users
   - Browser-agent evaluation
   - Human validation
   - UX observability
   - Launch readiness check

5. `Open Questions`
   - Calibration boundary
   - Human verification triggers
   - Buyer category: QA, research, product ops, or agent infrastructure
   - What builder platforms will absorb natively

## Dot Page Template

Each dot should have a compact, repeatable page:

- `What it is`
- `Bucket`
- `Where it sits on the map`
- `Who it serves`
- `Core workflow`
- `Strengths`
- `Blind spots`
- `Why it matters this week`
- `Confidence`
- `Sources`
- `Evidence badge`: product docs, benchmark, paper, community report, internal synthesis, or inference
- `UX risk tags`: synthetic overclaim, hidden state, weak consent, brittle browser grounding, poor recoverability, missing audit trail, launch risk

Source expectations:

- `Product` dots should link to the product website or official product documentation.
- `Workflow` dots should link to the internal research note plus 1-2 external articles, docs, or examples that make the workflow credible.
- `Experimental approach` dots should link to the paper, benchmark, talk, article, or project page that defines the method.

## Editorial Workflow

Every week, collect:

1. `3-7` new or changed dots.
2. `1` paragraph on the biggest landscape shift.
3. `1` calibration note: what evidence is strong, weak, or contested.
4. `1` buyer implication: who should care and why.
5. `1` open question that became more important.

Every month, publish:

1. a refreshed four-quadrant map,
2. new or changed dot profiles with source links,
3. one monthly landscape thesis,
4. one section on what became more credible,
5. one section on what remains unresolved.

## Prototype Scope

The first HTML prototype should be a static artifact:

- No backend.
- No build system.
- In-page detail sections instead of routed pages.
- Mock weekly update data based on current docs.
- Clear visual language that can later become a real website.
