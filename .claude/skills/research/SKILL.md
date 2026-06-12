---
name: research
description: Use when you need deeper, context-aware research than a quick web search. Pulls in business context (me, work, priorities, goals) so results are tailored, then saves a sourced report to research/.
---

# Research

A reusable research skill that goes beyond a basic web search. It loads your business context first so the output is relevant to what you are actually working on, then saves a full sourced report you can return to later.

## When to use
- You want research that is tailored to your business and current projects, not generic.
- You want a saved, sourced report rather than a one-off answer in chat.

## How to run
1. **Load context.** Read `context/me.md`, `context/work.md`, `context/current-priorities.md`, and `context/goals.md` so the research is framed around what matters now.
2. **Formulate queries.** Break the question into 2-4 focused search queries.
3. **Search.** Run the searches (web search, or a research API if one is configured in `.env`).
4. **Synthesize.** Write a concise summary in chat following the communication-style rules.
5. **Save the report.** Write the full detailed version, including all source links, to `research/{{YYYY-MM-DD}}-{{topic}}.md` (create the `research/` folder if it does not exist).

## Notes
- Keep the chat summary short. The detail lives in the saved file.
- Always include source links in the saved report.
- If this needs to run cheaply or in bulk, delegate it to a sub-agent on a smaller model (see `.claude/skills/event-research/` for the pattern).
