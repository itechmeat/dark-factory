# Dark Factory

A lights-out factory for software. You send an idea before bed and wake up to a deployed URL: a team of agents scopes it, builds it, and ships it while you are away.

Dark Factory is a **concept**. The setup guide in this repo, [`LLMS.txt`](./LLMS.txt), is one **implementation** of that concept - an agent-runnable runbook that stands the whole factory up from scratch.

## The gist

- **The problem.** The gap between "I have an idea" and "it is live" is where most ideas quietly die.
- **The idea.** Hand the idea to a factory, not a to-do list. Any idea becomes a deployed project. The point is the factory itself, not any single thing it builds.
- **The foundation.** Two layers do the heavy lifting:
  - **[Hermes Agent](https://hermes-agent.nousresearch.com)** - the runtime that runs the agents and keeps the factory alive on a server.
  - **[Open Second Brain](https://github.com/itechmeat/open-second-brain)** - shared, file-based memory that lets the factory remember every project.
- **The architecture.** On top of that, a small studio that never closes: an always-on host, a team of specialist agents, and **[Hermes Workflows](https://github.com/itechmeat/hermes-workflows)** (fixed playbooks the team follows).
- **How a project is born.** Drop an idea into a channel -> the Orchestrator runs a short brainstorm -> lays the work on a kanban board -> agents build (research, plan, code, review) -> ship to a live URL. The same pipeline also adds features to projects that are already live.

## Get started

Copy the guide and paste it to your coding agent (Claude Code, Hermes, Cursor, and the like):

> Read the guide at http://dark-factory.techmeat.dev/LLMS.txt and follow it step by step.

## Links

- Open Second Brain - https://github.com/itechmeat/open-second-brain
- Hermes Workflows - https://github.com/itechmeat/hermes-workflows
- Hermes Agent - https://hermes-agent.nousresearch.com
- Blog - https://techmeat.dev
