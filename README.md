# Agentic AI Deep Research System

An autonomous multi-agent AI research workflow that plans search strategies, performs parallel web research, synthesizes findings into detailed reports, and generates structured outputs using modern agent orchestration, async execution, tool calling, and LLM-powered workflows.

---

# Overview

The Agentic AI Deep Research System is a production-style multi-agent AI workflow designed to simulate how modern AI systems collaboratively perform deep research tasks autonomously.

Instead of relying on a single chatbot response, the system decomposes the research pipeline into multiple specialized AI agents responsible for:

- Research planning
- Search orchestration
- Parallel information retrieval
- Research synthesis
- Long-form report generation
- Structured output generation

The project demonstrates how modern agentic AI architectures can orchestrate multiple collaborating agents to autonomously execute complex research workflows using tool calling, async execution, and structured outputs.

---

# System Architecture

<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/f56829b8-31a9-43ce-bf3e-5ddec93ab1e9" />



---

# Workflow Explanation

## Step 1 — User Query

The workflow begins when the user submits a research topic or question.

Example:

```text
"Best companies building agentic AI systems"
```

---

## Step 2 — Planner Agent

The Planner Agent analyzes the query and strategically determines:

- what searches should be performed
- why each search matters
- how to structure the research process

Instead of hardcoded search queries, the system dynamically generates intelligent search strategies using LLM reasoning and structured outputs.

Example generated search plan:

```json
{
  "searches": [
    {
      "reason": "Identify major companies building agentic AI systems",
      "query": "top companies building agentic AI platforms"
    },
    {
      "reason": "Compare enterprise AI orchestration solutions",
      "query": "enterprise AI agent orchestration companies"
    }
  ]
}
```

---

## Step 3 — Parallel Search Agents

Multiple search tasks are executed concurrently using Python async workflows.

Each Search Agent:

- performs web retrieval
- searches external sources
- summarizes findings
- returns structured outputs

The system uses concurrent execution to improve:

- speed
- scalability
- workflow efficiency

---

## Step 4 — Research Synthesis

All retrieved information is aggregated and combined into a unified research context.

The workflow merges:

- search findings
- extracted summaries
- relevant sources
- contextual insights

before generating the final report.

---

## Step 5 — Writer Agent

The Writer Agent synthesizes all retrieved research into:

- detailed markdown reports
- structured summaries
- follow-up research suggestions

The workflow generates research-style outputs instead of short chatbot responses.

---

# Key Features

- Multi-agent orchestration
- Autonomous research planning
- Parallel async search execution
- Structured outputs using Pydantic
- Long-form markdown report generation
- OpenAI Hosted WebSearchTool integration
- Tool-calling workflows
- Modular AI pipeline architecture
- Production-style AI orchestration patterns
- Concurrent workflow execution using AsyncIO

---

# Tech Stack

## AI / LLM Infrastructure

- OpenAI Agents SDK
- GPT-4o / GPT-4o-mini
- DeepSeek Integration
- OpenAI Hosted Tools

## Backend & Workflow

- Python
- AsyncIO
- Pydantic
- Structured Outputs
- Tool Calling
- Async Orchestration

## UI / Interface

- Gradio

---

# Async Workflow Execution

The workflow uses Python async orchestration to execute multiple searches simultaneously.

## Traditional Sequential Workflow

```text
Search 1 → wait
Search 2 → wait
Search 3 → wait
```

## Async Parallel Workflow

```text
Search 1
Search 2
Search 3
↓
Run concurrently
```

This significantly improves:

- scalability
- latency
- workflow efficiency

---

# Structured Outputs

The project uses Pydantic schemas to enforce structured, machine-readable outputs.

Example:

```python
class WebSearchItem(BaseModel):
    reason: str
    query: str
```

This enables:

- reliable downstream automation
- cleaner orchestration
- production-grade workflow pipelines

---

# Multi-Agent Architecture

The workflow demonstrates how specialized AI agents can collaborate inside orchestrated pipelines.

## Planner Agent

Responsible for:

- query analysis
- research planning
- search strategy generation

---

## Search Agents

Responsible for:

- web retrieval
- summarization
- source gathering
- information extraction

---

## Writer Agent

Responsible for:

- report synthesis
- markdown generation
- long-form content creation
- follow-up recommendations

---

# Live Demo Screenshots

## Research Interface

<img width="1344" height="339" alt="Screenshot 2026-05-20 at 8 03 08 PM" src="https://github.com/user-attachments/assets/4668e2eb-2076-4015-a90e-779249852c69" />


---

## Generated Research Report

<img width="1358" height="767" alt="Screenshot 2026-05-20 at 8 05 31 PM" src="https://github.com/user-attachments/assets/7178a0ee-76cf-4e81-a956-5277a37e46dd" />

---
<img width="1462" height="813" alt="Screenshot 2026-05-20 at 8 05 51 PM" src="https://github.com/user-attachments/assets/c6e1f23b-47b1-4918-ac66-bd1f779ba361" />

---

# Concepts Demonstrated

This project demonstrates:

- Agentic AI Systems
- Multi-Agent Collaboration
- Async AI Workflows
- Structured Outputs
- Tool Calling
- AI Orchestration
- Autonomous Pipelines
- AI Workflow Decomposition
- Production-Style AI Engineering
- Concurrent Execution Architectures

---

# Future Improvements

Potential future enhancements include:

- Retrieval-Augmented Generation (RAG)
- Vector Database Integration
- Persistent Agent Memory
- Human-in-the-Loop Approvals
- Multi-Model Routing
- Citation Verification
- PDF / DOCX Export
- Autonomous Research Loops
- Enterprise Knowledge Base Integration

---

# Why This Project Matters

Modern AI systems are rapidly evolving beyond simple chatbot interactions.

This project explores how:

- specialized AI agents
- orchestration workflows
- structured reasoning
- async execution
- and external tools

can be combined into scalable autonomous AI systems capable of executing real-world research tasks.

The workflow reflects emerging patterns increasingly used in:

- AI copilots
- autonomous workflows
- enterprise AI systems
- orchestration platforms
- modern LLM applications

---

# Connect

- LinkedIn: https://www.linkedin.com/in/ruchikamotwani20/
- Portfolio: https://ruchika-motwani.notion.site/portfolio
- Email: ruchikamotwani20@utexas.edu

---

# License

This project is intended for educational and research purposes.
