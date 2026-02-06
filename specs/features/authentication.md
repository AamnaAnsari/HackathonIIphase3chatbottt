# Feature: Authentication (Phase-3)
## Stack
- Better Auth (Frontend)
## Flow
1. User logs in on Frontend -> Gets JWT from Better Auth
2. Frontend sends JWT in Header "Authorization: Bearer <token>"
3. Backend verifies JWT and extracts User ID

Notes: Authentication is unchanged from Phase-2. AI agents and MCP tools operate using the authenticated user_id; tools must validate the caller's user identity and enforce per-user data separation.
