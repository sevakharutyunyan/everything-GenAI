# Everything GenAI

A comprehensive hands-on tutorial covering applied GenAI — from LLM fundamentals through RAG to advanced agentic strategies.

This single Jupyter notebook walks through calling LLMs, building retrieval pipelines, and orchestrating autonomous agents — with runnable code for every pattern.

## What's Inside

| Part | Topic | Sections |
|------|-------|----------|
| **1** | **LLM Fundamentals** | API basics, tokenization, embeddings, context windows, streaming, sampling, prompting, structured output, LLM-as-judge, tool use |
| **2** | **RAG** | Data ingestion, chunking, embeddings for retrieval, vector databases, search strategies, generation, evaluation, HyDE, reranking |
| **3** | **Agent Fundamentals** | Agents, tools, memory, guardrails, parallelization, ReAct, plan-execute, routing, tree of thoughts |
| **4** | **Advanced Strategies I** | Supervisor/worker, fan-out, reflection, reflexion, voyager, GEPA, LATS |
| **5** | **Advanced Strategies II** | Error recovery, utility-based decisions, HTN, causal discovery, REWOO, self-discovery |

## Getting Started

### Prerequisites

- Python 3.11+
- An [OpenAI API key](https://platform.openai.com/api-keys)
- No other infrastructure required (vector DB runs in-memory)

### Setup

1. Set up a Python 3.11+ environment
2. Clone the repo and create a `.env` file with your OpenAI API key:
   ```bash
   git clone https://github.com/sevakharutyunyan/everything-GenAI.git
   cd everything-GenAI
   echo "OPENAI_API_KEY=sk-..." > .env
   ```
3. Open the notebook, choose venv as kernel — the first cell installs all dependencies

## References

### Foundational

- [Attention Is All You Need (Vaswani et al., 2017)](https://arxiv.org/abs/1706.03762)
- [LLM Powered Autonomous Agents (Lilian Weng, 2023)](https://lilianweng.github.io/posts/2023-06-23-agent/)
- [Artificial Intelligence: A Modern Approach (Russell & Norvig)](https://aima.cs.berkeley.edu/)

### LLM Fundamentals

- [OpenAI API Documentation](https://platform.openai.com/docs)
- [OpenAI Tokenizer](https://platform.openai.com/tokenizer)
- [tiktoken — Fast BPE tokeniser for OpenAI models](https://github.com/openai/tiktoken)

### RAG

- [RAG: Retrieval-Augmented Generation (Lewis et al., 2020)](https://arxiv.org/abs/2005.11401)
- [HyDE: Hypothetical Document Embeddings (Gao et al., 2022)](https://arxiv.org/abs/2212.10496)
- [Qdrant — Vector Search Engine](https://qdrant.tech/documentation/)
- [FastEmbed — Fast, lightweight embedding generation](https://github.com/qdrant/fastembed)
- [BGE Reranker — Cross-encoder for reranking](https://huggingface.co/BAAI/bge-reranker-base)

### Agentic AI

- [ReAct: Synergizing Reasoning and Acting (Yao et al., 2022)](https://arxiv.org/abs/2210.03629)
- [Reflexion: Language Agents with Verbal Reinforcement Learning (Shinn et al., 2023)](https://arxiv.org/abs/2303.11366)
- [Voyager: An Open-Ended Embodied Agent (2023)](https://arxiv.org/abs/2305.16291)
- [REWOO: Reasoning Without Observation (2023)](https://arxiv.org/abs/2305.18323)
- [LATS: Language Agent Tree Search (2023)](https://arxiv.org/abs/2310.04406)
- [Self-Discover: Large Language Models Self-Compose Reasoning Structures (2024)](https://arxiv.org/abs/2402.03620)

### Frameworks & SDKs

- [OpenAI Agents SDK — Documentation](https://openai.github.io/openai-agents-python/)
- [OpenAI Agents SDK — GitHub](https://github.com/openai/openai-agents-python)
- [OpenAI Agents SDK — Examples](https://github.com/openai/openai-agents-python/tree/main/examples)

### Pattern Libraries & Production References

- [Agent Patterns Documentation](https://agent-patterns.readthedocs.io/en/latest/)
- [Azure — Retry Pattern](https://learn.microsoft.com/en-us/azure/architecture/patterns/retry)
- [Azure — Circuit Breaker Pattern](https://learn.microsoft.com/en-us/azure/architecture/patterns/circuit-breaker)

### Code & Tools

- [Reflexion — GitHub](https://github.com/noahshinn/reflexion)
- [Voyager — GitHub](https://github.com/MineDojo/Voyager)
- [LATS — GitHub](https://github.com/andyz245/LanguageAgentTreeSearch)
- [DoWhy — Causal Inference Library](https://www.pywhy.org/dowhy/)
- [Wikipedia — HTN Planning](https://en.wikipedia.org/wiki/Hierarchical_task_network)
- [Python asyncio.gather](https://docs.python.org/3/library/asyncio-task.html#asyncio.gather)
