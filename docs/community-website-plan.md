# Community Website Plan

Working title: `AI Agent UX Research Landscape`

Purpose: a public map of the emerging AI agent UX research landscape. We will research the space weekly, but publish a more considered website update monthly so the site remains useful rather than noisy.

## Two Workstreams

This project now has two related but distinct workstreams. They should not be treated as the same activity.

### 1. Internal Opportunity Research

Goal: find product opportunities, unmet needs, wedge options, buyer pain, and defensible solution directions.

Operating posture:

- It is acceptable to form hypotheses, take strategic positions, and prioritize likely wedges.
- The work can be opinionated because the purpose is to decide where to build.
- Evidence should still be labeled clearly as `Evidence-backed`, `Inference`, or `Assumption`.
- Reddit/community feedback, interviews, papers, product launches, and market changes are inputs into opportunity discovery.

### 2. Public Landscape Website

Goal: maintain a neutral, evolving catalog of products, workflows, papers, benchmarks, and experimental approaches in AI agent UX research.

Operating posture:

- Avoid over-claiming or presenting our preferred wedge as the landscape's conclusion.
- Treat contested areas, especially synthetic users, as contested.
- Separate current-state observations from open hypotheses.
- Document professional skepticism as data, not as a position to defeat.
- Prioritize clear placement, source links, known strengths, blind spots, and open questions.
- The site can have a point of view about uncertainty, but should not read like product marketing for our future solution.

## Editorial Guardrails

- `Current state` is preferred over `current thesis` on the public website unless we are explicitly labeling a hypothesis.
- Avoid saying synthetic users are research participants or substitutes for users.
- Use language like `synthetic probes`, `model-based signals`, or `simulated evidence` when appropriate.
- Acknowledge that agents are goal-completion systems and are not representative users.
- Treat browser QA, task completion, screenshots, evals, and UAT-style flows as emerging infrastructure rather than the same thing as UX validation.
- Include accessibility/WCAG, trust, privacy, recoverability, and quality of completion as dimensions of launch readiness.

## Landing Page Concept

The landing page should lead with a four-quadrant landscape map. Each point can represent a `product`, `workflow`, or `experimental approach`.

Recommended axes:

- X-axis: `Autonomous signals` to `Human trust / handoff maturity`
- Y-axis: `Task execution / capability checks` to `UX learning / validation maturity`

Why this works:

- It separates browser-task execution from actual UX research judgment.
- It makes synthetic users visible without overstating them as human replacements.
- It gives native builder tools, research platforms, observability systems, and papers all a place on the same map.
- It creates space to compare multiple hypotheses without forcing the map into a single conclusion.

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

4. `Viewpoints`
   - A lightweight source log for external claims, critiques, and supporting evidence
   - Public fields: `source title`, `URL`, `date`, and `claim summary`
   - Avoid adding stance, score, or rebuttal fields on the public website unless clearly labeled elsewhere

5. `Methods`
   - Synthetic users
   - Browser-agent evaluation
   - Human validation
   - UX observability
   - Launch readiness check

6. `Open Questions`
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

## Viewpoint Source Template

Public viewpoint cards should stay intentionally small:

- `Source title`
- `URL`
- `Date`
- `Claim summary`

The goal is to show the range of external viewpoints without turning the public site into an argument, endorsement, or rebuttal database.

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
