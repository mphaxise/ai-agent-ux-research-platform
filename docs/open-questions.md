# Open Questions

These are the highest-value unknowns for the current divergence thesis: a UX research service for app-building agents plus an alternate `agent UX observability` wedge for open flow-based personal agents.

Legend:
- `Evidence-backed`: already grounded in external evidence.
- `Inference`: reasoned but still unconfirmed.
- `Assumption`: needs direct validation.

| Open question | Why it matters | Current status | Fastest way to reduce the unknown | Basis | Confidence |
|---|---|---|---|---|---|
| 1. Who is the first buyer: app-builder platform, end product team, or agency? | Determines GTM, packaging, and integration surface | Multiple plausible buyers; no winner yet | Run 10 interviews split across those three groups and force a willingness-to-pilot comparison | `Assumption` | Low |
| 2. Will teams trust synthetic UX results enough to act before human testing? | Core adoption blocker for the lead wedge | Emerging market signal exists, but trust threshold is unclear | Show two or three real-looking sample outputs and ask if they would block a release or change a roadmap item | `Assumption` | Low |
| 3. What input context is the minimum needed for useful tests? | Too much setup kills usage; too little context kills quality | Likely needs app URL plus target user plus mission, but this is not proven | Test three input modes: URL only, URL plus persona, URL plus persona plus success criteria | `Assumption` | Low |
| 4. What output format is most valuable to the buyer and to the agent? | Product shape changes materially depending on this answer | Strong hypothesis that dual-mode output is needed | Compare preference for structured JSON, ticket bundle, short narrative report, and release recommendation | `Assumption` | Low |
| 5. Is pre-deploy or post-deploy the stronger pain trigger? | Decides lead wedge versus backup wedge | Both appear plausible from market logic | Ask interviewees to rank which budget they would spend first: prevent bad launches or triage live problems | `Inference` | Medium-low |
| 6. Where does human escalation belong? | Service design and cost structure depend on this | Likely needed for ambiguous or high-risk flows | Test appetite for three options: synthetic-only, synthetic plus optional expert review, or always-human-verified | `Assumption` | Low |
| 7. Can the service live outside app-builder platforms, or must it be embedded? | Affects GTM speed and defensibility | Standalone seems possible, but embedded could be much stronger | Ask whether teams would adopt a standalone endpoint or only use something natively inside their builder | `Assumption` | Low |
| 8. What metric creates a budget story buyers believe? | Without ROI language, “research” may feel optional | Possible metrics include launch confidence, revision reduction, conversion lift, and fewer support complaints | Force interviewees to choose the metric they would defend in a budget meeting | `Inference` | Medium-low |
| 9. What access mode is acceptable from a security perspective? | Access friction can kill pilots immediately | Unknown across startups versus enterprise | Offer ranked options: screenshots only, prototypes, staging URL, authenticated staging, production replay | `Assumption` | Low |
| 10. Is this perceived as UX research, QA, or release infrastructure? | Category framing shapes conversion | Current market blurs these boundaries | Test three value props and see which one gets the strongest “I need this now” reaction | `Inference` | Medium-low |
| 11. How differentiated can this remain if builder platforms add native checks? | Important for long-term defensibility | Unclear | Ask platforms what they would build themselves versus buy; ask non-platform teams what they would trust from a neutral layer | `Assumption` | Low |
| 12. What is the right blend of synthetic users, heuristics, and human evidence? | Determines quality ceiling and operating model | No clear answer yet | Run one concierge-style comparison on the same app using all three methods and compare perceived usefulness | `Assumption` | Low |
| 13. Should a docs/community layer be treated as a GTM asset? | Could improve discovery, credibility, interview recruiting, and category shaping without becoming the product itself | Early signal says the GitHub curation niche is open, but product value is still the main question | Track whether a docs-first hub attracts relevant contributors, interview leads, and warm intros from target buyers | `Inference` | Low |
| 14. Is the stronger first wedge around generated-app workflows or agent UX observability for open flow-based personal agents? | This changes the product surface, data model, ICP, and GTM motion | Both appear plausible; the personal-agent observability wedge now has stronger research scaffolding than before | Interview both app-builder teams and open personal-agent teams using matched concept briefs and force a tradeoff on urgency and budget | `Inference` | Low |
| 15. What remains valuable if builder platforms ship native testing, monitoring, feedback widgets, and security checks? | Platform absorption risk is now evidence-backed rather than theoretical | Native features are expanding quickly in Replit, Lovable, and v0 | Compare our concept directly against native platform features and ask what buyers would still pay an independent layer to do | `Evidence-backed` + `Inference` | Medium |
| 16. Is the moat diagnosis and repair rather than testing itself? | Browser execution and task verification are becoming infrastructure | Browserbase Evaluations, Universal Verifier, WebTestBench, and OpenComputer strengthen the verification layer | Show buyers a raw test trace, a pass/fail verifier, and a UX diagnosis packet; ask which one changes what they would fix | `Inference` | Medium |
| 17. Should we optimize for human usability, AI-agent usability, or both? | AI-first apps increasingly need to be usable by humans and by agents/computer-use systems | Browser-agent verification and AI app-builder workflows are converging | Test separate concept briefs: human usability validation, agent usability verification, and combined experience validation | `Inference` | Low |
| 18. How should reports expose the calibration boundary of synthetic evidence? | June 2026 evidence shows both progress and serious behavioral misalignment in synthetic-user methods | PerceptUI supports persona-conditioned synthetic UX evaluation, while What Would GPT Click shows first-click misalignment and UXBench shows UI-reasoning limits | Show buyers report variants with confidence labels, human-verification triggers, and synthetic-vs-human evidence provenance | `Evidence-backed` + `Inference` | Medium |
| 19. Should safe-launch risk become a first-class output dimension? | Security and privacy failures are now part of the user trust problem for AI-generated apps | TechRadar, The Verge, Axios, and new arXiv work all point to recurring vibe-coded app exposure and vulnerability patterns | Test whether buyers want safe-launch flags in the UX report or prefer those routed to separate security tooling | `Evidence-backed` + `Inference` | Medium |

## Unknowns Most Worth Killing First

These are the fastest make-or-break questions:

1. `Trust`: will buyers act on synthetic results?
2. `Buyer`: who feels the pain sharply enough to buy now?
3. `Workflow`: should this be an API, gate, or concierge packet?
4. `Access`: can customers safely expose enough of the app for the service to work?
5. `Absorption`: what must remain independent when native builder platforms add testing and monitoring?
6. `Calibration`: how do we prevent plausible synthetic findings from being overtrusted?

## What Would Count As Strong Learning

- `Evidence-backed | confidence: medium` A buyer says they would place this in a shipping loop, not just use it as occasional advice.
- `Inference | confidence: medium` Multiple interviews converge on the same input/output contract.
- `Assumption | confidence: low` At least one real team volunteers a staging app, prototype, or generated site for a pilot.
