## Cursor Cloud specific instructions

This is a **content-only documentation repository** (L1B3RT4S). It contains curated AI system prompts (`.mkd` files), a glitch-token catalog (`*SPECIAL_TOKENS.json`), and a shortcuts reference (`!SHORTCUTS.json`). There is no source code, no package manager, no build step, no test suite, and no runnable application.

### Key facts

- **No dependencies to install.** No `package.json`, `requirements.txt`, or equivalent exists.
- **No services to run.** The repo is pure static content (Markdown + JSON).
- **No lint / test / build commands.** Validate JSON files with `python3 -c "import json; json.load(open('*SPECIAL_TOKENS.json'))"` and `python3 -c "import json; json.load(open('!SHORTCUTS.json'))"` as a sanity check.
- The `.vscode/launch.json` references a Deno runtime and `main.ts`, but that file does not exist — treat this as a stale artifact.
- File naming uses special characters (`*`, `!`, `-`) — quote paths when using shell commands.
