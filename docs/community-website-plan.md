# Community Website Plan

Working title: `AI Agent UX Research Landscape`

Purpose: a public, weekly-updated map of the emerging AI agent UX research landscape. The site should help builders, researchers, and agent-platform teams understand what is changing, where tools fit, and where the open research questions still are.

## Landing Page Concept

The landing page should lead with a four-quadrant landscape map. Each point can represent a `product`, `process`, or `experimental approach`.

Recommended axes:

- X-axis: `Autonomous / synthetic evidence` to `Human-grounded evidence`
- Y-axis: `Execution verification` to `UX diagnosis and learning`

Why this works:

- It separates browser-task execution from actual UX research judgment.
- It makes synthetic users visible without overstating them as human replacements.
- It gives native builder tools, research platforms, observability systems, and papers all a place on the same map.
- It creates a natural opening for our thesis: the most interesting whitespace is calibrated diagnosis that connects agent/browser evidence with human-grounded confidence.

## Three Buckets

| Bucket | Definition | Examples |
|---|---|---|
| `Product` | A tool, platform, or commercial service people can adopt | Uxia, Crowdi, Loop11 AI Browser Agents, UserTesting, Maze, Browserbase, Replit, Lovable, v0 |
| `Process` | A repeatable workflow or operational pattern | Workflow validation loop, safe-launch review, human escalation, app-builder feedback loop |
| `Experimental approach` | A paper, benchmark, research technique, or early method | PerceptUI, What Would GPT Click, UXBench, WebTestBench, OpenComputer, AgentFixer, Qux360 |

## Initial Information Architecture

1. `Home`
   - Four-quadrant map
   - Weekly change log
   - Featured thesis
   - New additions

2. `Landscape`
   - Filter by bucket, segment, evidence quality, and date added
   - Each item gets a short page

3. `Weekly Progress`
   - Dated update posts
   - What changed, why it matters, confidence level, and sources

4. `Methods`
   - Synthetic users
   - Browser-agent evaluation
   - Human validation
   - UX observability
   - Safe-launch review

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

## Weekly Editorial Workflow

Every week, add:

1. `3-7` new or changed dots.
2. `1` paragraph on the biggest landscape shift.
3. `1` calibration note: what evidence is strong, weak, or contested.
4. `1` buyer implication: who should care and why.
5. `1` open question that became more important.

## Prototype Scope

The first HTML prototype should be a static artifact:

- No backend.
- No build system.
- In-page detail sections instead of routed pages.
- Mock weekly update data based on current docs.
- Clear visual language that can later become a real website.

