## 🤖 n8n AI Agent Workflow — Gemini + Tools

A simple but powerful n8n AI agent workflow that uses **Google Gemini** as the LLM 
with built-in memory and three tools.

### Workflow Overview

**Trigger:** Chat message received  
**Agent:** AI Agent node (orchestrates all sub-components)

### Components

| Type | Node | Purpose |
|------|------|---------|
| 🧠 Model | Google Gemini Chat Model | Powers the agent's reasoning |
| 💾 Memory | Simple Memory | Retains conversation context |
| 🔍 Tool | Gemini Search Tool | Web search capability |
| 🕐 Tool | Date & Time | Fetches current date/time |
| 🧮 Tool | Calculator | Performs math operations |

### How It Works

1. A chat message is received via the **Chat Trigger** node  
2. The **AI Agent** processes it using Gemini as the LLM  
3. The agent decides which tools to call based on the query  
4. **Memory** keeps track of prior conversation turns  
5. The final response is returned to the user  

### Setup

- Requires an active **Google Gemini API key**
- Import the workflow JSON into n8n
- Connect your Gemini credentials
- Activate and test via the chat interface
