# Gabriel Silva Cheinquer

**Data Engineer** at Faz Capital · **MSc Applied Data Science** at Utrecht University

---

## Professional Work

I work as a Data Engineer at [Faz Capital](https://fazcapital.com.br), a subsidiary of XP Investimentos. I build and maintain the data infrastructure behind financial analytics and reporting.

**Core responsibilities:**
- Designing and optimizing PostgreSQL databases with complex temporal data structures (SCD Type 2, date-range overlaps, incremental refresh)
- Building ETL pipelines for commission processing and financial data integration
- Implementing dimensional models and client-level reporting tables
- Developing BI dashboards and reporting infrastructure

**Recent project — Client churn prediction (Faz Capital):** End-to-end predictive system for ~13K PF clients across 7 months of data. PostgreSQL materialized table with stored procedure and Airflow DAG for monthly refresh. Feature engineering pipeline in R (29 features across 8 categories: temporal lags, NPS sentiment, advisor aggregates, custody ratios, interaction terms) with VIF → LASSO → Stepwise AIC consensus selection and linear baseline. Lead-target reframe (predict next month's churn from this month's full state) to solve a temporal leakage issue in the original design. Phase 6 modeling in Python: XGBoost, LightGBM, and Random Forest with GPU-accelerated Optuna tuning (native API, early stopping, Hyperband pruning), three modeling approaches (regression, binary classification, two-stage), and SHAP interpretation. Classification AUC-ROC of 0.75 - the primary deliverable for advisor retention outreach. Key finding: NPS scores add no predictive value beyond financial behavior signals.

---

## Academic & Projects

MSc in Applied Data Science at Utrecht University; BSc in Economics with a data science specialization from the same institution.

**Current coursework (Period 3):** Transformers: Applications in Language and Communication · Human Network Analysis

**Recent work:** Recurrent transformer for **chess move prediction** (PyTorch): custom encoder with From/To prediction heads and shared recurrent blocks, trained from scratch on engine-generated data. Built for the INFOMTALC tournament; model on [Hugging Face](https://huggingface.co/Izzent/recurrent-transformer-chess).

**Quality of Dutch Government** (DSPG, Period 2): Full-stack RAG application for Utrecht University's Institute for Government Quality Research. Built a document ingestion pipeline (PyMuPDF → chunking → LLM summarization → topic classification), a 4-level retrieval hierarchy with agent-based query routing, and a Streamlit interface with dual views (citizen chat + researcher dashboard with data tables, Plotly visualizations, and export). Local LLM deployment via Ollama (Llama 3.2), SQLite/PostgreSQL backend, user-normalized satisfaction metrics to prevent survey skewing, and a custom Response Quality Score for verification. Privacy-first: no raw chat stored, only anonymized topic summaries.

**Earlier coursework:** Causal inference methods (DAGs, IPW, propensity scores, doubly robust estimators, marginal structural models) applied to workplace analytics. Policy analysis using intersectionality frameworks and fairness evaluation for public governance.

**BSc thesis — [The Historical Impact of Roman Roads on French Trade Costs](https://github.com/GabrielSC92/Thesis-Gabriel/tree/main):** 2SLS instrumental variable analysis using Roman road density (117 CE) as an instrument for modern French road infrastructure to identify the causal effect on bilateral trade costs and volumes across 94 departments × 13 EU14 partners. Gravity model trade costs (Novy 2013), spatial data processing (shapefiles, CRS transformations, density calculations), and robustness checks across elasticity values and model specifications. Supervised by Bas Machielsen.

Interests: quantitative methods, causal inference, data engineering, and turning research ideas into scalable systems.

---

## Technical Stack

**Databases:** PostgreSQL, dimensional modeling, temporal data architecture (SCD Type 2), incremental refresh patterns  
**Data engineering:** ETL pipelines, data quality frameworks, stored procedures, Airflow DAGs, dbt  
**Analytics:** BI dashboards, financial reporting, Streamlit  
**ML / modeling:** Python (XGBoost, LightGBM, Optuna, SHAP, scikit-learn, pandas), R (tidyverse, glmnet, Rmd reporting), feature engineering, temporal CV, leakage control  
**Deep learning / NLP:** PyTorch, transformer architectures, RAG pipelines, Ollama/Llama local deployment  
**Infrastructure:** Docker, Git, SQLite/PostgreSQL, Airflow
