# General AI Development Rulekit 0-1 Starter Pack (Template Set) Guide

This template set establishes a shared rule system at project start so AI and humans stay aligned.

## Directory Structure
```text
template-en/
├── AGENTS.md
├── ARCHITECTURE.md
├── API.md
├── CHANGELOG.md
├── MEMORY.md
├── README.md
├── STACK.md
├── TEMPLATE_GUIDE.md
├── .rules/
│   ├── AGENTS_BACKEND.md
│   ├── AGENTS_DOCS.md
│   ├── AGENTS_FRONTEND.md
│   └── AGENTS_TEST.md
└── WORKFLOWS/
    ├── INIT.md
    └── SYNC.md
```

## Usage
1. Copy this template set into your new project root.
2. Fill `STACK.md` to define the planned stack.
3. Follow `WORKFLOWS/INIT.md` to complete initialization.
4. All changes must comply with `AGENTS.md` + `.rules/`.

## Hard Constraints
- Keep all fixed H1 headings; do not remove or rename.
- Only append content under existing headings; no full rewrites.
- `MEMORY.md` must be maintained in reverse chronological order with newest first.
- For projects without a backend, replace `API.md` content with "Internal Protocol / Component Communication".

## Placeholders
- `{{PROJECT_NAME}}`: project name
- `YYYY-MM-DD` / `YYYY-MM-DD HH:MM`: actual date/time
