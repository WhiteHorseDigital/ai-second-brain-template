# Morning Plan — scheduled task prompt

Paste the block below into a Claude Cowork **Scheduled Task** (in the project: Scheduled Tasks → add task). Set it to run on weekday mornings, before you start work. Tweak the wording to taste.

---

Draft my morning plan for today.

First load context: read `memory/current-priorities.md`, `memory/goals.md`, and the READMEs of any active workstreams in `projects/`. If a calendar, email, or task connector is available, pull today's meetings, anything that needs a reply, and tasks due today or overdue.

Then give me, in this order and kept tight:

1. **Today's focus** — the one or two things that matter most, tied to my current priorities.
2. **Calendar** — meetings today with times, and anything I need to prep for.
3. **Needs a reply** — emails or messages waiting on me, most important first.
4. **Due or overdue** — tasks with a deadline of today or earlier.
5. **One nudge** — a priority or goal I have not touched in a while, if anything stands out.

Follow my communication style (see `.claude/rules/communication-style.md`). Short and scannable. Don't invent items: if a source is not connected or has nothing, say so in one line and move on.
