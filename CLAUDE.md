
## Project Overview
Phase III: Todo AI Chatbot — Basic Level Functionality

Objective: Create an AI-powered chatbot interface for managing todos through natural language using MCP (Model Context Protocol) server architecture and using Claude Code and Spec-Kit Plus.

Development Approach: Use the Agentic Dev Stack workflow: Write spec → Generate plan → Break into tasks → Implement via Claude Code. No manual coding allowed.

Technology Stack
- Frontend: OpenAI ChatKit
- Backend: Python FastAPI
- AI Framework: OpenAI Agents SDK
- MCP Server: Official MCP SDK
- ORM: SQLModel
- Database: Neon Serverless PostgreSQL
- Authentication: Better Auth

Requirements (Basic Level)
- Implement conversational interface for all Basic Level features
- Use OpenAI Agents SDK for AI logic
- Build MCP server with Official MCP SDK that exposes task operations as tools
- Stateless chat endpoint that persists conversation state to database
- AI agents use MCP tools to manage tasks; MCP tools are stateless and persist to DB

Spec files to review:
- /specs/overview.md
- /specs/api/rest-endpoints.md
- /specs/database/schema.md
- /specs/features/authentication.md
- /specs/features/task-crud.md

Commands
- Frontend: cd frontend && npm run dev
- Backend: cd backend && uvicorn main:app --reload
