# Contributing Guide

## Workflow
1. **Always** start from `main`. Fetch/Pull first.
2. Create a branch: `feature/<yourname>-<short-scope>`
   - Examples: `feature/kyle-map-oldtown`, `feature/jeremy-npc-sprites`
3. Communicate any major shared resources, files, etc. that you will be working on.
4. Commit small, focused changes with clear messages. Follow [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/#summary) format.
5. Push and open a Pull Request (PR). Fill the checklist.

## Pull Request Checklist
- [ ] Fetched latest `main` before starting
- [ ] Art/audio filenames are descriptive and lowercase
- [ ] Screenshots or short notes to help testers (optional)

## Map & DB Etiquette
- **Maps**: Try to have only one editor per `MapXXX.json` at a time.
- **Database** (`Actors.json`, `Classes.json`, etc.): Batch related changes in a single PR when possible.
- **Plugins**: Place JS in `js/plugins/`; enable/disable via RPG Maker’s Plugin Manager.

## Branch Protection (for maintainers)
- Protect `main`: require PRs, 1 approval, block force-pushes.
- Enable Git LFS (already configured via `.gitattributes`).
- Use Issues + Projects to assign tasks.

## Naming Conventions
- Files: kebab-case, descriptive (`inn-exterior.png`, `npc-bartender-01.png`)
- Audio: prefix type if helpful (`bgm-town-day.ogg`)
- Maps: keep default IDs, add a human name in an external doc or in-game notes.