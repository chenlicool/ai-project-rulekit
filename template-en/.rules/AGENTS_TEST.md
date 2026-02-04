# AGENTS_TEST.md (Testing Rulebook)

Version: v1.0
Effective Date: YYYY-MM-DD
Applies to: All code submissions, feature validation, and bug fixes

## 1. Scope
Validation workflows, mock data definition, and test case writing for all project features.

## 2. MUST
- **AI audit**: AI-generated or AI-modified code is untrusted by default.
- **Mock first**: Define mock data before frontend development to avoid unstable backend dependencies.
- **Critical path coverage**: Core flows must have regression tests (manual or automated).
- **Component first**: Complex components must be validated in isolation first.

## 3. MUST NOT
- Do not merge code without passing tests.
- Do not use production data for development/testing.
- Do not ignore lint/compile errors.

## 4. EXCEPTION
- Pure visual styling tweaks may relax testing, but require manual review confirmation.

## 5. ENFORCEMENT
- AI changes that fail tests must not be merged.
- After each major change, output a test record:
  - Time: YYYY-MM-DD HH:MM
  - Command:
  - Coverage:
  - Result:
  - Exceptions: None / brief note
