---
name: event-research
description: Use when researching artists, vendors, venues, suppliers, or a market for an event. Events-specific version of the research skill. Saves a sourced briefing to research/.
---

# Event Research

A research skill tuned for events work. Use it to scope artists and talent, vet vendors and suppliers, evaluate venues, or size up a market or city before committing to an event.

## When to use
- Building a shortlist of artists, vendors, or venues for an upcoming event.
- Vetting a supplier or partner before reaching out.
- Sizing up a new city or market for an expansion or tour.

## How to run
1. **Load context.** Read `context/work.md` and `context/current-priorities.md` so the research is framed around the events currently in the pipeline.
2. **Identify the angle.** Talent, vendor, venue, or market. Each needs different queries.
3. **Search across 3-4 angles.** For example, for a city: the scene and key players, venue options and capacity, vendor and supplier availability, and any application or permit process.
4. **Synthesize** a short summary in chat (communication-style rules apply).
5. **Save** the full briefing with sources to `research/{{YYYY-MM-DD}}-{{event-or-topic}}.md`.

## Running it cheaply
For bulk or low-stakes research, delegate to a sub-agent so the heavy summarization runs on a smaller, cheaper model. Create `.claude/agents/event-researcher.md` with a `model:` line set to a cheaper model, and have this skill invoke it when asked for "quick" or "cheap" research.
