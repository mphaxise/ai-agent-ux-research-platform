# AI Agent UX Research Platform

**Research and design probes for evaluating how people understand, direct, review, and collaborate with AI agents.**

This project explores a gap between technical agent evaluation and real product experience: an agent can complete a task successfully while still leaving users confused, overconfident, unable to intervene, or unsure what evidence supports the result.

The platform is being developed as a set of small, testable experiments around agent UX validation, observability, evidence calibration, and human-review boundaries.

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

## Intended audience

This work is for product designers, UX researchers, AI product teams, developer-tool builders, and technical founders working on agentic products where user judgment and system behavior must remain legible to one another.

## Status

This is an active research-and-prototyping repository. The architecture and experiments will evolve as individual probes are implemented and evaluated.

Related work:

- [Design Skill Pack for AI Agent Coding Platforms](https://github.com/mphaxise/design-skill-pack-for-ai-agent-coding-platforms)
- [Awesome Agent UX Research](https://github.com/mphaxise/awesome-agent-ux-research)
- [GStack Port for Codex](https://github.com/mphaxise/gstack-port-for-codex)