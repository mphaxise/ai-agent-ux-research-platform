# Problem-Space Taxonomy

Framing: if app-building agents are going to use UX research as a service, the problem is not just finding bugs. The real job is turning fuzzy experience quality into structured evidence that an agent can request, understand, and act on.

Legend:
- `Evidence-backed`: directly supported by market/product evidence.
- `Inference`: strategic synthesis.
- `Assumption`: unverified hypothesis.

## Major Conclusions

- `Inference | confidence: high` The hardest failure is not “the agent wrote bad code.” It is “the generated app technically works but is still confusing, untrustworthy, or misaligned with the user’s job.”
- `Inference | confidence: high` A useful service must cover both `what to test` and `how to return findings` in a machine-usable format.
- `Assumption | confidence: medium-low` Synthetic testing alone will cover many surface-level UX problems, but some higher-stakes trust and context questions will still need human escalation.

## Taxonomy

| Category | Core question | Example failure mode | Why app-building agents struggle here | Best evidence artifact | Synthetic-only fit | Basis |
|---|---|---|---|---|---|---|
| 1. Brief and audience formation | Who is this app for, and what job are they trying to complete? | Agent builds a polished flow for the wrong user or wrong task | The build prompt often lacks deep research context or a real persona | Structured research brief, job story, persona constraints | Low | `Inference` |
| 2. Information architecture and wayfinding | Can a target user understand where to start and how to navigate? | Navigation labels are generic, hierarchy is unclear, users cannot find the next step | Agents optimize for completeness, not cognitive clarity | Task-completion traces, path analysis, first-click behavior | High | `Inference` |
| 3. Visual hierarchy, copy, and affordance clarity | Do users know what is clickable, important, risky, or optional? | Primary CTA is buried, form instructions are vague, trust cues are weak | App-building agents often generate “acceptable defaults,” not strong UX judgment | Screenshot critique, click maps, transcript rationale | High | `Inference` |
| 4. Trust calibration and credibility | Does the interface create enough confidence for the user to proceed? | Payment, login, or permissions flow feels sketchy; AI claims feel overconfident | Agents rarely understand emotional trust thresholds without explicit testing | Confidence comments, hesitation points, abandon reasons | Medium | `Inference` |
| 5. Task execution and interaction flow | Can a user complete the intended goal without confusion or repeated backtracking? | Multi-step flow breaks down midway; key state changes are not obvious | Generated apps may work step by step but still create poor flow continuity | End-to-end transcript, drop-off step, error clusters | High | `Inference` |
| 6. Accessibility and inclusive defaults | Can diverse users perceive, understand, and operate the interface? | Poor contrast, weak labels, inaccessible keyboard flow, tiny touch targets | Agents can generate compliant-looking interfaces without real accessibility rigor | WCAG checks, semantic audit, annotated screenshots | High | Mix of tool-market `Evidence-backed` and product-need `Inference` |
| 7. Responsiveness and environmental edge cases | Does the UX hold up across devices, viewports, and imperfect conditions? | Mobile layout collapses; slow states create confusion; long forms are brittle | Agents tend to optimize for the “happy path” viewport first | Multi-device screenshots, responsive flow traces | High | `Inference` |
| 8. Failure debugging and root-cause attribution | When a UX issue appears, what caused it in the generation process? | The issue might come from prompt ambiguity, design defaults, code generation, or missing business context | Without attribution, the agent cannot improve systematically | Link between issue, screen state, task context, and fix suggestion | Medium | `Inference` |
| 9. Human override and escalation patterns | When should the system stop and ask for human research input? | Synthetic test results conflict, confidence is low, or risk is too high to auto-fix | A fully autonomous loop can overfit weak evidence or miss nuanced context | Escalation rule, confidence score, human review packet | Low to medium | `Assumption` |
| 10. Insight packaging back to the agent | What exact format should findings come back in so an agent can act on them? | Findings are trapped in a PDF or dashboard with no executable next step | Human-readable research reports do not map cleanly into agent workflows | Structured issue JSON, severity, evidence links, suggested fix directions | High | `Inference` |
| 11. Research memory and reuse | How does the service remember what worked, failed, or was already tested? | Agents repeat the same mistakes across apps or releases | Without memory, every run is a one-off critique | Reusable issue taxonomy, benchmark history, prior briefs | Medium | `Assumption` |

## What To Solve First

The first problem slice should be narrow enough to validate quickly but broad enough to matter.

### Best early slices

1. `Information architecture and wayfinding`
   Why: frequent, easy to demonstrate, and synthetic users can often surface it well.
2. `Visual hierarchy, copy, and affordance clarity`
   Why: common failure in AI-generated apps and easy to package back into actionable issues.
3. `Task execution and interaction flow`
   Why: closest to the buyer’s real pain of “can someone actually complete the job?”

### Important but likely later

1. `Human override and escalation patterns`
   Why: strategically important, but only after the base service generates enough signal to know when to escalate.
2. `Research memory and reuse`
   Why: becomes a moat later, but not the first wedge.
3. `Deep trust calibration for regulated or high-risk flows`
   Why: valuable, but higher burden of proof.

## Implications For Product Shape

- `Inference | confidence: high` The service should not start as a broad “research operating system.”
- `Inference | confidence: high` It should start as a narrow request-response loop that helps an app-building agent answer one practical question: `is this usable enough for the target user to proceed?`
- `Assumption | confidence: medium-low` The initial result format should likely be both human-readable and machine-readable: concise narrative summary plus structured issues and suggested next actions.
