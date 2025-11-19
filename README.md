# Agentic DeliOps Lab (Gemini + Multi-Agent + Streamlit)

This is a **sandbox project** to understand **Agentic AI** concepts using
Google Vertex AI (Gemini) with a **multi-agent pipeline**:

- **Planner Agent** → decides what to do (hours, menu, order, etc.).
- **Executor Agent** → calls tools (Python functions) and writes a friendly reply.
- **Tools** → Deli-style actions (get hours, check item, create order…).
- **Streamlit UI** → simple web chat to talk to your agent.

Later, you can integrate these ideas into your DeliOps backend and deploy
with a proper FastAPI API, but here we just focus on concepts.

---

## Prerequisites

- Python 3.10+ recommended
- A Google Cloud project with:
  - Vertex AI API enabled
  - Billing enabled
- `gcloud` CLI installed and authenticated:
  ```bash
  gcloud auth application-default login
  gcloud config set project YOUR_PROJECT_ID
