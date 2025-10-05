# smarrttask.ai
An Agentic AI system that autonomously plans, executes, and reports daily tasks using reasoning, memory, and web search.

## 🧠 Overview  
This is an open-source project that demonstrates the core principles of **Agentic AI** — autonomous systems capable of reasoning, planning, executing, and improving through feedback.  

This project was created as part of the **SMARTTASK.AI initiative**, aiming to make agentic intelligence accessible to everyone through simple, modular, and transparent design.  

Agentic TaskFlow takes a high-level human goal (like _“Summarize today’s AI news and draft a LinkedIn post”_) and breaks it down into actionable subtasks.  
The system then plans, executes, and stores its reasoning process using a lightweight memory module.  

The goal is to show how **AI agents can perform multi-step reasoning, web interaction, and self-tracking — all without human micromanagement.**

---

## ⚙️ Features  

✅ **Goal-Oriented Planning:** Converts natural language goals into structured action plans.  
✅ **Autonomous Execution:** Runs subtasks automatically (e.g., search → summarize → generate output).  
✅ **Memory and Reflection:** Saves previous results and context for continuous improvement.  
✅ **Tool Integration:** Modular tools for web search, summarization, and text generation.  
✅ **Extensible Framework:** Easily add new tools or memory backends (SQLite, VectorDB, etc.).  
✅ **Optional Streamlit UI:** Launch a simple dashboard to run and visualize agent tasks.  

---

## 🧩 Architecture  

```text
+------------------------+
|      User Goal         |
+------------------------+
            |
            v
+------------------------+
|       Planner          |  --> Breaks down goal into subtasks
+------------------------+
            |
            v
+------------------------+
|       Executor         |  --> Calls tools & collects results
+------------------------+
            |
            v
+------------------------+
|        Memory          |  --> Stores reasoning, tasks, outputs
+------------------------+
            |
            v
+------------------------+
|        Reporter        |  --> Summarizes task progress/output
+------------------------+
