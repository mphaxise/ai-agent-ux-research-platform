# AI Agent UX Research Platform

**A working research program for understanding how people direct, interpret, review, and recover from the actions of AI agents.**

An agent can complete a task successfully and still leave a person confused, overconfident, unable to intervene, or unsure what evidence supports the result. I started this project to investigate that gap between technical evaluation and the lived product experience.

This is not a finished platform presented as a foregone conclusion. It is a set of research artifacts, market maps, product theses, and small design probes that make the problem more concrete before the architecture hardens.

**[Explore the live AI Agent UX Research Landscape →](https://mphaxise.github.io/ai-agent-ux-research-platform/)**

## At a glance

| | |
| --- | --- |
| **Problem** | Technical success metrics do not tell us whether people understand an agent, can correct it, or know when to trust its output. |
| **What is here** | A live landscape, market and problem-space research, competing product wedges, validation plans, and emerging interaction principles. |
| **Useful for** | AI product teams, technical founders, designers, and UX researchers working on agentic products where system behavior and human judgment must stay legible to one another. |
| **Current status** | Active divergence and prototyping, with workflow validation as the lead wedge and agent UX observability as the strongest alternate direction. |

![AI Agent UX Research Landscape showing products, experimental probes, and workflow concepts mapped by evidence source and workflow depth](docs/assets/readme/ai-agent-ux-landscape.png)

*The live landscape maps products, research probes, and workflow concepts by evidence source and validation maturity. [Explore the interactive version.](https://mphaxise.github.io/ai-agent-ux-research-platform/)*

## Explore the work

- **See the field:** use the [interactive landscape](https://mphaxise.github.io/ai-agent-ux-research-platform/) to scan products, infrastructure, research, and emerging patterns.
- **Follow the reasoning:** read [what we have done so far](docs/what-weve-done-so-far.md), including the ideas we narrowed, reframed, or kept open.
- **Inspect the product options:** compare the [wedge analysis](docs/wedge-options.md) and [problem-space taxonomy](docs/problem-space-taxonomy.md).
- **Look at the two strongest directions:** read the [workflow-validation thesis](docs/workflow-validation-thesis.md) and [agent UX observability](docs/agent-ux-observability.md).
- **See what I would test next:** open the [next validation sprint](docs/next-validation-sprint.md).

## Why I am working on this

My background is in UX research, product design, and design leadership for complex expert workflows. Agentic products make many familiar design questions more consequential: what the system believes, what it is about to do, what evidence it used, whether an action is reversible, and when a person needs to step in.

I am using this repository to connect those questions to working product strategy. The aim is not to argue that synthetic evaluation replaces direct research. It is to find the places where agent-assisted diagnosis, observability, and pre-ship validation can create real value—and to define the calibration boundaries honestly.

## Product questions

- How should teams evaluate whether an agentic product is usable, not only functional?
- What information helps a person understand what an agent knows, assumes, proposes, and has already done?
- When should an agent proceed, ask for confirmation, hand off, or stop?
- How can teams inspect an agent’s trajectory without overwhelming users with implementation detail?
- Where can synthetic evaluation help, and where is direct human research still essential?
- How should confidence, provenance, uncertainty, and reversibility appear in the product experience?

## Current exploration areas

### Agent-experience observability

Experiments in turning traces, actions, tool calls, and decision points into views that support product diagnosis and human understanding.

### Evidence calibration

Ways to distinguish observed evidence, model inference, evaluator judgment, and unresolved uncertainty so that outputs do not appear more certain than they are.

### Human-review boundaries

Patterns for deciding when an agent may act independently and when meaningful human interpretation, approval, or correction is required.

### UX validation for agentic workflows

Research methods and design probes for evaluating comprehension, control, recovery, trust calibration, and handoff across multi-step agent experiences.

## Design principles

- Evaluate the user’s understanding and control, not only task completion.
- Make assumptions, proposed actions, and irreversible consequences visible.
- Preserve access to evidence without forcing every user to inspect raw traces.
- Design for correction, recovery, override, and graceful stopping.
- Separate measured behavior from interpretation and recommendation.
- Use small working experiments to clarify the product before scaling the architecture.

## Status

This is an active research-and-prototyping repository. The questions, product wedges, and architecture will continue to evolve as individual probes are implemented and evaluated. That evolution is part of the work: important changes in direction are documented rather than edited out of the story.

Related work:

- [Design Skill Pack for AI Agent Coding Platforms](https://github.com/mphaxise/design-skill-pack-for-ai-agent-coding-platforms)
- [Awesome Agent UX Research](https://github.com/mphaxise/awesome-agent-ux-research)
- [GStack Port for Codex](https://github.com/mphaxise/gstack-port-for-codex)
