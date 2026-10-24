# Instructions for coding agents

## Git commits

- Commit as the human collaborator who is running you. Use the existing local `git config user.name` and `user.email`. Never set the author or committer to Codex or any other agent identity (no `--author`, no `-c user.name=...`).
- End every commit message with a blank line and then this trailer:

  ```
  Co-authored-by: Codex <codex@users.noreply.github.com>
  ```

- If `git config user.email` is not set, stop and ask the user to set it to the email linked to their GitHub account before committing.
