# memory/

The deep-context layer. `CLAUDE.md` at the repo root is the hot cache that loads every message; it points into these files for detail. Keep `CLAUDE.md` short and let depth live here.

```
memory/
  personal.md            <- who I am: role, employer, location, work pattern, family, north star
  preferences.md         <- voice and working style, blind spots to catch
  glossary.md            <- acronyms and shorthand
  goals.md               <- quarterly direction and targets
  current-priorities.md  <- ~30-day focus
  context/               <- one file per business unit or portfolio (company.md is the main one)
  people/                <- team.md, leadership.md, direct-reports.md
  external/relationships.md  <- vendors, partners, advisors, agencies
```

Only keep the files that apply. Delete the rest. Add files (e.g. another `context/` unit, a `people/` group) as the picture gets richer. Active workstreams stay in the root `projects/` folder; decisions stay in `decisions/log.md`.
