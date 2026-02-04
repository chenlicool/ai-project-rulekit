# Project Rules Initialization Workflow (0 -> 1)

When starting from zero, complete the rule system before writing code.

## Phase 0: No stack files yet
1. Establish the rule system:
   - `AGENTS.md`
   - All rulebooks under `.rules/`
   - `MEMORY.md` / `ARCHITECTURE.md` / `README.md` / `API.md` / `CHANGELOG.md`
2. Fill `STACK.md` to define the planned stack and deployment.
3. Initialize `CHANGELOG.md` version to `0.0.1`.

## Phase 1: After scaffolding
1. Scan project structure and stack files (e.g., `package.json`).
2. Align version numbers with `CHANGELOG.md`.
3. Verify `STACK.md` plan matches the actual stack.

## After initialization
- All subsequent tasks must follow the forced flow: Impact Analysis → MEMORY → Changes.
