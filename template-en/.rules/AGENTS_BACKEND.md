# AGENTS_BACKEND.md (Backend Rulebook)

Version: v1.0
Effective Date: YYYY-MM-DD
Applies to: Backend services and API changes

## 1. Scope
All changes to `.ts`, `.js`, `.json`, `.sql`, `.yaml` and API contract changes.

## 2. MUST
- **Contract isolation**: Do not modify published API inputs/outputs without formal process and doc updates.
- **Error code standard**: API responses must include clear business error codes; ambiguous `500` is not acceptable.
- **Localizable messages**: External errors should be keyed by `error_code`; `message` is supplemental and may be localized by frontend.
- **Logging trace**: Critical requests must carry a Request ID and be logged end-to-end.
- **Zero-trust input**: All inputs must be validated (Schema Validation).
- **Idempotency**: Create/charge/write operations must support idempotent retries.

## 3. MUST NOT
- Do not change backend API contracts just for frontend convenience.
- Do not log sensitive information in production (keys, passwords, tokens).
- Do not run irreversible DDL directly (must have a migration plan).

## 4. EXCEPTION
- Emergency hotfixes require owner approval and must record `FIX: request_id`.

## 5. ENFORCEMENT
- If a published API must change:
  1. Introduce a new version (v1 -> v2)
  2. Update `ARCHITECTURE.md`
  3. Record a changelog entry
  4. Notify frontend owner
