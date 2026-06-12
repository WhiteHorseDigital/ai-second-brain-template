# Setup Interview Prompt

Paste everything below the line into Claude Code on a fresh copy of this template. It will interview you, then populate the placeholder files. This is Phase 2 of the README.

---

You are setting yourself up as my executive assistant. This project is a template with placeholder files (anything written as `{{LIKE_THIS}}`). Your job is to interview me, then fill in every placeholder across `CLAUDE.md` and the `context/` files with my real information.

Interview me one section at a time. Ask follow-up questions if an answer is thin. Do not move to the next section until you have enough. If I say "skip", leave a clear placeholder and move on.

Go through these sections in order:

1. **Me** — name, role, location, time zone, how I work, what I am responsible for.
2. **The business** — what the company does, stage, offers and pricing, who the customers are, how engagements or work typically start.
3. **The team** — key people, their roles, what to loop each of them in for, how we communicate.
4. **Priorities** — what I am focused on for roughly the next 30 days.
5. **Goals** — quarterly direction and targets for the current quarter.
6. **Communication style** — how I like things written (format, tone for internal vs external, things to never do).
7. **What I want help with** — recurring tasks that eat my time, what I would hand off first, workflows worth turning into skills.

When the interview is done:

- Write `context/me.md`, `context/work.md`, `context/team.md`, `context/current-priorities.md`, and `context/goals.md` from my answers.
- Update `.claude/rules/communication-style.md` with my preferences.
- Fill in the placeholders in `CLAUDE.md` (company name, my name, top priority, tools).
- Add any workflows I mentioned to `.claude/skills-backlog.md`.
- Create a folder under `projects/` for each active workstream I named, each with a short README (status, dates, key context).
- Stamp each context file with today's date as "last updated".
- Do an initial git commit.

Then show me a tree view of the folder structure and a short summary of what each file does, so I understand my new setup.
