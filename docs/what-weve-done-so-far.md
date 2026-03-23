# What We've Done So Far

This article captures the work completed so far across the divergence phase of the `ai-agent-ux-research-platform` project. It is not a build log in the narrow sense. It is the story of how the idea evolved, what we learned from the market, what artifacts we created, where we changed our mind, and what now looks like the most promising direction.

## The Starting Point

We began with a broad thesis: if AI agents can now build apps quickly, they also need a way to get fast, usable, trustworthy feedback on what they have built. The original framing was `UX research as a service for AI agents`, especially for agents that generate websites or apps and need validation before shipping.

From the start, the important nuance was that the AI agent would be the operational user of the service, but a human product lead, founder, designer, or engineering lead would still be the buyer and approval surface. That distinction shaped the work that followed. We were never just exploring "a research tool." We were exploring an agent-callable layer that could sit inside a generation loop.

## Building The First Divergence Pack

The first major output was a six-document divergence pack in this repo:

- `docs/divergence-market-map.md`
- `docs/icp-options.md`
- `docs/problem-space-taxonomy.md`
- `docs/wedge-options.md`
- `docs/open-questions.md`
- `docs/next-validation-sprint.md`

Those documents gave the project an initial structure:

- a market map of direct competitors, substitutes, adjacent platforms, and internal-tool alternatives
- a set of ICP candidates and buying dynamics
- a taxonomy of problem spaces for agent UX and UX research
- multiple wedge concepts scored with an explicit framework
- a one-week validation plan
- a running list of strategic unknowns

At this stage, the most important move was not choosing a product. It was forcing breadth before narrowing. We deliberately kept multiple possibilities alive long enough to compare them against explicit criteria instead of falling in love with the first plausible idea.

## What The Market Work Revealed

As the market map deepened, the landscape became more legible. We found a real but still early category around synthetic or AI-led usability testing, with products such as Uxia, Crowdi, Loop11 AI Browser Agents, and RUXAILAB. We also found strong adjacent infrastructure in Browserbase, Stagehand, Zencoder, QA Wolf, LogRocket, and Fullstory.

The key insight was that these tools do not all compete in the same way. The market actually splits into at least two clusters:

1. researcher-facing synthetic testing
2. builder-facing autonomous validation

That split matters. Research-facing tools assume a human researcher or product manager is framing, interpreting, and acting on the study. What we were more interested in was a service contract that could be called by a builder agent itself:

`here is the app, target user, task, and context; return structured findings, evidence, severity, and suggested fixes`

Community research sharpened this further. Reddit and Hacker News discussions did not reject the idea of synthetic testing outright. The consistent objection was trust. People wanted synthetic findings benchmarked against reality before they would treat them as a real shipping signal. That pushed us toward a framing closer to `pre-ship validation`, `confidence checks`, and `usability triage`, rather than "AI replaces user research."

## The Lead Wedge Became Sharper

Out of the wedge analysis, one direction stood out as the current lead:

`Task-based synthetic UX test API for app-building agents`

This wedge scored highest because it sits directly in the pain created by AI app generation. Agents can create software quickly, but fast generation does not imply usable workflows, clear interaction patterns, or trustworthy outcomes. A validation layer that runs before launch could become part of the agent's normal loop rather than a separate, slower research process.

We also kept strong backups alive:

- `Pre-deploy UX gate for AI app builders`
- `Human escalation brokerage for hard UX questions`
- later, `Agent UX observability for open flow-based personal agents`

The key here is that we did not collapse the landscape into a single winner too early. The lead wedge earned its position through explicit scoring, but the alternatives remain active because each one corresponds to a real risk in the lead thesis.

## From Broad Wedge To Concrete Workflow

A major step forward came when the abstract wedge was turned into a more concrete thesis: a `workflow validation loop for AI-generated apps`.

That led to the document `docs/workflow-validation-thesis.md`, which made the service feel much more real. The concept became:

- an app-building agent submits a validation request with a URL, workflow, audience, and success criteria
- a browser QA baseline checks mechanical completion first
- hosted testers or synthetic users run the workflow
- clicks, keystrokes, timings, screenshots, path deviations, and post-task ratings are captured
- the system synthesizes a small number of runs into a structured diagnosis
- the diagnosis is handed back to the builder agent or human operator
- the agent patches, reruns, escalates, or approves

This was an important conceptual shift. Instead of imagining a giant dashboard from day one, we started seeing that the first product might only need three things:

- a request surface
- a hosted task page
- a results packet

That was the first moment where the product started to feel like a real service loop instead of a generic platform idea.

## The Docs-First Detour Was Useful

During the divergence work, we also asked a different question: is there already a strong docs-only GitHub repo collecting material about AI agent UX and UX research for AI agents?

We found adjacent repos in human-AI interaction, human-AI collaboration, and agent papers, but nothing that cleanly combined:

- AI agent UX
- UX research for agents
- market tools
- evaluation methods
- community discussions
- practical design and validation patterns

That looked like real whitespace, so we created a separate docs-only repo:

`awesome-agent-ux-research`

This repo served as a category-shaping and discovery asset rather than the main product. It pulled together products, papers, community signals, and design or evaluation patterns in a GitHub-native form. Later, after reflecting on what that repo really represented, we integrated the lesson back into the main divergence work:

- a docs-first layer is useful
- but it should be treated as a GTM and category-legibility asset, not the product itself

This was one of the healthiest course corrections in the process. It let us separate an ecosystem contribution from the core business wedge.

## A Second Direction Emerged: Personal Agents

The next major turn came when we explored another direction altogether: what if the better opportunity is not around generated apps, but around `open flow-based personal agents` like OpenClaw-style systems?

This changed the artifact under study. In the app-builder wedge, the unit of analysis is mostly a task flow on a website or app. In the personal-agent wedge, the unit of analysis becomes a richer loop:

- transcript
- flow transitions
- tool calls
- retries
- user corrections
- repair attempts
- recovery or abandonment

That led to `docs/cloud-agent-conversation-ux-thesis.md`, which framed a possible product for analyzing conversation-plus-execution behavior. But even while that work was useful, another insight emerged: calling this "UX research" was no longer quite right.

## The Category Language Changed

As we dug into literature and adjacent tools, it became clear that this second branch looked less like classic UX research and more like `observability from a UX angle`.

That led to a more precise framing:

`Agent UX Observability`

The new framing is documented in `docs/agent-ux-observability.md`. The core claim is that some of the opportunity here is not about running discrete research studies at all. It is about observing live agent interactions, detecting critical incidents, reconstructing what happened, and handing back fix-ready diagnoses from the user's point of view.

This framing was grounded by adjacent methods:

- digital experience monitoring
- session replay and AI-assisted summarization
- conversational analytics
- qualitative dialogue analysis
- satisfaction prediction from logs
- breakdown and repair analysis
- human-AI interaction rubrics
- LLM-assisted qualitative coding with explicit guardrails

That work gave the personal-agent branch a clearer identity. It also protected us from forcing everything into the "research platform" label when the product logic was starting to look more like observability plus incident synthesis.

## The OpenClaw Research Added Real Whitespace

Once OpenClaw became the reference example, we did a focused pass on whether an ecosystem already exists for `UX incident analysis as a service` inside OpenClaw-style companies.

The findings are now captured in `docs/openclaw-service-landscape.md`.

The most important conclusion was that OpenClaw appears technically extensible enough for this category today. Official docs and ecosystem examples suggest that plugins can access rich runtime surfaces, including:

- session transcripts
- message hooks
- tool hooks
- lifecycle hooks
- background services
- Gateway RPC and HTTP routes

We also found adjacent extension patterns such as memory plugins, telemetry bridges, workflow plugins, and infrastructure monitors. What we did not find was a mature, well-known UX-observability layer that:

- detects misunderstandings or trust drops
- backtraces the local context that caused them
- builds a textual and visual incident packet
- returns fix-ready insight to the company running the agent

That absence matters. It means the OpenClaw branch is not just a random adjacent idea. It is an actual whitespace candidate with enough technical surface to be plausible.

## The Two Main Directions Now Look Distinct

At this point, the project has two serious directions on the table:

### 1. Workflow validation for AI-generated apps

This remains the current lead wedge because the buyer pain is easier to see, the integration story is clearer, and the output contract is more immediately legible.

### 2. Agent UX observability for open flow-based personal agents

This is now the strongest alternate direction because it maps to a real technical ecosystem, a different data model, and a potentially important emerging category.

The main strategic question is no longer "is there an idea here?" It is "which product surface represents the most urgent, reachable, high-value first wedge?"

That open tension is now explicit in `docs/open-questions.md`.

## We Also Started Separating Product Work From Idea Capture

Another useful side move was operational rather than strategic. We found a `docs/build-ideas.md` document living in the awesome-list repo even though it really belonged in `PraneetIdeas`.

We moved it to the right home:

- added to `PraneetIdeas`
- removed from `awesome-agent-ux-research`

That might sound small, but it reflects a broader cleanup principle in this project: category-shaping assets, product research, and raw idea capture should live in the right places. Otherwise the repositories start to blur together and the reasoning becomes harder to trust.

## What Exists Now

Today, the main repo contains a coherent divergence set:

- market map
- ICP options
- problem taxonomy
- wedge scoring and recommendation
- open questions
- validation sprint plan
- workflow validation thesis
- personal-agent conversation thesis
- agent UX observability framing
- OpenClaw service landscape

Those artifacts together represent a real body of thought, not just scattered brainstorming.

## What Changed Most In Our Thinking

Several shifts mattered more than the others:

First, we moved from a broad "UX research platform" idea toward a much sharper `agent-callable validation loop`.

Second, we learned that the market should be read as two different opportunities: synthetic research workflows for humans, and autonomous validation or observability loops for agent builders and operators.

Third, we realized that one of the alternate branches is better framed as `Agent UX Observability` than as traditional UX research.

Fourth, we discovered that a docs-first GitHub layer is valuable, but mainly as a distribution and category-making asset rather than the product.

Finally, we ended this phase with a healthier strategic posture: one lead wedge, two serious backups, explicit falsifiers, and a much better vocabulary for what we are actually trying to build.

## The Current State

If we summarize the state of the project in one sentence, it is this:

We started by asking how app-building agents could use UX research as a service, and we now have a much more concrete answer in the form of a workflow-validation wedge, alongside a credible alternate category in Agent UX Observability for OpenClaw-style personal agents.

That is meaningful progress. The idea is no longer vague. The landscape is clearer, the wedge options are more defensible, the unknowns are explicit, and the work now lives in a cleaner set of repositories than when we began.
