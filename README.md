# Agentic_ai_trip_planner - ADK_Basic

# 🌍 Agentic AI Trip Planner using Google ADK

A multi-agent AI travel planning system built using **Google ADK (Agent Development Kit)** with support for:

* Sequential agent workflows
* Parallel agent execution
* Loop/refinement agents
* Routing agents
* Tool orchestration
* MCP integration
* Stateful memory
* Personalized conversational planning

This project demonstrates a production-style **Agentic AI architecture** where specialized agents collaborate to generate intelligent and personalized trip plans.

---

# 🚀 Features

## ✅ Multi-Agent Architecture

The system contains multiple specialized AI agents:

| Agent Type        | Purpose                                |
| ----------------- | -------------------------------------- |
| Single Agent      | Basic trip planning                    |
| Sequential Agents | Step-by-step coordinated workflows     |
| Parallel Agents   | Multiple agents working simultaneously |
| Loop Agents       | Iterative refinement and improvement   |
| Routing Agents    | Dynamic routing based on user intent   |
| Agent-as-Tool     | Agents invoking other agents/tools     |
| Memory Agents     | Personalized memory-enabled planning   |
| MCP Agents        | External tool integration              |

---

# 🧠 Built-in Memory System

The project supports conversational memory using the ADK Session Service.

The AI can remember:

* food preferences
* travel style
* budget
* preferred activities
* prior interactions

Example:

User:

```text
Remember that I prefer vegetarian food and low-budget trips.
```

Later:

```text
Plan a weekend trip for me.
```

The agent automatically personalizes the response using stored memory.

---

# 📂 Project Structure

```text
ADK_Basic/
│
├── a_single_agent/
├── b1_sequential_agent/
├── b2_parallel_agent/
├── b3_loop_agent/
├── b4_manual_sequential_flow/
├── c_custom_agent/
├── d_routing_agent/
├── e_agent_as_tool/
├── f_agent_with_memory/
├── g_agents_mcp/
├── mcp_tool_box/
│
├── requirements.txt
├── README.md
├── run.sh
├── setup_trip_database.py
├── setup_venv.sh
├── setup_venv.bat
```

---

# ⚙️ Installation & Setup

## 1️⃣ Clone Repository

```bash
git clone https://github.com/sreeadvaithi4/Agentic_AI_Trip_planner.git
cd Agentic_AI_Trip_planner
```

---

## 2️⃣ Create Virtual Environment

### Windows

```bash
python -m venv adk-env
adk-env\Scripts\activate
```

### Linux / Mac

```bash
python3 -m venv adk-env
source adk-env/bin/activate
```

---

## 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 4️⃣ Create `.env`

Create a `.env` file in the project root:

```env
GOOGLE_API_KEY=YOUR_API_KEY
GOOGLE_CLOUD_PROJECT=YOUR_PROJECT_ID
GOOGLE_CLOUD_LOCATION=us-central1
GOOGLE_GENAI_USE_VERTEXAI=False
```

---

# ▶️ Running the Project

## Run Memory Agent

```bash
python f_agent_with_memory/main.py
```

---

## Run MCP Agent

```bash
python g_agents_mcp/main.py
```

---

## Run Sequential Agent

```bash
python b1_sequential_agent/agents.py
```

---

# 💬 Example Prompts

## 🌴 Travel Planning

```text
Plan a relaxing day trip in San Francisco with museums and good food.
```

```text
Create a personalized beach vacation for me.
```

---

## 🍱 Food Preferences

```text
Remember that I prefer vegetarian food.
```

```text
Suggest restaurants for my preferences.
```

---

## 💰 Budget Planning

```text
Remember that I prefer low-budget trips.
```

```text
Plan a 2-day budget-friendly trip.
```

---

## 🎨 Personalized Interests

```text
I enjoy museums, hiking, and photography.
```

```text
Plan a trip based on my interests.
```

---

# 🧩 Technologies Used

* Python
* Google ADK
* Gemini API
* Vertex AI
* MCP Tools
* Session Memory
* Multi-Agent Workflows

---

# 🏗️ Architecture Overview

The system follows an Agentic AI orchestration model:

1. User query is received
2. Routing agent determines task type
3. Specialized agents are invoked
4. Memory system retrieves prior preferences
5. Tool agents gather additional information
6. Final personalized response is generated

---

# 🎯 Use Cases

* Intelligent travel planning
* Personalized recommendation systems
* Multi-agent orchestration research
* Conversational memory systems
* AI workflow experimentation
* Agentic AI demonstrations

---

# 📸 Demo

The project supports:

* CLI interaction
* Stateful conversations
* Persistent user sessions
* Dynamic agent routing

---

# 🔐 Security Note

Do NOT upload:

* `.env`
* API keys
* virtual environment folders

The repository already uses `.gitignore` to prevent sensitive files from being uploaded.

---

# 👨‍💻 Author

Developed by Sree Advaithi

GitHub:
https://github.com/sreeadvaithi4

---

# ⭐ Future Improvements

* Web UI using Streamlit/React
* Real-time map integration
* Flight and hotel APIs
* Voice-enabled planning
* Multi-user support
* Vector database memory
* Autonomous planning agents

