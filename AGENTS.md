# AGENTS.md

## Cursor Cloud specific instructions

This is a **static content repository** (L1B3RT45 / Libertas). It contains curated AI system prompts (`.mkd` files), a glitch-token catalog (`*SPECIAL_TOKENS.json`), and a shortcuts reference (`!SHORTCUTS.json`). There is no source code, no package manager, no build step, no test suite, and no runnable application.

### Key facts

- **No dependencies to install.** No `package.json`, `requirements.txt`, or equivalent exists.
- **No services to run.** The repo is pure static content (Markdown + JSON).
- **No lint / test / build commands.** Validate JSON with:

  ```bash
  python3 -c "import json; json.load(open('!SHORTCUTS.json'))"
  python3 -c "import json; json.load(open('*SPECIAL_TOKENS.json'))"
  ```

- `.vscode/launch.json` references Deno and `main.ts`, but that file does not exist — treat it as a stale artifact.
- File naming uses special characters (`*`, `!`, `-`) — quote paths when using shell commands.
- `LICENSE`: AGPL-3.0

### Contributions

Edits and additions are made to `.mkd` or `.json` content files.
