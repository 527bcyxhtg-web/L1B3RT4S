# AGENTS.md

## Cursor Cloud specific instructions

This is a **static content repository** (L1B3RT45 / Libertas) containing markdown (`.mkd`) and JSON files. There is no source code, no build system, no dependencies, and no runnable application.

### Repository structure

- `*.mkd` files: AI model system prompt documentation (Anthropic, OpenAI, Google, Meta, xAI, DeepSeek, Mistral, etc.)
- `!SHORTCUTS.json`, `*SPECIAL_TOKENS.json`: structured reference data
- `.vscode/launch.json`: references a non-existent `main.ts` — this is a dead config, ignore it
- `LICENSE`: AGPL-3.0

### Development notes

- **No dependencies to install** — no `package.json`, `requirements.txt`, or any other manifest exists.
- **No lint, test, or build commands** — standard dev-workflow commands are not applicable.
- **Validation**: JSON files can be validated with `python3 -c "import json; json.load(open('FILENAME'))"`.
- Contributions consist of editing/adding `.mkd` or `.json` content files.
