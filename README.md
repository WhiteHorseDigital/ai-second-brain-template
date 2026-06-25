# AI Second Brain Template

A starter kit for turning Claude Cowork into a personalized AI second brain that knows your business and does real work for you. Built by [Whitehorse AI](mailto:alex@whitehorseai.ai).

This is the folder Whitehorse AI sets you up with. Get it onto your computer, point Claude Cowork at it, and run the setup below.

---

## What you get

A second brain that knows your name, your business, your team, your priorities, and the decisions you have made. It can plan your day, research, draft in your voice, check in on the team, and create things. Everything it does gets saved as files in this folder, so it gets smarter the more you use it.

This is a **personal** brain: one person's context, voice, and priorities. One person, one folder.

## The idea in one line

`CLAUDE.md` is the hot cache. Cowork reads it at the start of every session, so it stays short and points into `memory/`. The deep context (who you are, your people, your business, how you like things written) lives in `memory/` and loads when it's needed.

```
CLAUDE.md            <- the hot cache, read every session, kept short
SETUP-INTERVIEW.md   <- paste this in once; it interviews you and fills memory/
memory/              <- the deep-context layer (two-tier with CLAUDE.md)
  personal.md          who you are: role, employer, location, work pattern, family
  preferences.md       voice and working style, blind spots to catch
  glossary.md          acronyms and shorthand
  goals.md             quarterly direction and targets
  current-priorities.md  ~30-day focus
  context/             one file per business unit or portfolio (company.md)
  people/              team.md, leadership.md, direct-reports.md
  external/            relationships.md (vendors, partners, advisors, agencies)
.claude/rules/       <- how you like things written
.claude/skills/      <- reusable workflows the brain can run
.claude/skills-backlog.md  <- workflows waiting to become skills
decisions/log.md     <- append-only log of meaningful decisions
projects/            <- one folder per active workstream
references/          <- SOPs and example outputs
templates/           <- reusable scaffolds
archives/            <- finished or outdated material (never delete, move here)
```

---

## Setup (the 4 phases)

### Phase 1 — Give it a home (15 min)

1. Install the **Claude Desktop** app (Mac or Windows) and sign in. Cowork needs a paid plan (Pro, Max, Team, or Enterprise) and runs on desktop only, not the web or mobile app.
2. Save this folder somewhere stable on your computer (for example `~/Cowork/second-brain/`). Don't move it afterwards.
3. Open Claude Desktop and switch to the **Cowork** tab. In the left panel, click **+** to create a project, choose **Use an existing folder**, and select this folder. That makes it your second brain's home: Cowork now reads and writes here.
4. Optional but recommended: connect your tools (Gmail, Calendar, Drive, Slack, your CRM) in **Settings → Connectors**. Leave Cowork on **"Ask before acting"** while you get comfortable.

### Phase 2 — Give it life (20 min)

In the project, paste the entire contents of [`SETUP-INTERVIEW.md`](SETUP-INTERVIEW.md) into the chat. It interviews you one question at a time about yourself, your people, your business, and your priorities, writing each `memory/` file as you go. At the end it runs a verification pass and hands you a ~200-word Profile block to paste into Claude's Settings. Take your time and give it detail. You can say "skip" on anything and fill it later.

### Phase 3 — First win and your morning plan (10 min)

Ask it: **"Draft my morning plan."** It pulls your priorities, goals, active projects, and (if connected) your calendar and inbox, and gives you a short plan for the day. This is the fastest proof that the setup paid off.

Then make it automatic. In the project, open **Scheduled Tasks**, add a new task, and paste the prompt from [`templates/morning-plan-prompt.md`](templates/morning-plan-prompt.md). Set it to run on weekday mornings. From now on the plan is waiting for you before you start.

### Phase 4 — Let it grow

Use this every day instead of web Claude or ChatGPT. Log decisions as you make them. When you notice you have done the same thing twice, ask it to turn that into a skill (see `.claude/skills/` for the shape). The more you feed it, the sharper it gets.

---

## Prerequisites checklist

- [ ] Claude Desktop app installed and signed in
- [ ] Paid Claude plan active (Pro, Max, Team, or Enterprise)
- [ ] This folder saved somewhere stable and added as a Cowork project
- [ ] Connectors decided (Gmail, Calendar, Drive, Slack, CRM, project management)
- [ ] Context gathered: team list, current projects, goals, brand assets, a few emails in your voice

---

## Keeping it sharp

- `memory/current-priorities.md` — update when focus shifts
- `memory/goals.md` — update at the start of each quarter
- `memory/` generally — update the matching file when a person, priority, or preference changes
- `decisions/log.md` — append when a meaningful decision is made
- Scheduled Tasks — adjust the morning plan, or add a weekly review, as your routine settles
- To make your second brain remember something permanently, just tell it: "remember that I always prefer X"

---

## Placeholders

Anything written as `{{LIKE_THIS}}` is a placeholder. The setup interview fills them in, or you can edit the files directly. Search the folder for `{{` to find anything still unfilled.
