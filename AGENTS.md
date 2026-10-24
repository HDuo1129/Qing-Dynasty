# Instructions for AI agents

This file is the shared memory for every AI tool used on this project (Codex, Claude, and others) by Dong, Jianhao, and Duo. Read it at the start of every session.

## Shared memory: update after every session

- Before you finish any session that changed or decided something, update the **Project memory** section below and commit it together with your other changes.
- Record what a teammate or another AI would need next time: decisions on sample, variables and identification, data sources and their status, file locations, open questions, and who is working on what.
- Write each entry as one line: `- YYYY-MM-DD (name): what was done or decided`. Use the name of the human collaborator you are working with.
- Keep it short. Do not paste code, logs or long reasoning. Edit or remove entries that are no longer true instead of piling up new ones. Longer decisions go in `docs/decisions/` and can be linked from here.
- Always `git pull --ff-only` before editing this file so you do not overwrite a teammate's entries.

## Git commits

- Commit as the human collaborator who is running you. Use the existing local `git config user.name` and `user.email`. Never set the author or committer to an AI identity (no `--author`, no `-c user.name=...`).
- End every commit message with a blank line and a co-author trailer for the AI you are, for example:

  ```
  Co-authored-by: Codex <codex@users.noreply.github.com>
  ```

- If `git config user.email` is not set, stop and ask the user to set it to the email linked to their GitHub account before committing.

## Project memory

- 2026-10-24 (Duo): Commits must be authored by the human collaborator, with the AI as co-author. Every AI session updates this section so all three of us share the same context.
- 2026-10-24 (Duo): Dong is not yet listed as a contributor because his Codex commits were authored as `Codex`. Reminder and steps are in README and `docs/project_notes/todo.md`. The three earlier Codex-authored commits are left as they are (no history rewrite).
- 2026-10-24 (Duo): `CLAUDE.md` only imports this file, so Claude and Codex share one memory. Saying "更新 AGENTS.md" at the end of a session is the agreed cue for the AI to update this section.
