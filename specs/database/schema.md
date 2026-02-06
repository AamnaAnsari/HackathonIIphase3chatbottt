# Database Schema (Phase-3 additions)
## Tables
### users (Managed by Better Auth)

### tasks
- id: int (pk)
- user_id: string (indexed string, Better Auth ID)
- title: string
- description: string (optional)
- completed: boolean

### conversations
- id: int (pk)
- user_id: string (indexed)
- created_at: datetime
- updated_at: datetime

### messages
- id: int (pk)
- conversation_id: int (fk -> conversations.id)
- role: string ("user" | "assistant")
- content: text
- created_at: datetime

Notes: Conversation and Message tables store chat history for Phase-3 CUI. All state persisted to PostgreSQL (Neon).
