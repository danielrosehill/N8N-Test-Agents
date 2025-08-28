# N8N-Test-Agents

A collection of AI agent system prompts designed to test various MCP (Model Context Protocol) tools with N8N workflows.

## Agent Index

| Agent | MCP Tool | Function Tested | Description |
|-------|----------|----------------|-------------|
| [![Email Sending](https://img.shields.io/badge/Email-Sending-blue?style=flat-square)](./email-mcp/sending/system-prompt.md) | Email MCP | Send emails | Tests email composition and sending functionality to Hannah about Netflix recommendations |
| [![Email Retrieval](https://img.shields.io/badge/Email-Retrieval-lightblue?style=flat-square)](./email-mcp/retrieval/system-prompt.md) | Email MCP | Retrieve/search emails | Tests inbox search, filtering, and email organization capabilities |
| [![Calendar](https://img.shields.io/badge/Calendar-Management-green?style=flat-square)](./calendar-mcp/system-prompt.md) | Calendar MCP | Event management | Tests calendar event creation, scheduling, and meeting coordination |
| [![Google Contacts](https://img.shields.io/badge/Google-Contacts-orange?style=flat-square)](./google-contact-mcp/system-prompt.md) | Google Contacts MCP | Contact management | Tests adding, updating, and organizing contact information |
| [![Google Docs](https://img.shields.io/badge/Google-Docs-red?style=flat-square)](./google-doc-mcp/system-prompt.md) | Google Docs MCP | Document operations | Tests document creation, editing, formatting, and sharing |
| [![Google Drive](https://img.shields.io/badge/Google-Drive-yellow?style=flat-square)](./google-drive-mcp/system-prompt.md) | Google Drive MCP | File management | Tests file upload, organization, folder creation, and sharing |
| [![Notion Docs](https://img.shields.io/badge/Notion-Docs-black?style=flat-square)](./notion-doc-mcp/system-prompt.md) | Notion MCP | Knowledge management | Tests Notion page creation, database management, and workspace organization |
| [![Task Management](https://img.shields.io/badge/Task-Management-purple?style=flat-square)](./task-mcp/system-prompt.md) | Task MCP | Productivity workflows | Tests task creation, status updates, project organization, and deadline tracking |

## Usage

Each agent folder contains a `system-prompt.md` file that defines:
- The agent's role and personality
- Specific task instructions for Daniel
- Expected tool execution patterns
- Output formatting templates
- Confirmation requirements

## Testing Structure

### Email MCP Functions
- **Sending** (`/email-mcp/sending/`) - Outbound email composition and delivery
- **Retrieval** (`/email-mcp/retrieval/`) - Inbox search and email organization

### Other MCP Tools
Each remaining tool focuses on its primary function set:
- **Calendar** - Event scheduling and management
- **Contacts** - Contact database operations
- **Docs** - Document creation and editing
- **Drive** - File storage and organization
- **Notion** - Knowledge base management
- **Tasks** - Productivity and project tracking

## Integration with N8N

These system prompts are designed to work with N8N workflows that:
1. Load the appropriate system prompt
2. Connect to the corresponding MCP server
3. Execute tool functions based on user input
4. Provide structured feedback and confirmations
