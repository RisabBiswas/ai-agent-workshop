# Build a real AI agent, layer by layer

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RisabBiswas/ai-agent-workshop/blob/main/AI_Agent_Workshop.ipynb)

Hands-on session of the One Day AI/ML Workshop, Dept. of CSE, Tezpur University, 23 Nov 2026.

You build **Alex**, a customer-support agent for an online shop called **Acme Store**, one production layer at a
time, in one Google Colab notebook. Plain Python, a free LLM (Groq), the official MCP SDK. No agent framework.

| Layer | What you add |
|---|---|
| 1 | One LLM API call |
| 1+ | A look inside the model: its chain of thought, thinking time, and confident mistakes |
| 2 | A system prompt |
| 3 | RAG over the shop's policies |
| 4 | Tools over MCP, and the agent loop |
| 5 | Access control: signed login tokens and roles |
| 6 | Guardrails: prompt injection, PII redaction |
| 7 | A semantic cache and a small/big model router |
| 8 | Traces and evals |

## Start
1. Click **Open in Colab** above, then *File → Save a copy in Drive*.
2. Get a free Groq key: [console.groq.com](https://console.groq.com) → **API Keys** → *Create API Key* (no card).
3. In Colab: **🔑 Secrets** → *Add new secret* → name `GROQ_API_KEY` → paste → switch on *Notebook access*.
4. Run the cells top to bottom with **Shift + Enter**.

Never paste an API key into a code cell.

## Run it on your laptop instead
```bash
pip install jupyter openai "mcp>=2.3,<3" fastembed scikit-learn pandas matplotlib
export GROQ_API_KEY=...        # your key
jupyter notebook AI_Agent_Workshop.ipynb
```
