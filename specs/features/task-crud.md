# Feature: Task CRUD Operations (Phase-3)
## User Stories
- As a user, I can create, view, update, delete tasks via natural language conversation with the AI assistant.
- As a user, I can ask the assistant to list, filter, and search my tasks.

## Acceptance Criteria
- Title required (1-200 chars)
- Only show tasks for current user (JWT Auth required)
- All task operations performed by AI agents must go through MCP tools; direct DB writes by agents are forbidden.

## Agent Interaction
- Agents use MCP tools: `create_task`, `list_tasks`, `update_task`, `delete_task`.
- Agents must create or bind a `conversation` and append `messages` for each turn.
