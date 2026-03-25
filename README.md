# 2026: What's New in Tech

A comprehensive, hands-on reference for the most important tools and concepts across **Data Engineering**, **AI/GenAI**, and **DevOps** in 2025–2026.

---

## Structure

```
2026_whatsnew_in_tech/
├── data_engineering/       # Modern data stack tools
├── ai_genai/               # AI, LLMs, GenAI, Agents
└── devops/                 # Infrastructure, containers, IaC
```

---

## Data Engineering

| File | Topic | Level |
|------|-------|-------|
| [intro_dbt.md](data_engineering/intro_dbt.md) | dbt – Data Build Tool | Beginner → Advanced |
| [interview_dbt.md](data_engineering/interview_dbt.md) | dbt Interview Q&A | Mid → Senior |
| [intro_openclaw.md](data_engineering/intro_openclaw.md) | OpenClaw – Data Lineage & Orchestration | Beginner → Advanced |
| [intro_databricks.html](data_engineering/intro_databricks.html) | Databricks Platform | Beginner → Advanced |
| [intro_apache_spark.md](data_engineering/intro_apache_spark.md) | Apache Spark – Distributed Processing | Beginner → Advanced |
| [intro_apache_kafka.md](data_engineering/intro_apache_kafka.md) | Apache Kafka – Event Streaming | Beginner → Advanced |
| [intro_apache_airflow.md](data_engineering/intro_apache_airflow.md) | Apache Airflow – Workflow Orchestration | Beginner → Advanced |
| [intro_delta_lake.md](data_engineering/intro_delta_lake.md) | Delta Lake – ACID Tables on Cloud Storage | Beginner → Advanced |
| [intro_apache_iceberg.md](data_engineering/intro_apache_iceberg.md) | Apache Iceberg – Open Table Format | Beginner → Advanced |
| [intro_duckdb.md](data_engineering/intro_duckdb.md) | DuckDB – In-Process OLAP Database | Beginner → Advanced |

---

## AI & GenAI

| File | Topic | Level |
|------|-------|-------|
| [intro_anthropic.md](ai_genai/intro_anthropic.md) | Anthropic AI – Claude, APIs, Concepts | Beginner → Advanced |
| [intro_mcp.md](ai_genai/intro_mcp.md) | Model Context Protocol (MCP) | Beginner → Advanced |
| [intro_agentic_ai.md](ai_genai/intro_agentic_ai.md) | Agentic AI & Multi-Agent Systems | Beginner → Advanced |
| [intro_rag.md](ai_genai/intro_rag.md) | RAG – Retrieval-Augmented Generation | Beginner → Advanced |
| [intro_vector_databases.md](ai_genai/intro_vector_databases.md) | Vector Databases – Pinecone, Weaviate, pgvector | Beginner → Advanced |
| [intro_langchain.md](ai_genai/intro_langchain.md) | LangChain & LangGraph | Beginner → Advanced |
| [intro_llmops.md](ai_genai/intro_llmops.md) | LLMOps – Deploying & Monitoring LLMs | Beginner → Advanced |

---

## DevOps & Infrastructure

| File | Topic | Level |
|------|-------|-------|
| [intro_docker.md](devops/intro_docker.md) | Docker – Containers | Beginner → Advanced |
| [intro_kubernetes.md](devops/intro_kubernetes.md) | Kubernetes – Container Orchestration | Beginner → Advanced |
| [intro_terraform.md](devops/intro_terraform.md) | Terraform – Infrastructure as Code | Beginner → Advanced |
| [intro_helm.md](devops/intro_helm.md) | Helm – Kubernetes Package Manager | Beginner → Advanced |
| [intro_github_actions.md](devops/intro_github_actions.md) | GitHub Actions – CI/CD | Beginner → Advanced |

---

## 2026 Trends at a Glance

### Data Engineering
- **Open Table Formats** (Iceberg, Delta Lake, Hudi) have become the standard for lakehouses
- **DuckDB** is eating SQLite's lunch for local analytics and replacing heavy Spark jobs for small-to-medium data
- **Streaming-first pipelines** with Kafka + Flink replacing traditional batch ETL
- **Data Contracts** (dbt contracts, OpenClaw policies) enforcing schema and quality at the source
- **Unified batch + streaming** with Apache Flink and Spark Structured Streaming

### AI & GenAI
- **Agentic AI** – LLMs calling tools, managing state, and running autonomous workflows (Claude Code, GitHub Copilot Workspace)
- **Model Context Protocol (MCP)** – Anthropic's open standard for connecting LLMs to tools and data sources; adopted industry-wide
- **RAG 2.0** – Hybrid search, re-ranking, agentic RAG replacing naive vector lookup
- **LLMOps** – Mature observability, evals, and guardrails (LangSmith, Arize, Weights & Biases)
- **Multimodal models** – Vision, audio, and code generation in a single model
- **Small Language Models (SLMs)** – Phi-4, Gemma 3, Llama 3.3 running on-device

### DevOps
- **Platform Engineering** – Internal Developer Platforms (IDPs) with Backstage, Port
- **GitOps** – ArgoCD, Flux becoming standard for Kubernetes deployments
- **eBPF** – Kernel-level observability powering Cilium, Tetragon, Pixie
- **OpenTofu** – Open-source Terraform fork gaining enterprise adoption
- **Dagger** – Portable CI/CD pipelines as code (replacing YAML-heavy pipelines)

---

## How to Use This Repo

Each guide follows a consistent structure:
1. **What is it & why does it matter** – mental model first
2. **Core concepts** – the 20% you need to know 80% of the time
3. **Hands-on examples** – real code, real commands
4. **Advanced patterns** – production-grade techniques
5. **Interview questions** – where applicable
6. **Cheat sheet** – quick reference at the end

---

*Last updated: March 2026*
