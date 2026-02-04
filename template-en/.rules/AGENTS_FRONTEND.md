# AGENTS_FRONTEND.md (Frontend Rulebook)

Version: v1.0
Effective Date: YYYY-MM-DD
Applies to: Frontend code and UI interaction changes

## 1. Scope
All changes to `.tsx`, `.ts`, `.css`, `DESIGN_TOKENS`, and UI interaction logic.

## 2. MUST
- **Component layering**: Follow the agreed component layering/atomic rules; no cross-layer imports.
- **Semantic tokens**: Colors/spacing/typography must use design tokens or CSS variables.
- **i18n first**: All copy must go through i18n (e.g., `t()`). If i18n is not available, record as TODO.
- **Functional components**: Components must be functional; avoid class components.
- **Data layer isolation**: No direct `fetch`/`axios` calls inside components; use `hooks` or `services`.
- **Defensive programming**: Validate API responses (e.g., Zod or project standard).

## 3. MUST NOT
- Do not hardcode color values (e.g., `#FFF`).
- Do not use `px` for spacing without justification (except 1px borders or fixed-size icons).
- Do not change backend API contracts directly for UI needs.

## 4. EXCEPTION
- `px` is only allowed for `1px/0.5px` borders or fixed-size icons and must be annotated with `// token-exception: reason`.
- Temporary debugging may use `console.log`, but it must be removed before commit.

## 5. ENFORCEMENT
- If hardcoded colors, missing i18n, or cross-layer imports are found, the change must be rejected and rolled back.
