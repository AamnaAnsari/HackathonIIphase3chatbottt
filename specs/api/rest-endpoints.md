# REST API Endpoints (Phase-3)
## Base URL: http://localhost:8000
## Auth: Bearer <token>

Note: Core REST endpoints are preserved for backward compatibility. AI agents interact with MCP tools, but the REST API remains available for direct calls and operational tooling.

## Task Endpoints (preserved)
- GET /api/{user_id}/tasks
- POST /api/{user_id}/tasks
- GET /api/{user_id}/tasks/{id}
- PUT /api/{user_id}/tasks/{id}
- DELETE /api/{user_id}/tasks/{id}

## Conversation / Message Endpoints (optional admin/inspection)
- GET /api/{user_id}/conversations
- GET /api/conversations/{id}/messages

## MCP Server (tools exposed to agents)
The MCP server exposes task-related operations as tools (not REST):
- create_task(user_id, title, description)
- list_tasks(user_id, filter)
- update_task(task_id, changes)
- delete_task(task_id)
- create_conversation(user_id)
- append_message(conversation_id, role, content)

