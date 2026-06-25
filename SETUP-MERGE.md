# Merge Prompt — for an existing memory system

Use this **instead of** `SETUP-INTERVIEW.md` if you already built a memory system (a `CLAUDE.md` plus a `memory/` folder) from the bootstrap prompt. You don't need to rebuild any of that. This adds the functionality on top: skills, a decision log, a projects folder, references, templates, and a morning-plan scheduled task.

## Before you paste

1. Stay in your **existing** Cowork project (the one that already has your `CLAUDE.md` and `memory/`).
2. Put this template where Cowork can read it: unzip it and drop the folder inside your project (for example a subfolder called `ai-second-brain-template/`), or save it right next to your project folder.
3. Note the folder name. You'll tell the prompt where it is.

Then paste everything below the line into the chat.

---

I already have a working second brain in this project: a `CLAUDE.md` and a `memory/` folder I built earlier. I've placed the AI Second Brain template in a folder called `{{TEMPLATE_FOLDER_NAME}}` (ask me if you can't find it). I want to merge the template's **functionality** into my setup without touching my existing memory.

Work in this order and do not write anything until step 4.

1. **Read what I already have.** List my actual `memory/` tree and read my `CLAUDE.md`. Note my real file names: they may differ from the template's (for example my external contacts file might be named differently). Everything you wire up later must point at my real names, not the template's.

2. **Read what the template adds.** Look in `{{TEMPLATE_FOLDER_NAME}}` and identify everything **outside** `memory/`:
   - `.claude/skills/` and `.claude/skills-backlog.md`
   - `.claude/rules/communication-style.md`
   - `decisions/log.md`
   - `projects/` (workstream folders with READMEs)
   - `references/` (sops, examples), `templates/`, `archives/`

3. **Plan the merge and show it to me.** Before writing, show me:
   - Which folders and files you'll copy in.
   - The exact additions you'll make to my `CLAUDE.md` (Skills, Decision Log, Projects, References, Archives sections, and a Tool Integrations table), pointing at my real `memory/` file names.
   - Any conflicts you found.
   Wait for my approval.

4. **Apply the merge.** On my approval:
   - Copy in everything outside `memory/`. **Never overwrite or edit my `memory/` files.** If a file would collide, stop and ask.
   - Add the new sections to my `CLAUDE.md`. Keep it short; point into folders rather than inlining detail.
   - Delete the leftover `{{TEMPLATE_FOLDER_NAME}}` folder only after I confirm the copy looks right.

## Two decisions to apply during the merge

- **Voice rules.** I keep my voice and working style in `memory/preferences.md`. Point my `CLAUDE.md` Rules section at `memory/preferences.md`. Do **not** add the template's separate `.claude/rules/communication-style.md` unless I say I want it. (If I say I'd rather use the rule file, do the reverse and fold my voice into it.)
- **Projects.** Active workstreams live in the root `projects/` folder, one folder per workstream with a README. If I have a `memory/projects/` folder from my bootstrap run, ask whether to migrate those into root `projects/` so there's only one project home.

## After the merge

5. **Set up my morning plan.** Run "draft my morning plan" once so I can see it work against my memory. Then walk me through making it recurring: in this project, open **Scheduled Tasks**, add a task, and paste the prompt from `templates/morning-plan-prompt.md`, set to run on weekday mornings. Offer to tune the prompt to my routine first.

6. **Verification pass.** List the final structure. Confirm my `memory/` files are untouched, the new `CLAUDE.md` pointers all resolve to files that actually exist, and there are no leftover template placeholders (`{{LIKE_THIS}}`) in anything you copied in. Flag anything I still need to decide.

## Posture

Be direct. The one rule you must not break: do not modify my existing `memory/` files. If anything is ambiguous, ask before writing. Start by reading my current setup and the template folder, then show me the plan.
