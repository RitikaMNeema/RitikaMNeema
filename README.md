# Ritika Neema

**Data Engineer** · San Francisco Bay Area

I build data platforms that hold up in production — incremental and idempotent pipelines, lakehouse table design, orchestration, and quality gates that actually block bad data. Three years of production AWS + PySpark work at TCS on the Eli Lilly account, now finishing an M.S. in Applied Data Intelligence at San José State.

Lately I've been pushing into the overlap between data engineering and LLM systems: streaming pipelines that carry a model, and agents that read the pipeline's output and explain it.

[LinkedIn](https://linkedin.com/in/ritika-neema) · [Portfolio](https://ritikamneema.github.io) · [ritikamukesh.neema@sjsu.edu](mailto:ritikamukesh.neema@sjsu.edu)

---

## Featured work

| Project | What it does | Stack |
|---|---|---|
| **GH Archive Lakehouse** | Incremental, idempotent lakehouse over the public GitHub event stream. Raw → bronze → silver → gold with a blocking quality gate, documented SLAs, and atomic per-file redo. Deliberately model-free — the hard parts are schema evolution, partition design, and late-arriving data. 33/33 dbt tests green on real data. | Iceberg, Spark, dbt on Trino, Airflow, Postgres |
| [**FraudLens**](https://github.com/RitikaMNeema/Large_Scale_Product-Review) | End-to-end big-data pipeline over 20.8M records (11 GB): Spark batch ETL, dual sentiment + fraud models, and a Structured Streaming scorer that flagged 20,048 fraudulent records (3.71%). Includes an autonomous LLM auditor that reviews flagged records over an MCP tool server and emits structured audit reports. | PySpark, Kafka, MLflow, FastAPI, Ollama, FastMCP |
| [**PaySim Fraud Triage**](https://github.com/RitikaMNeema/paysim-fraud-chain-triage) | Fraud detection on 6.3M mobile-money transactions at 773:1 class imbalance. Chain-aware features (TRANSFER→CASH_OUT), 7 models benchmarked, calibrated CatBoost at PR-AUC 0.9986, and a GREEN/YELLOW/RED triage system with SHAP behind every flag. | CatBoost, scikit-learn, SHAP |
| [**Netflix Analytics Pipeline**](https://github.com/RitikaMNeema/Netflix-Data-Analytics-Pipeline-Snowflake-dbt-AWS-S3) | Enterprise-shaped warehouse workflow: S3 → Snowflake via `COPY INTO`, then modular, tested, version-controlled dbt transformations into analytics models. | AWS S3, Snowflake, dbt |
| [**Urban Traffic & Weather**](https://github.com/RitikaMNeema/Urban-Traffic-Weather-Analysis) | Orchestrated pipeline joining live traffic and weather APIs to surface California congestion hotspots, modeled in Snowflake and visualized for real-time situational awareness. | Airflow, Snowflake, dbt, Preset, TomTom & Open-Meteo APIs |

---

## What I work with

**Data & warehousing** — PySpark · Spark SQL · Apache Iceberg · Trino · dbt · Airflow · Snowflake · Kafka · DuckDB · PostgreSQL · MySQL · Delta/Parquet · partition & schema-evolution design · idempotent reprocessing · late-arriving data

**Cloud** — AWS (S3, Athena, Glue, EC2) · Docker · MinIO/object storage · AWS Certified Solutions Architect – Associate

**ML** — CatBoost · XGBoost · scikit-learn · SHAP · class-imbalance modeling · model calibration (Platt, isotonic) · time-series forecasting (SARIMA, Prophet) · MLflow

**Statistics & experimentation** — A/B testing · hypothesis testing · power analysis · difference-in-differences · Bayesian structural time series · causal impact analysis

**LLM & agentic systems** — LangGraph · LangChain · MCP (Model Context Protocol) · RAG · Ollama · LoRA fine-tuning · quantization · LLM-as-judge evaluation

**Languages & tools** — Python · SQL (Advanced) · R · FastAPI · Streamlit · Git · CUDA (basics)

---

## More projects

| Project | What it does | Stack |
|---|---|---|
| [**Clinverify**](https://github.com/Akashkumarsenthil/Clinical-Discharge-Treatment-Plan-Verification) | Neurosymbolic checker for LLM-generated clinical discharge plans. Compiles each plan into logic and tests it with an SMT solver, naming the broken rule when a plan fails. Runs on a synthetic stand-in, so the whole thing is reproducible without credentialed data. *(DATA 298A team project — I own the model track)* | Python, Z3, pandas |
| [**Healthcare Multi-Agent Copilot**](https://github.com/RitikaMNeema/Healthcare-Multi-Agent-Copilot) | Multi-agent copilot for claims-denial management: planner/executor/critic agents, hybrid keyword + vector retrieval with citation provenance checks, guardrails, human-in-the-loop approval, and an eval harness with a golden set. Fully reproducible offline against a deterministic mock LLM. | LangGraph, Python, synthetic data |
| [**SkillSync**](https://github.com/RitikaMNeema/SkillSync) | Three-tier distributed LinkedIn simulation — microservices, Kafka event streaming, and agentic AI workflows for hiring and analytics. *(group project)* | TypeScript, Kafka, microservices |
| [**NL2SQL**](https://github.com/RitikaMNeema/NL2SQL) | Conversational analytics over a cloud-hosted relational database: semantic query understanding, adaptive table selection, and LLM-driven SQL generation across 8+ tables. | LangChain, ChromaDB, Streamlit, Gemini |
| [**LiteGround RAG**](https://github.com/RitikaMNeema/liteground-rag) | Claim-level NLI verification plus targeted retrieval repair for RAG, evaluated fully locally on 80 QASPER questions. | Python, local NLI models |

---

## Graduate coursework

**DATA 266 · Generative AI** — built a mini-GPT from scratch; LoRA fine-tuning of LLMs and of Stable Diffusion 1.5; self-supervised learning (SimCLR / NT-Xent, rotation pretext) on STL-10; GANs and autoencoders; DDPM and latent diffusion from scratch; RAG with chunking, reranking and memory; CLIP zero-shot classification; GPTQ quantization and knowledge distillation; multi-agent pipelines; CUDA kernels for matmul. Also on a Kaggle competition team building an autonomous software-engineering agent on Gemma 4 (Google ADK) that localizes bugs and submits patches against hidden tests, SWE-bench style.

**DATA 255 · Deep Learning** — neural networks from first principles, optimization and initialization, regularization and generalization, CNNs, modern CNN architectures and transfer learning.

**DATA 298A · MS Project I** — leading a model track on neurosymbolic verification of LLM-generated clinical care plans (Team 6): formal rule catalog, SMT-based plan checking, and an evaluation harness on labeled plans.

**Previous semesters** — *DATA 226 Data Warehousing* (Snowflake, dbt, Airflow, Preset; Netflix and traffic pipelines) · *DATA 245 Machine Learning* (PaySim fraud modeling, model selection, imbalance handling) · *DATA 236 Distributed Systems* (microservices, Kafka, three-tier architecture) · *DATA 230 Data Visualization* · *DATA 220 Statistics & Data Mining*

---

## Education & certifications

**M.S., Applied Data Intelligence** — San José State University · expected May 2027  
**B.Tech, Electronics & Communication Engineering** — CHARUSAT · 2018–2022

AWS Certified Solutions Architect – Associate (2026) · Databricks GenAI Fundamentals · HackerRank SQL (Advanced)
