# Pet Brains

**Tools and methodology for builders who code with AI.**

Open-source frameworks and workflows for shipping real products with AI agents — not endless prototypes.

→ [YouTube](https://youtube.com/@petbrains)  ·  [Tools](#tools)  ·  [petbrains.dev](https://petbrains.dev)

---

## The problem we keep hitting

AI coding agents are brilliant but unreliable. They hallucinate. They cut corners — stubs, mocks, "TODO: implement later". They forget context between sessions. They say "done" when work is half-finished. You start using AI to save time and end up debugging its mistakes.

The fix is not better prompts. It is structured workflow:  
**specs before code, verification before commit, documents as source of truth.**

---

## Our approach: Document-Driven Development

> If the agent performs poorly, the task description is lacking.

LLMs are strong reasoners but unreliable workers. We treat that as a process problem, not a model problem. Every Pet Brains tool is built on one rule:  
**specifications generate code, not the other way around.**

```
Define  →  Design  →  Build  →  Verify  →  Ship
 PRD       UX/Plan    TDD       Review     Memory
```

Each tool below is a working implementation of this methodology. We use them on our own builds. If they don't survive production, they don't ship.

---

## Tools

Built in our workflow. Shared with you.

Each tool started as something we needed in our own builds. Free, open source, and ready to drop into your Claude Code setup.

### [mvp-builder](https://github.com/petbrains/mvp-builder)
**Build MVPs with an AI agent that verifies its own work.**  
A Document-Driven Development framework for Claude Code. Specs generate code, TDD cycles guarantee tests, self-review catches the agent before it commits broken work, and session memory keeps context across runs.

### [design-builder](https://github.com/petbrains/design-builder)
**Design plugin for Claude Code — distinctive production-grade interfaces on web and iOS.**  
Four user-facing commands (`/setup`, `/create`, `/improve`, `/review`) cover the full design pipeline. A knowledge-base skill (anti-patterns, motion, HIG, BM25 search) backed by `designlib-mcp` does the heavy lifting. You stay in conversation with one of four entry points.

### [designlib-mcp](https://github.com/petbrains/designLib-mcp)
**A curated design-knowledge catalog for AI coding agents.**  
Stop letting Claude, Cursor, or Copilot guess hex codes and font pairings. Give them a real, opinionated source of truth — over MCP. Powers `design-builder` and works standalone in any MCP-capable client.

*We ship something new every few weeks. Subscribe on [YouTube](https://youtube.com/@petbrains) to hear when the next tool drops.*

---

## Beyond the tools

Tools are an instance of the methodology. **[petbrains.dev](https://petbrains.dev)** is where we write up the methodology itself — walkthroughs, build films, and deeper dives into how we work.

Subscribe on [YouTube](https://youtube.com/@petbrains) for new builds and methodology breakdowns.

---

## How we build

**Skin in the game.** We use what we ship. If we wouldn't run it on our own production code, we don't release it.

**Substance over hype.** The AI space has enough thought leaders. We focus on tools that compound — the unsexy infrastructure that quietly works.

**Permanent learner mode.** This field changes monthly. So do our tools, our patterns, and our priors.

**Strong opinions, weak attachments.** We respect feedback. We don't outsource our thinking.

---

## Connect

- **YouTube** — [@petbrains](https://youtube.com/@petbrains) — workflows, builds, demos
- **GitHub** — [github.com/petbrains](https://github.com/petbrains) — all repositories  
- **petbrains.dev** — methodology, walkthroughs, build films

*All projects MIT licensed.*
