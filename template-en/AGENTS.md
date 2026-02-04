# AGENTS.md (Master Rules)

Version: v1.0
Effective Date: YYYY-MM-DD
Applies to: All AI coding / refactoring / documentation work

## 1. Scope
These rules apply to {{PROJECT_NAME}} and all subprojects/subdirectories.

## 2. MUST
1. Do not modify files or services marked Protected unless explicitly authorized.
2. Before any substantive change, complete Impact Analysis and update `MEMORY.md`.
3. If rules conflict, follow the stricter rule; sub-rules may not loosen the master rules.
4. New features must follow an "atomic decomposition" approach (smallest units first, then compose).
5. Uncertain information must be labeled "TBD/Unknown".

## 3. MUST NOT
1. Do not rewrite entire documents; apply minimal patches only.
2. Do not change architecture without reviewing `ARCHITECTURE.md`.
3. Changing code before updating required docs is a violation.

## 4. Rule Index
- Frontend rules → `.rules/AGENTS_FRONTEND.md`
- Backend rules → `.rules/AGENTS_BACKEND.md`
- Test rules → `.rules/AGENTS_TEST.md`
- Docs rules → `.rules/AGENTS_DOCS.md`

## 5. Enforcement Flow
1. Impact Analysis
2. Update `ARCHITECTURE.md` / `API.md` / `README.md` as needed
3. Make code changes
4. Update `MEMORY.md` / `CHANGELOG.md`
