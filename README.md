# 🤖 n8n AI Agent Workflows

This repository contains **n8n workflows** for building and experimenting with **AI-powered automations** using [n8n](https://n8n.io/).

---

## 🧩 Workflow: Basic Agent Example

**File:** `Basic Agent Example.json`  
**Category:** AI Agent / Automation  
**Status:** ✅ Working Example  

### 📘 Overview

The **Basic Agent Example** demonstrates how to create a simple **AI Agent** inside n8n that can process user input, perform reasoning with an LLM (like OpenAI), and use built-in tools such as a calculator.

This workflow showcases how to chain together multiple n8n nodes to create an intelligent automation.

---

### 🧠 Components Used

| Node | Purpose |
|------|----------|
| 🗣 **Chat Input** | Captures user messages and passes them to the agent |
| 🤖 **AI Agent** | Orchestrates the logic, memory, and tool use |
| 🧩 **OpenAI Chat Model** | Generates intelligent natural language responses |
| 💾 **Simple Memory** | Stores short-term context between messages |
| 🔢 **Calculator** | Handles basic math operations |

---

### ⚙️ How It Works

1. **User inputs text** (e.g., “What is 2 + 2?”) via the **Chat Input** node  
2. The message is passed to the **AI Agent**, which routes the task  
3. The **OpenAI Chat Model** interprets the query and decides whether to use a tool  
4. The **Calculator** node performs the arithmetic if required  
5. The final response (e.g., “2 + 2 is 4.”) is returned to the user  

---

### 💬 Example Interaction

| Input | Output |
|--------|---------|
| `2 + 2` | `2 + 2 is 4.` |
| `What is 12 * 3?` | `12 * 3 is 36.` |
| `Hello!` | `Hi there! How can I help you today?` |

---

### 🧰 Requirements

Before importing and running this workflow:
- [n8n](https://n8n.io/) installed locally or hosted (e.g., [n8n.cloud](https://n8n.cloud))
- OpenAI API key added in your n8n credentials
- Internet connection (for LLM API calls)

---

### 🚀 How to Import

1. Open your n8n instance (e.g. [http://localhost:5678](http://localhost:5678))
2. Go to **Workflows → Import → Upload**
3. Select the file:  
