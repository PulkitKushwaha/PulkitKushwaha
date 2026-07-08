<h1 align="center">Hi, I'm Pulkit Kushwaha 👋</h1>

<p align="center">
  <b>Agentic AI Engineer · LangGraph · Multi-Agent Systems · LLM Security & Eval · Data Engineering</b><br/>
  <i>Building production-grade agentic systems that automate complex enterprise workflows at scale</i>
</p>

<p align="center">
  <a href="mailto:pulkitkushwahadev@gmail.com">📧 Email</a> &nbsp;·&nbsp;
  <a href="https://linkedin.com/in/pulkit-kushwaha-514764197">💼 LinkedIn</a> &nbsp;·&nbsp;
  📍 India &nbsp;·&nbsp;
  <b>Open to opportunities</b>
</p>

---

## About me

I'm an Agentic AI Engineer with 3+ years shipping production multi-agent systems at enterprise scale. I have built a LangGraph orchestrator-workers pipeline serving 50K+ documents, a human-in-the-loop compliance system executing 2,185 checks per quarter across 95 countries, and so on. I am comfortable with both high-code and low-code architectures, as long as they are challenging.

What makes my perspective different is that I understand the full stack that enterprise AI sits on top of: from data pipelines and ETL through to agent orchestration, RAG retrieval, and LLM observability. I've worked with the data infrastructure before building the AI on top of it, which means I know where data breaks, where it's slow, and how to design agents that are actually reliable in production.

I also go deep on the parts most engineers skip: LLM security, eval frameworks, failure modes, output validation, and guardrails, because that's where production AI systems actually break.

Currently deep-diving into MCP (Model Context Protocol): the open standard for plug-and-play tool connectivity in agentic systems and catching up with "Agent Skills". See [`model-context-protocol`](https://github.com/PulkitKushwaha/model-context-protocol).

---

## 🔭 What I'm building

| Area | Repo | Status |
|---|---|---|
| 🤖 MCP Deep Dive | [`model-context-protocol`](https://github.com/PulkitKushwaha/model-context-protocol) | 🔄 In progress |
| 📄 Agentic Documentation Generator | [`autodoc-agent`](https://github.com/PulkitKushwaha/autodoc-agent) | ✅ Available |
| 🕸️ Multi-Agent System (LangGraph) | [`multi-agent-system`](https://github.com/PulkitKushwaha/multi-agent-system) | ✅ Available |
| 🔍 Advanced RAG Pipeline | [`rag-pipeline`](https://github.com/PulkitKushwaha/rag-pipeline) | ✅ Available |
| 🚀 Production RAG API (FastAPI) | [`production-rag-api`](https://github.com/PulkitKushwaha/production-rag-api) | ✅ Available |
| 🏆 Enterprise RAG System (capstone) | [`enterprise-rag-system`](https://github.com/PulkitKushwaha/enterprise-rag-system) | ✅ Available |
| 🛡️ LLM Guardrails & Output Validation | [`llm-guardrails`](https://github.com/PulkitKushwaha/llm-guardrails) | ✅ Available |
| 📊 LLM Evaluation Framework | [`llm-eval-framework`](https://github.com/PulkitKushwaha/llm-eval-framework) | ✅ Available |
| 🔐 LLM Security & Threat Modeling | [`llm-security-playbook`](https://github.com/PulkitKushwaha/llm-security-playbook) | ✅ Available |

---

## 🛠️ Tech stack

**Agentic AI**
`LangGraph` `LangChain` `LangSmith` `MCP (Model Context Protocol)` `ReAct Reasoning` `Parallel Tool Calling` `Human-in-the-Loop Design` `asyncio`

**LLM & Generative AI**
`Azure OpenAI` `Copilot Studio` `Mistral` `HuggingFace` `FAISS` `Azure AI Search` `RAGAS` `Prompt Engineering`

**APIs & Backend**
`Python` `FastAPI` `REST APIs`

**Data Engineering & Pipelines**
`PySpark` `SQL` `Azure Databricks` `Azure Data Factory` `Alteryx` `ETL Pipelines`

**BI & Analytics**
`Power BI` `Qlik SaaS` `DAX` `Power Query`

**Cloud & DevOps**
`Azure` `Azure Web Apps` `Azure Monitor` `Azure Blob Storage` `Power Automate` `CI/CD` `Docker` `Entra ID`

---

## 🏗️ Production projects

### Agentic Knowledge Management Platform
> Rebuilt a GenAI knowledge platform (50K+ documents) as a stateful **LangGraph** graph with typed `QueryState` — session-aware enrichment node, router node with conditional edges to specialist workers: factual RAG, summarization RAG, and NL2SQL aggregation. Added parallel tool calling via `asyncio.gather` for hybrid queries. Integrated RBAC, CI/CD, and Azure Monitor observability.

**Impact:** 60% reduction in document search time · 40% increase in knowledge reuse

---

### Multi-Country Funding Compliance & Report Generation System
> Enterprise-scale **human-in-the-loop** compliance system across 95 countries — an orchestrator agent surfaces 23 compliance questions per submission, each dynamically retrieving its document combination from a 19-document knowledge base (SharePoint) and running a dedicated reasoning agent. Separate 9-agent report generation pipeline produces a structured PDF from HTML sections. Built on **Copilot Studio** and **Azure OpenAI**.

**Impact:** ~60% reduction in review time per country · 95+ person-days saved per quarter · Report drafting cut from days to under an hour

---

### AI-Driven Complaint Screening System
> Stateful 3-node **LangGraph** pipeline (Extraction → Classification → Reporting) for automated OIG complaint screening. Typed `ScreeningState` schema shared across all nodes. Orchestrator LLM dynamically routes to report generation or human review via conditional edges. Strict JSON output contracts at each boundary. Monitored via **LangSmith** tracing.

**Impact:** 70–80% reduction in screening time · ~60% improvement in classification consistency · 50% reduction in drafting effort

---

## 🧪 Portfolio projects

### AutoDoc-Agent — Agentic Technical Documentation Generator
> Multi-agent documentation system built on **LangGraph** that ingests any Python codebase and produces professional technical documentation. A planner agent reads a structured `CodebaseManifest` (produced by an AST-based ingestion engine) and delegates to five specialist writer agents — architecture, API reference, data models, authentication, and deployment — each rendering a **Jinja2** prompt template with real manifest data before calling **Claude** (Anthropic). A critic agent then scores all five sections 1–10 in one LLM call, returning structured JSON; sections below the quality threshold are sent back to their writer with specific critique injected into the revision prompt. The loop is capped at two rounds. Final output rendered as Markdown, a static HTML site, and PDF via **WeasyPrint**. Full strategy-pattern LLM abstraction — one env var switches between mock and real Claude, zero code changes.

**Stack:** LangGraph · Anthropic Claude · Pydantic v2 · Jinja2 · Typer · WeasyPrint · Python AST (stdlib) · uv

**Patterns demonstrated:** orchestrator-workers · conditional edges · iterative self-evaluation loop · strategy pattern · typed state contracts · Jinja2 prompt templates · multi-format rendering

[`autodoc-agent`](https://github.com/PulkitKushwaha/autodoc-agent)

---

## 📌 Areas I go deep on

- **Agentic AI**: LangGraph orchestration, orchestrator-workers pattern, ReAct reasoning, parallel tool calling, stateful graph design, human-in-the-loop workflows, iterative self-evaluation loops, conditional edges, agent failure modes
- **MCP (Model Context Protocol)**: Host/Client/Server architecture, JSON-RPC 2.0, Tools/Resources/Prompts, transport types (stdio vs SSE), adapter patterns
- **Advanced RAG**: HyDE, reranking, metadata filtering, hybrid retrieval, query enrichment, multi-doc retrieval, NL2SQL
- **LLM Security**: Prompt injection (direct + indirect), OWASP LLM Top 10, system prompt extraction, red-teaming, mitigation patterns
- **Eval & Observability**: LangSmith tracing, RAGAS integration, custom eval metrics, CI/CD eval gates, failure mode detection, output schema validation
- **LLM Guardrails**: PII detection + redaction, toxicity filtering, topic scope validation, structured output enforcement
- **Data Architecture**: End-to-end pipeline design — from ETL and data transformation through to AI retrieval and agent orchestration; understanding where data breaks in production

---

## 🎓 Certifications

- Microsoft Certified: Azure AI Engineer Associate (AI-102)
- Microsoft Certified: Azure Data Scientist Associate (DP-100)
- Databricks Generative AI Engineer Associate
- Google Cloud Certified: Generative AI Leader
- Microsoft Certified: Azure Data Fundamentals (DP-900)
- Databricks Certified Data Engineer Associate
- Microsoft Certified: Power BI Data Analyst Associate (PL-300)

---

## 📈 GitHub activity

> Actively building — the portfolio covers the full production agentic AI stack: orchestration, MCP, advanced retrieval, evaluation, security, and guardrails. The [`model-context-protocol`](https://github.com/PulkitKushwaha/model-context-protocol) repo is a structured deep-dive updated as I go.

---

<p align="center">
  <i>"Most AI systems don't fail because of the model. They fail because of everything around it."</i>
</p>
