# GitHub Copilot instructions

Before changing code, read the repository's `AGENTS.md` and the most specific `AGENTS.md` files for the paths you touch. Those files are the source of truth for Sentry conventions.

- Keep changes narrow and tied to the assigned task. Do not refactor unrelated code.
- For backend work, use the repository's `.venv` and run the smallest relevant pytest file or node IDs. Do not run an unscoped full test suite.
- Run the relevant `prek` hooks for changed files. Follow the exact commands in `AGENTS.md`.
- For frontend work, use the documented `pnpm` commands in `AGENTS.md`; do not invoke `tsc` directly.
- Do not include real customer identifiers or data in code, tests, commits, or pull requests.
- Report the files changed, the validation commands run, and any commands that could not run. Never claim a test passed unless it ran successfully.
