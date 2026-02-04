# AGENTS_DOCS.md (Documentation Rulebook)

Version: v1.0
Effective Date: YYYY-MM-DD
Applies to: Updates to all docs such as `MEMORY.md`, `ARCHITECTURE.md`, `README.md`, `API.md`, `CHANGELOG.md`

## 1. Scope
All document creation, updates, and patch outputs.

## 2. MUST
- **Template output order**: After any functional change, output in this order:
  1. Update `MEMORY.md` (include Impact Analysis and result, 8-line format)
  2. Minimal patch to `ARCHITECTURE.md` (as needed)
  3. Minimal patch to `README.md` / `API.md` (as needed)
  4. Minimal patch to `CHANGELOG.md` (as needed)
- **Impact timing**: Impact Analysis must be completed before code changes; it may be recorded in `MEMORY.md` afterward.
- **Minimal patch**: Do not rewrite whole documents; update only relevant sections.
- **English primary**: All documentation is written in English. If a translation is required, keep it in a separate file (e.g., `README.zh-CN.md`).
- **Single source of truth**: `ARCHITECTURE.md` is the architectural source of truth; code must follow the doc.
- **Ordering**: `MEMORY.md` must be kept in reverse chronological order with the newest entry on top.

## 3. Templates (MUST)
- **MEMORY.md format (8 lines)**:
  - Time / Goal / Changes / Current / Do Not Touch / TODO / Rollback / Constraints
- **Other docs**: Keep fixed H1 headings; do not remove or rename them.

## 4. MUST NOT
- Do not invent unknown information; mark uncertain items as "TBD/Unknown".
- Do not add speculative explanations or suggestions in patches.
- Do not skip doc updates; code changes without doc sync are a task failure.

## 5. EXCEPTION
- **Initial creation**: New projects or new docs may output the full document.

## 6. Versioning
- Tightened rules or new mandatory steps: bump Minor version (e.g., v1.1).
- Breaking existing processes or template structure: bump Major version (e.g., v2.0).
- Wording-only clarification that does not affect execution: no version bump required.
