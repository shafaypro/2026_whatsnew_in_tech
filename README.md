# 2026: What's New in Tech

> A hands-on, production-focused reference for every major tool in **Data Engineering**, **AI & GenAI**, and **DevOps** — written for 2025–2026.

**Repository:** [github.com/shafaypro/2026_whatsnew_in_tech](https://github.com/shafaypro/2026_whatsnew_in_tech)

This repo is a living knowledge base. Each guide covers a tool from first principles to advanced production patterns — with real code, real commands, and clear explanations of *why* things work the way they do.

---

## Quick Navigation

| I want to learn about... | Go to |
|--------------------------|-------|
| Running containers locally | [Docker](devops/intro_docker.md) |
| Orchestrating containers in production | [Kubernetes](devops/intro_kubernetes.md) |
| Provisioning cloud infrastructure as code | [Terraform](devops/intro_terraform.md) |
| Automating CI/CD pipelines | [GitHub Actions](devops/intro_github_actions.md) |
| Packaging apps for Kubernetes | [Helm](devops/intro_helm.md) |
| Transforming data in a warehouse with SQL | [dbt](data_engineering/intro_dbt.md) |
| Distributed data processing at scale | [Apache Spark](data_engineering/intro_apache_spark.md) |
| Real-time event streaming | [Apache Kafka](data_engineering/intro_apache_kafka.md) |
| Scheduling and orchestrating data pipelines | [Apache Airflow](data_engineering/intro_apache_airflow.md) |
| ACID tables on S3/cloud storage | [Delta Lake](data_engineering/intro_delta_lake.md) |
| Open table format for multi-engine lakehouses | [Apache Iceberg](data_engineering/intro_apache_iceberg.md) |
| Fast local SQL analytics on files | [DuckDB](data_engineering/intro_duckdb.md) |
| Building with Claude / Anthropic APIs | [Anthropic AI](ai_genai/intro_anthropic.md) |
| Connecting LLMs to tools and data | [Model Context Protocol (MCP)](ai_genai/intro_mcp.md) |
| Autonomous AI agents and multi-agent systems | [Agentic AI](ai_genai/intro_agentic_ai.md) |
| Giving LLMs access to private/up-to-date knowledge | [RAG](ai_genai/intro_rag.md) |
| Storing and searching AI embeddings | [Vector Databases](ai_genai/intro_vector_databases.md) |
| LLM app frameworks and pipelines | [LangChain & LangGraph](ai_genai/intro_langchain.md) |
| Running LLMs in production reliably | [LLMOps](ai_genai/intro_llmops.md) |
| Data lineage and pipeline observability | [OpenClaw](data_engineering/intro_openclaw.md) |
| Unified analytics on Databricks | [Databricks](data_engineering/intro_databricks.html) |

---

## Repository Structure

```
2026_whatsnew_in_tech/
│
├── README.md                          ← You are here
│
├── data_engineering/                  ← Modern data stack
│   ├── intro_dbt.md
│   ├── interview_dbt.md
│   ├── intro_databricks.html
│   ├── intro_openclaw.md
│   ├── intro_apache_spark.md
│   ├── intro_apache_kafka.md
│   ├── intro_apache_airflow.md
│   ├── intro_delta_lake.md
│   ├── intro_apache_iceberg.md
│   └── intro_duckdb.md
│
├── ai_genai/                          ← AI, LLMs, GenAI, Agents
│   ├── intro_anthropic.md
│   ├── intro_mcp.md
│   ├── intro_agentic_ai.md
│   ├── intro_rag.md
│   ├── intro_vector_databases.md
│   ├── intro_langchain.md
│   └── intro_llmops.md
│
└── devops/                            ← Infrastructure & CI/CD
    ├── intro_docker.md
    ├── intro_kubernetes.md
    ├── intro_terraform.md
    ├── intro_helm.md
    └── intro_github_actions.md
```

---

## Data Engineering

The modern data stack — tools for moving, transforming, storing, and querying data at scale.

### [dbt – Data Build Tool](data_engineering/intro_dbt.md)
> *The T in ELT. SQL-first data transformation inside your warehouse.*

| Section | Link |
|---------|------|
| What is dbt? | [→](data_engineering/intro_dbt.md#what-is-dbt) |
| Project Structure | [→](data_engineering/intro_dbt.md#project-structure) |
| Models & Materializations | [→](data_engineering/intro_dbt.md#materializations) |
| Sources & `ref()` | [→](data_engineering/intro_dbt.md#sources--the-ref-function) |
| Tests | [→](data_engineering/intro_dbt.md#tests) |
| Macros & Jinja | [→](data_engineering/intro_dbt.md#macros--jinja) |
| Snapshots (SCD Type 2) | [→](data_engineering/intro_dbt.md#snapshots) |
| Incremental Models | [→](data_engineering/intro_dbt.md#incremental-models) |
| Semantic Layer | [→](data_engineering/intro_dbt.md#semantic-layer--metrics) |
| Cheat Sheet | [→](data_engineering/intro_dbt.md#cheat-sheet) |

### [dbt Interview Q&A](data_engineering/interview_dbt.md)
> *Mid-level to senior/lead interview preparation for dbt.*

| Section | Link |
|---------|------|
| Mid-Level Questions | [→](data_engineering/interview_dbt.md#mid-level-engineer-questions) |
| Incremental Models & Strategies | [→](data_engineering/interview_dbt.md#incremental-models) |
| Snapshots & SCD Type 2 | [→](data_engineering/interview_dbt.md#snapshots--scd-type-2) |
| Jinja, Macros & Packages | [→](data_engineering/interview_dbt.md#jinja-macros--packages) |
| Senior / Lead Questions | [→](data_engineering/interview_dbt.md#seniorlead-questions) |
| Scenario Questions | [→](data_engineering/interview_dbt.md#scenario-questions) |

### [Databricks Platform](data_engineering/intro_databricks.html)
> *The unified analytics platform — Spark, Delta Lake, ML, and SQL in one place.*

- Databricks architecture and workspace concepts
- Unity Catalog for data governance
- Delta Live Tables (DLT) for declarative pipelines
- Databricks SQL for BI workloads
- MLflow integration for ML experiments

> **Note:** This guide is an interactive HTML file — open it in a browser for the full experience with sidebar navigation.

### [OpenClaw – Data Lineage & Orchestration](data_engineering/intro_openclaw.md)
> *Open-source data orchestration with lineage-first design.*

| Section | Link |
|---------|------|
| What is OpenClaw? | [→](data_engineering/intro_openclaw.md#what-is-openclaw) |
| Architecture | [→](data_engineering/intro_openclaw.md#architecture) |
| Lineage Tracking | [→](data_engineering/intro_openclaw.md#lineage-tracking) |
| Data Contracts | [→](data_engineering/intro_openclaw.md#data-contracts) |
| Integration Patterns | [→](data_engineering/intro_openclaw.md#integration-patterns) |
| CLI & GraphQL API | [→](data_engineering/intro_openclaw.md#cli-commands) |
| Glossary | [→](data_engineering/intro_openclaw.md#glossary) |

### [Apache Spark](data_engineering/intro_apache_spark.md)
> *The leading distributed data processing engine for TBs–PBs of data.*

| Section | Link |
|---------|------|
| What is Spark? | [→](data_engineering/intro_apache_spark.md#what-is-spark) |
| Architecture | [→](data_engineering/intro_apache_spark.md#architecture) |
| DataFrames | [→](data_engineering/intro_apache_spark.md#dataframes) |
| Transformations | [→](data_engineering/intro_apache_spark.md#transformations) |
| Spark SQL | [→](data_engineering/intro_apache_spark.md#spark-sql) |
| Writing Data | [→](data_engineering/intro_apache_spark.md#writing-data) |
| Structured Streaming | [→](data_engineering/intro_apache_spark.md#structured-streaming) |
| Performance Tuning | [→](data_engineering/intro_apache_spark.md#performance-tuning) |
| Spark in 2026 | [→](data_engineering/intro_apache_spark.md#spark-in-2026) |
| Cheat Sheet | [→](data_engineering/intro_apache_spark.md#cheat-sheet) |

### [Apache Kafka](data_engineering/intro_apache_kafka.md)
> *The standard for distributed event streaming at scale.*

| Section | Link |
|---------|------|
| What is Kafka? | [→](data_engineering/intro_apache_kafka.md#what-is-kafka) |
| Core Concepts | [→](data_engineering/intro_apache_kafka.md#core-concepts) |
| Running Kafka | [→](data_engineering/intro_apache_kafka.md#running-kafka) |
| Kafka CLI | [→](data_engineering/intro_apache_kafka.md#kafka-cli) |
| Python Producer | [→](data_engineering/intro_apache_kafka.md#python-producer) |
| Python Consumer | [→](data_engineering/intro_apache_kafka.md#python-consumer) |
| Schema Registry | [→](data_engineering/intro_apache_kafka.md#kafka-schemas-with-schema-registry) |
| Kafka Connect & Debezium CDC | [→](data_engineering/intro_apache_kafka.md#kafka-streams--kafka-connect) |
| Data Engineering Pipelines | [→](data_engineering/intro_apache_kafka.md#kafka-in-data-engineering-pipelines) |
| Kafka in 2026 | [→](data_engineering/intro_apache_kafka.md#kafka-in-2026) |

### [Apache Airflow](data_engineering/intro_apache_airflow.md)
> *The most widely used workflow orchestration platform.*

| Section | Link |
|---------|------|
| What is Airflow? | [→](data_engineering/intro_apache_airflow.md#what-is-airflow) |
| Core Concepts | [→](data_engineering/intro_apache_airflow.md#core-concepts) |
| Writing DAGs (TaskFlow API) | [→](data_engineering/intro_apache_airflow.md#writing-dags) |
| Common Operators | [→](data_engineering/intro_apache_airflow.md#common-operators) |
| Dynamic Task Mapping | [→](data_engineering/intro_apache_airflow.md#advanced-dag-patterns) |
| Branching & Sensors | [→](data_engineering/intro_apache_airflow.md#advanced-dag-patterns) |
| dbt + Airflow (Cosmos) | [→](data_engineering/intro_apache_airflow.md#dbt--airflow-integration) |
| Variables & Connections | [→](data_engineering/intro_apache_airflow.md#variables--connections) |
| Monitoring & Alerts | [→](data_engineering/intro_apache_airflow.md#monitoring--alerts) |
| Airflow in 2026 | [→](data_engineering/intro_apache_airflow.md#airflow-in-2026) |
| Cheat Sheet | [→](data_engineering/intro_apache_airflow.md#cheat-sheet) |

### [Delta Lake](data_engineering/intro_delta_lake.md)
> *ACID transactions, time travel, and schema enforcement on your data lake.*

| Section | Link |
|---------|------|
| What is Delta Lake? | [→](data_engineering/intro_delta_lake.md#what-is-delta-lake) |
| Core Features | [→](data_engineering/intro_delta_lake.md#core-features) |
| Writing & Reading | [→](data_engineering/intro_delta_lake.md#writing-and-reading) |
| ACID Transactions | [→](data_engineering/intro_delta_lake.md#acid-transactions) |
| Schema Enforcement & Evolution | [→](data_engineering/intro_delta_lake.md#schema-enforcement--evolution) |
| Time Travel | [→](data_engineering/intro_delta_lake.md#time-travel) |
| Updates, Deletes & MERGE | [→](data_engineering/intro_delta_lake.md#updates-deletes-and-merge-upserts) |
| Streaming | [→](data_engineering/intro_delta_lake.md#streaming-with-delta-lake) |
| Change Data Feed | [→](data_engineering/intro_delta_lake.md#change-data-feed-cdf) |
| Optimize & Z-Order | [→](data_engineering/intro_delta_lake.md#optimize--z-order) |
| Delta Lake + dbt | [→](data_engineering/intro_delta_lake.md#delta-lake--dbt) |
| Delta Lake in 2026 | [→](data_engineering/intro_delta_lake.md#delta-lake-in-2026) |
| Cheat Sheet | [→](data_engineering/intro_delta_lake.md#cheat-sheet) |

### [Apache Iceberg](data_engineering/intro_apache_iceberg.md)
> *The open table format that became the industry standard in 2026.*

| Section | Link |
|---------|------|
| What is Apache Iceberg? | [→](data_engineering/intro_apache_iceberg.md#what-is-apache-iceberg) |
| Iceberg vs Delta vs Hudi | [→](data_engineering/intro_apache_iceberg.md#iceberg-vs-delta-lake-vs-hudi) |
| Core Architecture | [→](data_engineering/intro_apache_iceberg.md#core-architecture) |
| Getting Started | [→](data_engineering/intro_apache_iceberg.md#getting-started) |
| Core Operations (CRUD + MERGE) | [→](data_engineering/intro_apache_iceberg.md#core-operations) |
| Schema Evolution | [→](data_engineering/intro_apache_iceberg.md#schema-evolution) |
| Hidden Partitioning | [→](data_engineering/intro_apache_iceberg.md#partitioning--hidden-partitioning) |
| Partition Evolution | [→](data_engineering/intro_apache_iceberg.md#partition-evolution) |
| Time Travel & Snapshots | [→](data_engineering/intro_apache_iceberg.md#time-travel--snapshots) |
| Table Maintenance | [→](data_engineering/intro_apache_iceberg.md#table-maintenance) |
| Catalogs (Glue, Nessie, REST) | [→](data_engineering/intro_apache_iceberg.md#iceberg-catalogs) |
| DuckDB + Iceberg | [→](data_engineering/intro_apache_iceberg.md#duckdb--iceberg) |
| Iceberg in 2026 | [→](data_engineering/intro_apache_iceberg.md#iceberg-in-2026) |
| Cheat Sheet | [→](data_engineering/intro_apache_iceberg.md#cheat-sheet) |

### [DuckDB](data_engineering/intro_duckdb.md)
> *In-process OLAP database — the SQLite of analytics. Fast, zero-setup, powerful.*

| Section | Link |
|---------|------|
| What is DuckDB? | [→](data_engineering/intro_duckdb.md#what-is-duckdb) |
| Installation & Setup | [→](data_engineering/intro_duckdb.md#installation--setup) |
| Reading Files Directly | [→](data_engineering/intro_duckdb.md#reading-files-directly) |
| Querying S3 / Cloud Storage | [→](data_engineering/intro_duckdb.md#s3--cloud-storage) |
| Delta Lake & Iceberg | [→](data_engineering/intro_duckdb.md#delta-lake) |
| Python API | [→](data_engineering/intro_duckdb.md#python-api) |
| Querying DataFrames (zero-copy) | [→](data_engineering/intro_duckdb.md#querying-dataframes-directly) |
| Advanced SQL Features | [→](data_engineering/intro_duckdb.md#advanced-sql-features) |
| dbt + DuckDB | [→](data_engineering/intro_duckdb.md#integrations) |
| DuckDB in Production | [→](data_engineering/intro_duckdb.md#duckdb-in-production) |
| DuckDB vs Spark vs Pandas | [→](data_engineering/intro_duckdb.md#duckdb-vs-spark-vs-pandas) |
| DuckDB in 2026 | [→](data_engineering/intro_duckdb.md#duckdb-in-2026) |
| Cheat Sheet | [→](data_engineering/intro_duckdb.md#cheat-sheet) |

---

## AI & GenAI

Large language models, agents, retrieval systems, and the infrastructure to run them in production.

### [Anthropic AI – Claude, APIs & Core Concepts](ai_genai/intro_anthropic.md)
> *Building with Claude — from the first API call to production agents.*

| Section | Link |
|---------|------|
| Anthropic & Claude Overview | [→](ai_genai/intro_anthropic.md#anthropic--claude-overview) |
| Claude Model Family | [→](ai_genai/intro_anthropic.md#claude-model-family) |
| Core AI/LLM Concepts | [→](ai_genai/intro_anthropic.md#core-aillm-concepts) |
| API Basics & Setup | [→](ai_genai/intro_anthropic.md#anthropic-api-basics) |
| Messages API | [→](ai_genai/intro_anthropic.md#messages-api) |
| Tool Use (Function Calling) | [→](ai_genai/intro_anthropic.md#tool-use-function-calling) |
| Vision & Multimodal | [→](ai_genai/intro_anthropic.md#vision--multimodal) |
| Streaming | [→](ai_genai/intro_anthropic.md#streaming) |
| Prompt Engineering | [→](ai_genai/intro_anthropic.md#prompt-engineering) |
| Constitutional AI & Safety | [→](ai_genai/intro_anthropic.md#claudes-constitution--safety) |
| Context Caching & Batch API | [→](ai_genai/intro_anthropic.md#claude-in-production) |
| 2026: What's New | [→](ai_genai/intro_anthropic.md#2026-whats-new) |

### [Model Context Protocol (MCP)](ai_genai/intro_mcp.md)
> *The USB-C of AI integrations — one protocol to connect any LLM to any tool.*

| Section | Link |
|---------|------|
| What is MCP? | [→](ai_genai/intro_mcp.md#what-is-mcp) |
| Why MCP Matters | [→](ai_genai/intro_mcp.md#why-mcp-matters) |
| Architecture & Transport | [→](ai_genai/intro_mcp.md#architecture) |
| Core Primitives (Tools, Resources, Prompts) | [→](ai_genai/intro_mcp.md#core-primitives) |
| MCP in Claude Code | [→](ai_genai/intro_mcp.md#mcp-in-claude-code) |
| Popular MCP Servers | [→](ai_genai/intro_mcp.md#popular-mcp-servers) |
| Build an MCP Server (Python) | [→](ai_genai/intro_mcp.md#building-an-mcp-server-python) |
| Build an MCP Server (TypeScript) | [→](ai_genai/intro_mcp.md#building-an-mcp-server-typescript) |
| MCP Client Usage | [→](ai_genai/intro_mcp.md#mcp-client-using-a-server) |
| MCP in 2026 | [→](ai_genai/intro_mcp.md#mcp-in-2026--ecosystem) |

### [Agentic AI & Multi-Agent Systems](ai_genai/intro_agentic_ai.md)
> *LLMs that plan, use tools, and autonomously execute multi-step tasks.*

| Section | Link |
|---------|------|
| What is Agentic AI? | [→](ai_genai/intro_agentic_ai.md#what-is-agentic-ai) |
| Agent Anatomy | [→](ai_genai/intro_agentic_ai.md#agent-anatomy) |
| Agent Patterns (ReAct, Plan-Execute) | [→](ai_genai/intro_agentic_ai.md#agent-patterns) |
| Building Agents with Claude | [→](ai_genai/intro_agentic_ai.md#building-agents-with-claude) |
| Multi-Agent Systems | [→](ai_genai/intro_agentic_ai.md#multi-agent-systems) |
| Human-in-the-Loop | [→](ai_genai/intro_agentic_ai.md#anthropic-agent-sdk) |
| Agent Memory | [→](ai_genai/intro_agentic_ai.md#agent-memory) |
| Evaluation & Safety | [→](ai_genai/intro_agentic_ai.md#agent-evaluation--safety) |
| Real-World Examples | [→](ai_genai/intro_agentic_ai.md#real-world-examples) |
| 2026 Landscape | [→](ai_genai/intro_agentic_ai.md#2026-landscape) |

### [RAG – Retrieval-Augmented Generation](ai_genai/intro_rag.md)
> *Give your LLM access to private, up-to-date, and domain-specific knowledge.*

| Section | Link |
|---------|------|
| What is RAG? | [→](ai_genai/intro_rag.md#what-is-rag) |
| RAG vs Fine-tuning | [→](ai_genai/intro_rag.md#rag-vs-fine-tuning) |
| Pipeline Architecture | [→](ai_genai/intro_rag.md#rag-pipeline-architecture) |
| Indexing: Loading & Chunking | [→](ai_genai/intro_rag.md#indexing-offline) |
| Embeddings | [→](ai_genai/intro_rag.md#step-3-embedding) |
| Vector Storage | [→](ai_genai/intro_rag.md#step-4-store-in-vector-db) |
| Retrieval: Vector + Hybrid Search | [→](ai_genai/intro_rag.md#retrieval-online) |
| Reranking | [→](ai_genai/intro_rag.md#reranking) |
| Generation | [→](ai_genai/intro_rag.md#generation) |
| Query Rewriting & HyDE | [→](ai_genai/intro_rag.md#advanced-rag-techniques) |
| Agentic RAG | [→](ai_genai/intro_rag.md#agentic-rag) |
| Evaluation (RAGAS) | [→](ai_genai/intro_rag.md#evaluation) |
| End-to-End Example | [→](ai_genai/intro_rag.md#end-to-end-example) |
| RAG in 2026 | [→](ai_genai/intro_rag.md#rag-in-2026) |

### [Vector Databases](ai_genai/intro_vector_databases.md)
> *Storing and searching AI embeddings — the backbone of semantic search and RAG.*

| Section | Link |
|---------|------|
| What is a Vector Database? | [→](ai_genai/intro_vector_databases.md#what-is-a-vector-database) |
| Similarity Metrics | [→](ai_genai/intro_vector_databases.md#similarity-metrics) |
| ANN Algorithms | [→](ai_genai/intro_vector_databases.md#ann-algorithms) |
| Pinecone | [→](ai_genai/intro_vector_databases.md#1-pinecone-managed-cloud-native) |
| Weaviate | [→](ai_genai/intro_vector_databases.md#2-weaviate-open-source-hybrid-search-built-in) |
| Chroma | [→](ai_genai/intro_vector_databases.md#3-chroma-developer-friendly-local-first) |
| pgvector | [→](ai_genai/intro_vector_databases.md#4-pgvector-postgresql-extension) |
| Qdrant | [→](ai_genai/intro_vector_databases.md#5-qdrant-performance-focused-rust-based) |
| Choosing a Vector DB | [→](ai_genai/intro_vector_databases.md#choosing-a-vector-database) |
| Embedding Models in 2026 | [→](ai_genai/intro_vector_databases.md#embedding-models-in-2026) |
| Production Patterns | [→](ai_genai/intro_vector_databases.md#production-patterns) |

### [LangChain & LangGraph](ai_genai/intro_langchain.md)
> *The most widely used framework for building LLM-powered applications.*

| Section | Link |
|---------|------|
| LangChain Overview | [→](ai_genai/intro_langchain.md#langchain-overview) |
| LCEL – Pipe Operator | [→](ai_genai/intro_langchain.md#lcel--langchain-expression-language) |
| RAG Chain | [→](ai_genai/intro_langchain.md#rag-chain) |
| Document Loaders & Splitters | [→](ai_genai/intro_langchain.md#document-loaders--text-splitters) |
| Agents with @tool | [→](ai_genai/intro_langchain.md#agents-in-langchain) |
| LangGraph – Stateful Graphs | [→](ai_genai/intro_langchain.md#langgraph--stateful-agent-graphs) |
| Multi-Agent Graph | [→](ai_genai/intro_langchain.md#multi-agent-graph) |
| LangSmith Observability | [→](ai_genai/intro_langchain.md#langsmith-observability) |
| LangChain vs LlamaIndex vs Raw API | [→](ai_genai/intro_langchain.md#langchain-vs-llamaindex-vs-raw-api) |

### [LLMOps](ai_genai/intro_llmops.md)
> *Deploying, monitoring, evaluating, and maintaining LLMs in production.*

| Section | Link |
|---------|------|
| LLMOps vs MLOps | [→](ai_genai/intro_llmops.md#llmops-vs-mlops) |
| The LLMOps Stack | [→](ai_genai/intro_llmops.md#the-llmops-stack) |
| Observability & Tracing | [→](ai_genai/intro_llmops.md#observability--tracing) |
| Evaluations (LLM-as-judge, RAGAS) | [→](ai_genai/intro_llmops.md#evaluations-evals) |
| Eval Suites in CI/CD | [→](ai_genai/intro_llmops.md#eval-suites-continuous-testing) |
| Prompt Versioning & A/B Testing | [→](ai_genai/intro_llmops.md#prompt-management) |
| Cost Management | [→](ai_genai/intro_llmops.md#cost-management) |
| Guardrails (input/output safety) | [→](ai_genai/intro_llmops.md#guardrails) |
| Production Checklist | [→](ai_genai/intro_llmops.md#production-checklist) |
| LLMOps Tools in 2026 | [→](ai_genai/intro_llmops.md#llmops-tools-in-2026) |

---

## DevOps & Infrastructure

Containers, orchestration, infrastructure as code, and CI/CD for modern software delivery.

### [Docker](devops/intro_docker.md)
> *The standard for packaging applications into portable containers.*

| Section | Link |
|---------|------|
| What is Docker? | [→](devops/intro_docker.md#what-is-docker) |
| Core Concepts | [→](devops/intro_docker.md#core-concepts) |
| Dockerfile | [→](devops/intro_docker.md#dockerfile) |
| Images & Containers | [→](devops/intro_docker.md#images--containers) |
| Volumes & Networking | [→](devops/intro_docker.md#volumes--networking) |
| Docker Compose | [→](devops/intro_docker.md#docker-compose) |
| Multi-Stage Builds | [→](devops/intro_docker.md#multi-stage-builds) |
| Docker in CI/CD | [→](devops/intro_docker.md#docker-in-cicd) |
| Security Best Practices | [→](devops/intro_docker.md#security-best-practices) |
| Docker in 2026 | [→](devops/intro_docker.md#docker-in-2026) |
| Cheat Sheet | [→](devops/intro_docker.md#cheat-sheet) |

### [Kubernetes](devops/intro_kubernetes.md)
> *Container orchestration — automating deployment, scaling, and self-healing at scale.*

| Section | Link |
|---------|------|
| What is Kubernetes? | [→](devops/intro_kubernetes.md#what-is-kubernetes) |
| Architecture | [→](devops/intro_kubernetes.md#architecture) |
| Core Objects | [→](devops/intro_kubernetes.md#core-objects) |
| kubectl Basics | [→](devops/intro_kubernetes.md#kubectl-basics) |
| Deployments & Rollbacks | [→](devops/intro_kubernetes.md#workloads) |
| StatefulSets, DaemonSets, Jobs | [→](devops/intro_kubernetes.md#statefulset) |
| Services & DNS | [→](devops/intro_kubernetes.md#services--networking) |
| Storage (PV / PVC) | [→](devops/intro_kubernetes.md#storage) |
| ConfigMaps & Secrets | [→](devops/intro_kubernetes.md#configuration) |
| Namespaces & RBAC | [→](devops/intro_kubernetes.md#namespaces--rbac) |
| Ingress | [→](devops/intro_kubernetes.md#ingress) |
| HPA & VPA Autoscaling | [→](devops/intro_kubernetes.md#scaling--auto-scaling) |
| Observability (Prometheus, Loki) | [→](devops/intro_kubernetes.md#observability) |
| Kubernetes in 2026 | [→](devops/intro_kubernetes.md#kubernetes-in-2026) |
| Cheat Sheet | [→](devops/intro_kubernetes.md#cheat-sheet) |

### [Terraform](devops/intro_terraform.md)
> *Infrastructure as Code — provision and manage cloud resources declaratively.*

| Section | Link |
|---------|------|
| What is Terraform? | [→](devops/intro_terraform.md#what-is-terraform) |
| Core Concepts | [→](devops/intro_terraform.md#core-concepts) |
| Installation | [→](devops/intro_terraform.md#installation) |
| HCL Language Basics | [→](devops/intro_terraform.md#hcl-language-basics) |
| Resources & Data Sources | [→](devops/intro_terraform.md#resources--data-sources) |
| Variables & Outputs | [→](devops/intro_terraform.md#variables--outputs) |
| State Management | [→](devops/intro_terraform.md#state-management) |
| Modules | [→](devops/intro_terraform.md#modules) |
| Workspaces & Environments | [→](devops/intro_terraform.md#workspaces--environments) |
| Terraform Workflow | [→](devops/intro_terraform.md#terraform-workflow) |
| Real-World Example (VPC + EKS) | [→](devops/intro_terraform.md#real-world-examples) |
| Testing Terraform | [→](devops/intro_terraform.md#testing-terraform) |
| OpenTofu (open-source fork) | [→](devops/intro_terraform.md#terraform-in-2026-opentofu) |
| Cheat Sheet | [→](devops/intro_terraform.md#cheat-sheet) |

### [Helm](devops/intro_helm.md)
> *The package manager for Kubernetes — deploy complex apps with one command.*

| Section | Link |
|---------|------|
| What is Helm? | [→](devops/intro_helm.md#what-is-helm) |
| Core Workflow | [→](devops/intro_helm.md#core-workflow) |
| Chart Structure | [→](devops/intro_helm.md#chart-structure) |
| Templates & Go Templating | [→](devops/intro_helm.md#templates) |
| Values Override Strategies | [→](devops/intro_helm.md#values-override-strategies) |
| Debugging & Testing | [→](devops/intro_helm.md#debugging--testing) |
| OCI Registries | [→](devops/intro_helm.md#oci-registries-2026-standard) |
| Popular Charts in 2026 | [→](devops/intro_helm.md#popular-charts-in-2026) |
| Cheat Sheet | [→](devops/intro_helm.md#cheat-sheet) |

### [GitHub Actions](devops/intro_github_actions.md)
> *Built-in CI/CD for GitHub — automate everything from tests to deployments.*

| Section | Link |
|---------|------|
| Core Concepts | [→](devops/intro_github_actions.md#core-concepts) |
| Basic Workflow | [→](devops/intro_github_actions.md#basic-workflow) |
| Triggers (on:) | [→](devops/intro_github_actions.md#triggers-on) |
| Jobs & Steps | [→](devops/intro_github_actions.md#jobs--steps) |
| Matrix Strategy | [→](devops/intro_github_actions.md#matrix-strategy-run-jobs-across-multiple-configs) |
| Job Dependencies | [→](devops/intro_github_actions.md#job-dependencies--fan-outfan-in) |
| Secrets & Variables | [→](devops/intro_github_actions.md#secrets--variables) |
| Reusable Workflows | [→](devops/intro_github_actions.md#reusable-workflows) |
| Complete CI/CD Pipeline | [→](devops/intro_github_actions.md#complete-cicd-pipeline-example) |
| Useful Actions (2026) | [→](devops/intro_github_actions.md#useful-actions-2026) |
| Cheat Sheet | [→](devops/intro_github_actions.md#cheat-sheet) |

---

## 2026 Trends at a Glance

### Data Engineering
- **Open Table Formats** — Apache Iceberg is now the default. Delta Lake and Hudi converging via UniForm.
- **DuckDB everywhere** — replacing Spark for <500GB workloads. Runs in browsers (WASM), notebooks, pipelines.
- **Streaming-first** — Kafka + Flink replacing traditional batch ETL in most real-time use cases.
- **Data Contracts** — dbt contracts + OpenClaw policies enforcing schema and quality at the source.
- **Lakehouse is the architecture** — no more separate data lake + data warehouse.

### AI & GenAI
- **Agentic AI is production-ready** — ReAct loops, multi-agent orchestration, and human-in-the-loop patterns are battle-tested.
- **MCP is the integration standard** — every major AI tool (Claude, GPT, Gemini, Cursor) supports it.
- **RAG 2.0** — Hybrid search + reranking + agentic RAG replacing naive vector lookup.
- **LLMOps matured** — Evals, tracing, and guardrails are non-negotiable in production.
- **200K context windows** — For small datasets, just stuff everything in context instead of building RAG.
- **Small Language Models** — Phi-4, Gemma 3, Llama 3.3 running on-device for privacy and cost.

### DevOps
- **Platform Engineering** — Internal Developer Platforms (Backstage, Port) abstracting K8s complexity.
- **GitOps is the default** — ArgoCD and Flux for all Kubernetes deployments.
- **eBPF observability** — Cilium, Tetragon, Pixie — kernel-level insight without sidecars.
- **OpenTofu** — Open-source Terraform fork is now the safe enterprise choice.
- **AI-assisted infrastructure** — Claude Code, Copilot, and Cursor writing Terraform, Helm, and K8s YAML.

---

## How Each Guide is Structured

Every guide in this repo follows the same pattern so you can navigate quickly:

1. **What is it & why does it matter** — The mental model. What problem does it solve?
2. **Core concepts** — The 20% of knowledge that covers 80% of use cases. Diagrams where helpful.
3. **Installation & setup** — Getting started in under 5 minutes.
4. **Hands-on code examples** — Real, runnable code you can copy and adapt.
5. **Advanced patterns** — Production-grade techniques used at real companies.
6. **Tool X in 2026** — What's new, what changed, what's trending.
7. **Cheat sheet** — Quick reference for commands and syntax at the end.

---

## Contributing

Contributions are welcome! To add or improve a guide:

1. Fork the repo: [github.com/shafaypro/2026_whatsnew_in_tech](https://github.com/shafaypro/2026_whatsnew_in_tech)
2. Create a branch: `git checkout -b add-tool-name`
3. Follow the guide structure above
4. Submit a PR with a clear description of what you added

### Suggested topics still to cover
- Apache Flink
- Trino / Presto
- Great Expectations / Soda (data quality)
- Prefect / Dagster (alternative orchestrators)
- dbt Cloud
- Snowflake (SQL guide)
- AWS CDK / Pulumi
- ArgoCD / Flux (GitOps)
- OpenTelemetry
- Grafana + Prometheus

---

*Last updated: March 2026 · Maintained by [@shafaypro](https://github.com/shafaypro)*
