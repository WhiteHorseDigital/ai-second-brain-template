# AI Second Brain Template

A starter kit for turning Claude Code into a personalized AI second brain that knows your business and does real work for you. Built by [Whitehorse AI](mailto:alex@whitehorseai.ai).

This is a **GitHub template repository**. Click **Use this template** to spin up a clean copy for a new person or company, then run the setup below.

---

## What you get

A second brain that knows your name, your business, your team, your priorities, and the decisions you have made. It can plan your day, research, draft in your voice, check in on the team, and create things. Everything it does gets saved as files in this project, so it gets smarter the more you use it.

## The idea in one line

`CLAUDE.md` is the hot cache. It gets read every time you talk to Claude Code, so it stays short and points into `memory/`. The deep context (who you are, your people, your business, how you like things written) lives in `memory/` and loads when it's needed.

```
CLAUDE.md            <- the hot cache, read every message, kept short
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

1. Install [VS Code](https://code.visualstudio.com/) (free, Windows or Mac).
2. In VS Code, open Extensions (left sidebar), search **Claude Code**, install it. Sign in when prompted (needs a paid Anthropic plan, Claude Pro or Max).
3. Click **Use this template** on this repo to create your own copy, then clone it and open the folder in VS Code. This folder is your assistant's home.

### Phase 2 — Give it life (20 min)

Open the Claude Code panel (orange button, top right) and paste the entire contents of [`SETUP-INTERVIEW.md`](SETUP-INTERVIEW.md). It interviews you one question at a time about yourself, your people, your business, and your priorities, writing each `memory/` file as you go. At the end it runs a verification pass and hands you a ~200-word Profile block to paste into Claude's Settings. Take your time and give it detail. You can say "skip" on anything and fill it later.

### Phase 3 — Give it hands (30 min)

Build your first skill. The fastest high-value one is usually connecting your project management tool (ClickUp, Asana, Notion, Monday) or a research skill. There are two example skills in `.claude/skills/` to copy the shape from. To build a new one, switch Claude Code to plan mode and describe in plain language what you want it to do.

### Phase 4 — Let it grow

Use this every day instead of web Claude or ChatGPT. Migrate your existing custom GPTs and saved prompts in ("turn this into a skill"). Log decisions. Push to GitHub so you have version control and can use it from any machine. It compounds.

---

## Prerequisites checklist

- [ ] VS Code installed
- [ ] Claude Code extension installed and signed in
- [ ] Paid Anthropic plan active (Claude Pro or Max)
- [ ] Project management tool decided (the first integration target)
- [ ] Context gathered: team list, current projects, goals, brand assets, a few emails in your voice

---

## Keeping it sharp

- `memory/current-priorities.md` — update when focus shifts
- `memory/goals.md` — update at the start of each quarter
- `memory/` generally — update the matching file when a person, priority, or preference changes
- `decisions/log.md` — append when a meaningful decision is made
- `.claude/skills/` — build a skill when you notice you have done the same thing twice
- To make your second brain remember something permanently, just tell it: "remember that I always prefer X"

---

## Placeholders

Anything written as `{{LIKE_THIS}}` is a placeholder. The setup interview fills them in, or you can edit the files directly. Search the repo for `{{` to find anything still unfilled.
