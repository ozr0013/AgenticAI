# AgenticAI

A personal learning repository for building AI agents from the ground up. This is where I work through the concepts, patterns, and frameworks behind agentic AI — one project at a time.

## Why this repo exists

I'm learning how to design and build AI agents: systems that can reason, plan, use tools, and act toward a goal rather than just responding to a single prompt. The plan is to move from fundamentals to working, non-trivial agents, and to keep everything I build (and break) here as I go.

## What "agentic AI" means here

An agent is more than a wrapper around an LLM call. The things I want to actually understand and implement:

- **Reasoning & planning** — breaking a goal into steps, deciding what to do next
- **Tool use** — letting a model call functions, APIs, search, code execution, etc.
- **Memory** — short-term context plus longer-term state across steps
- **Reflection & self-correction** — checking its own output and retrying
- **Multi-agent coordination** — several agents with roles working together
- **Evaluation** — measuring whether an agent actually did the task well

## Roadmap

- [ ] **Foundations** — LLM basics, prompting, structured output, function calling
- [ ] **Single-agent loop** — build a ReAct-style agent (reason → act → observe)
- [ ] **Tool integration** — web search, code execution, file/data access
- [ ] **Memory** — add short-term and persistent memory to an agent
- [ ] **Frameworks** — try LangChain / LangGraph, and compare against a from-scratch version
- [ ] **Multi-agent** — coordinate multiple agents on a shared task
- [ ] **Evaluation** — set up a benchmark to score agent runs
- [ ] **A real project** — ship one useful end-to-end agent

## Tech stack (planned)

- **Language:** Python
- **Models:** LLM APIs (Anthropic / OpenAI / local via Ollama)
- **Frameworks:** LangChain / LangGraph (and hand-rolled loops for learning)
- **Vector store:** ChromaDB / FAISS for retrieval and memory
- **Environment:** notebooks for experiments, scripts for real agents

## Getting started

```bash
# clone
git clone https://github.com/ozr0013/AgenticAI.git
cd AgenticAI

# set up a virtual environment
python -m venv .venv
source .venv/bin/activate        # Windows: .venv\Scripts\activate

# install dependencies (once requirements.txt exists)
pip install -r requirements.txt

# add your API keys
cp .env.example .env             # then fill in your keys
```

## Structure

```
AgenticAI/
├── notebooks/     # experiments and learning exercises
├── agents/        # agent implementations
├── tools/         # reusable tools agents can call
├── docs/          # notes on concepts as I learn them
└── README.md
```

## Learning resources

Papers, courses, and repos worth working through:

- **ReAct** — Reasoning + Acting in language models
- **Reflexion** — agents that self-reflect to improve
- **Toolformer** — teaching models to use tools
- LangChain / LangGraph documentation
- Anthropic's guides on building effective agents

## Status

Early days — actively learning. Expect frequent, messy commits. That's the point.

---

Maintained by [@ozr0013](https://github.com/ozr0013) (Omar Rizwan)
