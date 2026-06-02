# Install Checklist

The install is good only if every item below passes.

## GOG

- [ ] `gog auth list` shows the correct operating account
- [ ] Gmail *message search* works
- [ ] Calendar list / read works
- [ ] Sheets metadata read works
- [ ] Google Docs read works if meeting-notes ingestion is enabled

## Skills

- [ ] `executive-assistant` is installed in `~/.hermes/skills/`
- [ ] `business-development` is installed in `~/.hermes/skills/`
- [ ] `daily-task-manager` is installed in `~/.hermes/skills/`
- [ ] `daily-task-prep` is installed in `~/.hermes/skills/`

## Workspace

- [ ] `hermes-exec/priority-map.md` is installed
- [ ] `hermes-exec/auto-resolver.md` is installed
- [ ] `hermes-exec/meeting-notes.md` is installed
- [ ] `hermes-exec/tasks.md` is installed
- [ ] `hermes-exec/tasks-completed.md` is installed
- [ ] `workspace/HEARTBEAT.md` is installed
- [ ] `workspace/TOOLS.md` is installed
- [ ] `workspace/memory/meeting-notes-state.json` is installed
- [ ] private workspace files have been authored if your setup depends on them
- [ ] all placeholders are replaced

## Behavior

- [ ] heartbeat reads the source-of-truth files instead of duplicating workflow logic
- [ ] proactive updates route to the intended channel + target
- [ ] inbox sweeps use *message-level* Gmail search
- [ ] scheduling checks all relevant calendars before booking
- [ ] the task system uses `hermes-exec/tasks.md` as the live source of truth
- [ ] prior-day completed tasks archive into `hermes-exec/tasks-completed.md`
- [ ] meeting notes are treated as a live signal source if enabled
- [ ] business-development work treats the outreach sheet as the live source of truth
- [ ] daily task prep promotes due-today items into `## Today`

## Cron

- [ ] executive assistant sweep exists
- [ ] daily task prep exists
- [ ] daily business-development sourcing exists
- [ ] optional nightly backup is configured only if desired
- [ ] optional self-update is enabled only if explicitly desired

If any box is unchecked, the install is not done.
