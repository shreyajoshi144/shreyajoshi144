<div align="center">

# Shreya Joshi

### Data & AI Engineer | Data Engineering · Agentic AI · Machine Learning

Final-year Computer Science student building data pipelines, AI applications, and machine learning systems with Python and SQL.

**[LinkedIn](https://www.linkedin.com/in/shreya-joshi144) · [GitHub](https://github.com/shreyajoshi144) · [Email](mailto:shreyaajoshi88@gmail.com)**

</div>

<br>

## About

I'm a final-year B.Tech Computer Science and Engineering student at Medicaps University, graduating in 2026.

My work sits across **data engineering, applied AI, and machine learning**. I enjoy building systems where data has to move reliably, models need to be evaluated rather than just trained, and AI outputs need context or guardrails before they are trusted.

That has led me to work on:

* ETL pipelines with validation, data-quality monitoring, and drift detection
* Agentic AI systems with controlled tool access and retrieval
* Natural-language analytics with SQL validation and reliability signals
* Machine learning and recommendation systems with explicit evaluation
* NLP applications for sentiment and meeting intelligence

I am particularly interested in the engineering problems between **data, machine learning, and AI systems**—where retrieval quality, data reliability, model evaluation, validation, and system design directly affect the usefulness of the final product.

Currently seeking **Data Engineer, AI Engineer, Applied AI, and Machine Learning Engineer opportunities for 2026**.

<br>

## Technical Skills

| Area                     | Technologies                                                                                                                |
| ------------------------ | --------------------------------------------------------------------------------------------------------------------------- |
| **Languages & Data**     | Python, SQL, Pandas, NumPy                                                                                                  |
| **Data Engineering**     | ETL/ELT, Data Pipelines, Data Ingestion, Transformation, Data Validation, Data Quality, Data Modeling, Data Drift Detection |
| **Machine Learning**     | scikit-learn, Feature Engineering, Model Evaluation, TF-IDF, Collaborative Filtering, Matrix Factorization                  |
| **AI & Agentic Systems** | LLMs, RAG, LangChain, LangGraph, AI Agents, Tool Calling, Embeddings, Vector Search, ChromaDB                               |
| **Backend & Databases**  | FastAPI, REST APIs, MySQL, PostgreSQL, SQLite, DuckDB, SQLAlchemy, Redis, JWT Authentication                                |
| **Cloud & Engineering**  | AWS (EC2, S3, RDS, IAM, VPC), Docker, Git/GitHub, pytest, Logging & Monitoring, Streamlit                                   |
| **Data Platforms**       | Azure Data Factory, Azure Data Lake Storage Gen2, Databricks, Apache Spark, PySpark                                         |

<br>

# Featured Work

## InnoVista — AI-Assisted Data Reliability Platform

[GitHub →](https://github.com/shreyajoshi144/innovista-data-platform)

A production-style data pipeline for live weather data, built around validation, observability, and controlled AI-assisted investigation.

The pipeline processes weather data across **20 Indian cities** through ingestion, validation, MySQL storage, and drift detection. It includes **6 independent validation rules** and z-score-based drift detection against a rolling **7-day baseline**.

On top of the deterministic pipeline, an investigation agent can call **8 whitelisted, read-only tools** to gather evidence about pipeline and data-quality issues. The LLM does not directly query or modify the database.

The investigation output separates:

`Observation → Evidence → Hypothesis → Limitation → Next Step`

The project also includes **67 offline unit tests**, integration smoke tests, and a **4-page Streamlit dashboard** for monitoring and investigation.

`Python` · `SQL` · `MySQL` · `AWS S3` · `Streamlit` · `Anthropic API`

---


## Atlas — Agentic Research Workspace

[GitHub →](https://github.com/shreyajoshi144/atlas)

An agentic research system designed to move from a research question to evidence-backed output through a structured workflow.

Atlas uses a **10-step LangGraph pipeline** covering search, scraping, evidence extraction, verification, credibility scoring, and report generation.

Source selection combines deterministic ranking methods including:

* BM25
* TF-IDF
* Cosine similarity
* Fuzzy matching

LLM calls are limited to stages where language understanding is actually required. Previous research is indexed in ChromaDB for semantic retrieval and follow-up RAG-based interaction.

`LangGraph` · `LangChain` · `ChromaDB` · `FastAPI` · `LLMs`

---

## QuerySure — Trust-First Natural Language Analytics

[GitHub →](https://github.com/shreyajoshi144/querysure)

A natural-language analytics system designed around the idea that generating SQL is only one part of answering a data question reliably.

QuerySure retrieves relevant schema context before generation, validates generated SQL before execution, and enforces read-only analytical access.

The platform includes:

* TF-IDF-based schema retrieval
* SQL validation with SQLGlot
* JWT authentication and per-user data isolation
* PostgreSQL persistence through SQLAlchemy
* Redis-backed rate limiting
* LLM budget tracking
* Data reliability checks for completeness, freshness, integrity, drift, and uniqueness
* Alembic-managed database migrations
* Docker Compose for reproducible local development

`Python` · `SQL` · `FastAPI` · `PostgreSQL` · `Redis` · `Docker` · `SQLGlot` · `TF-IDF`

---

## HealthGuard — Patient Feedback Intelligence

[GitHub →](https://github.com/shreyajoshi144/healthguard)

A patient-feedback intelligence application that analyzes healthcare reviews and adds reliability checks around NLP/ML predictions.

The project uses **TF-IDF and spaCy semantic-embedding classifiers** and includes **confidence calibration, entropy-based uncertainty measurement, out-of-distribution detection, and model-disagreement checks** to provide additional signals about prediction reliability.

The application is supported by a **FastAPI backend** with **JWT-secured workspace APIs**.

`Python` · `scikit-learn` · `NLP` · `TF-IDF` · `spaCy` · `Pandas` · `NumPy` · `FastAPI` · `JWT`

---

## ShopScope — Azure Data Engineering Pipeline

[GitHub →](https://github.com/shreyajoshi144/ShopScope)

A cloud data engineering project that processes the **Olist Brazilian e-commerce dataset** across Azure Data Factory, Azure Data Lake Storage Gen2, and Azure Databricks.

The completed pipeline ingests **9 relational e-commerce datasets** into a layered cloud storage structure, including datasets with **99K+ orders, 112K+ order items, and over 1 million geolocation records**. Raw data is validated in Databricks before transformation using **six data-quality rule categories**, including null, duplicate, schema, value-range, and completeness checks. Critical failures halt downstream processing, while warnings are logged for review.
Validated datasets are then joined, enriched, and aggregated into an **order-level master transactions table** containing customer, product, payment, review, delivery, and revenue information.

**Current implementation:** Azure Data Factory ingestion, ADLS Gen2 storage layout, Databricks validation, and master-table transformation are complete. Delta Lake persistence and Apache Airflow orchestration are the next stages of the project.

`Azure Data Factory` · `Azure Data Lake Storage Gen2` · `Azure Databricks` · `Apache Spark` · `PySpark` · `Python` · `SQL`

---

---

# AI Applications

## Notiv — Voice-to-Insight Meeting Intelligence

[GitHub →](https://github.com/shreyajoshi144/notiv)

A meeting intelligence pipeline that converts recordings into structured and searchable outputs.

The system supports:

* English transcription with Whisper
* Hinglish transcription with Sarvam AI
* Map-reduce summarization
* Action-item extraction
* Decision extraction
* RAG-based chat over meeting transcripts

Meeting content is indexed using ChromaDB and sentence-transformer embeddings for semantic retrieval.

`Whisper` · `Sarvam AI` · `LangChain` · `ChromaDB` · `Sentence Transformers` · `RAG`

---

## Verdict — AI Shopping Intelligence Platform

[GitHub →](https://github.com/shreyajoshi144/verdict)

A shopping comparison application combining product comparison and LLM-assisted buying analysis.

The platform includes side-by-side comparison, budget planning, and JWT-based user authentication.

`FastAPI` · `Python` · `Groq` · `JWT Authentication`

<br>

# Machine Learning

## Valora — Hybrid Movie Recommendation Engine

[GitHub →](https://github.com/shreyajoshi144/valora-movie-recommendation-engine) · [Live Demo →](https://valora-movies.streamlit.app/)

A machine-learning recommendation system combining multiple recommendation strategies rather than relying on a single model.

Valora brings together:

* **Content-based filtering** using TF-IDF and cosine similarity
* **Item-item collaborative filtering**
* **Matrix factorization** using Truncated SVD

The strategies are blended into a hybrid recommendation approach and evaluated across **six strategies**.

Evaluation uses:

* Precision@K
* Recall@K
* Hit Rate
* RMSE

The project also includes a **per-user chronological train/test split** to reduce temporal leakage during evaluation, along with cold-start fallback and popularity-bias mitigation.

This is the project where I worked most directly with the full ML workflow—from recommendation strategy design and feature representation to evaluation methodology and metric comparison.

`Python` · `scikit-learn` · `TF-IDF` · `Cosine Similarity` · `Collaborative Filtering` · `Truncated SVD` · `Streamlit`


---



# How My Work Connects

```text
                    Data
                     │
        ┌────────────┼────────────┐
        │            │            │
        ▼            ▼            ▼
   Data Pipelines  Machine       AI Systems
                  Learning
        │            │            │
        ▼            ▼            ▼
   InnoVista      Valora        Atlas
   ShopScope      HealthGuard   QuerySure
                                Notiv
                                Verdict
        │            │            │
        └────────────┴────────────┘
                     │
                     ▼
          Reliable, usable systems
```

The common thread across these projects is not one specific framework.

It is working with the stages around the core model or AI call:

```text
Data
  ↓
Preparation
  ↓
Retrieval / Modeling / Analysis
  ↓
Evaluation or Validation
  ↓
Application Layer
  ↓
Monitoring or Reliability Checks
```

Depending on the project, that means validating incoming records, designing leakage-aware evaluation, ranking retrieval results, restricting AI tool access, validating generated SQL, or monitoring data drift.

<br>

# Experience

## Data Analyst Program Trainee — HCLTech

**January 2026 – May 2026**

Completed a **240-hour Data Analyst program** focused on strengthening practical foundations in Python, SQL, and data-processing workflows.

Applied these foundations directly while developing **HealthGuard**, a patient-feedback intelligence project. The work expanded beyond sentiment analysis into a reliability-focused NLP/ML pipeline.

Key work included:

* Building reliability checks around **TF-IDF and spaCy semantic-embedding classifiers**
* Implementing **confidence calibration** and **entropy-based uncertainty measurement**
* Adding **out-of-distribution detection** to identify inputs that differ from the model's expected data distribution
* Implementing **model-disagreement checks** as an additional reliability signal
* Serving the application through a **FastAPI backend**
* Adding **JWT-secured workspace APIs**
* Working with **scikit-learn, Pandas, and NumPy** for the data-processing and ML workflow

`Python` · `SQL` · `scikit-learn` · `NLP` · `Pandas` · `NumPy` · `FastAPI` · `JWT`

---

## AWS Academy Cloud Trainee

**AWS Academy × Medicaps University**
**June 2025 – July 2025**

Completed hands-on cloud training covering the core components used in cloud-based application architecture:

* **Amazon EC2** — compute and virtual servers
* **Amazon S3** — object storage
* **Amazon RDS** — managed relational databases
* **AWS IAM** — access and permission management
* **Amazon VPC** — cloud networking and resource isolation

Completed:

* **AWS Academy Cloud Foundations**
* **AWS Academy Cloud Architecting**

These programs provided hands-on exposure to how compute, storage, databases, networking, and identity management work together in cloud application architectures.

[View AWS Academy credentials on Credly →](https://www.credly.com/users/shreya-joshi144)

---

## Research Publication

### Optimizing Recycling Stream Sorting Systems Using Machine Learning to Minimize Contamination

**IJSRET · Vol. 11, Issue 1 · January–February 2025**

[Read the publication →](https://ijsret.com/wp-content/uploads/2025/01/IJSRET_V11_issue1_198.pdf)

Published research exploring the application of machine learning to improve recycling stream sorting and reduce contamination.

The work focused on applying and evaluating machine-learning approaches for a practical classification problem, contributing to my interest in applied ML systems where model performance is connected to measurable operational outcomes.

### Open to Data, AI & Machine Learning Engineering Opportunities

[LinkedIn](https://www.linkedin.com/in/shreya-joshi144) · [GitHub](https://github.com/shreyajoshi144) · [Email](mailto:shreyaajoshi88@gmail.com)

</div>
