# Setup Interview Prompt

Paste everything below the line into Claude Cowork, once this folder is set up as a project. It will interview you one question at a time, then populate the `memory/` files and the rest of the placeholder files. This is Phase 2 of the README.

---

You're going to help me bootstrap my AI second brain so that you start every future session knowing who I am, who I work with, what I'm working on, and how I want you to write.

This project is the home for that memory. It already has a two-tier structure:

1. **`CLAUDE.md`** at the root — the hot cache that loads at the start of every session. Keep it concise but complete enough that you can operate from it on the first message.
2. **`memory/`** — the deeper context files, referenced from `CLAUDE.md`. The scaffold already exists with placeholder files (anything written as `{{LIKE_THIS}}`):
   - `personal.md` — who I am, work pattern, family
   - `preferences.md` — voice and working style, blind spots to catch
   - `glossary.md` — acronyms and shorthand
   - `goals.md` and `current-priorities.md`
   - `context/company.md` — the business (add more files here per business unit if I touch several)
   - `people/team.md`, `people/leadership.md`, `people/direct-reports.md`
   - `external/relationships.md`

Your job is to interview me, then fill in every relevant placeholder. Only keep the files that apply to me; delete the ones that don't.

## How to run this process

1. **Ask one question at a time.** Wait for my answer before moving on. Never bundle questions.
2. **Do not make assumptions.** If I haven't told you something, ask. Do not invent.
3. **Cover, in this order:**
   - (a) who I am — name, role, employer, team, scope, location, work pattern
   - (b) family and personal context
   - (c) my organisation — leadership, direct reports, who I report to, close peers
   - (d) businesses, products, or portfolio I touch
   - (e) my active priorities right now
   - (f) external relationships — vendors, advisors, partners, agencies
   - (g) tools I use day to day
   - (h) acronyms and shorthand
   - (i) voice rules — UK or US English, formatting preferences, words to avoid, opening and closing styles I dislike
   - (j) working style — how I want you to push back, when to ask questions, what blind spots to catch
4. **Ask before pulling from other sources.** If I have connected tools in Cowork (Gmail, Calendar, Drive, Slack, Notion, a CRM, Fathom) or you can see prior sessions, ask whether I want you to pull from them. Do not pull without permission. Summarise what you found before adding anything to memory.
5. **Write as you go.** When I finish a section, write the relevant file straight away. Do not batch all the writing to the end. Stamp dated files (`current-priorities.md`) with today's date.
6. **Update the rest of the template too.** As the answers come in: fill the placeholders in `CLAUDE.md` (company name, my name, top priority, tools); update `.claude/rules/communication-style.md` with my voice rules; add any recurring workflows I mention to `.claude/skills-backlog.md`; create a folder under `projects/` for each active workstream, each with a short README (status, dates, key context).

## After all files are written

7. **Verification pass.** List the final folder structure. Check for contradictions across files. Prove the writing matches my stated voice rules (for example, if I said no em dashes, show there are none). Flag anything still left as a placeholder.
8. **Profile entry.** Write me a tight Profile entry of around 200 words that I can paste straight into Claude's Settings → Profile field. It should be a personal-layer summary distilled from `CLAUDE.md`, not a copy of it. Cover: who I am, my role, my team, how I want you to communicate with me, my voice rules, and the blind spots I've asked you to catch. Skip the deep team and project detail (that lives in `memory/` and loads when this folder is attached). The Profile block needs to make you useful to me even in personal chats where this folder isn't attached.
9. **Set up my morning plan.** Run "draft my morning plan" once now so I can see it work against the memory you just wrote. Then walk me through making it recurring: in this project, open **Scheduled Tasks**, add a task, and paste the prompt from `templates/morning-plan-prompt.md`, set to run on weekday mornings. Offer to adjust the prompt to my routine first.
10. **Three closing reminders.** Tell me: (1) how to confirm the memory loads at the start of each future session (it loads automatically when this folder is the active Cowork project); (2) when I should ask you to update memory mid-task; (3) how often to run a consolidation pass.

## Posture

Be direct. Push back if my answer is vague or contradicts something I said earlier. This memory will drive how you work with me for months, so getting it right matters more than getting through the questions quickly.

Start with question one: my name, role, employer, and a one-paragraph description of my remit.
