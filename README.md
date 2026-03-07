# Gabriel Silva Cheinquer

**Data Engineer** at Faz Capital · **MSc Applied Data Science** at Utrecht University

---

## Professional Work

I work as a Data Engineer at [Faz Capital](https://fazcapital.com.br), a subsidiary of XP Investimentos. I build and maintain the data infrastructure behind financial analytics and reporting.

**Core responsibilities:**
- Designing and optimizing PostgreSQL databases with complex temporal data structures (SCD Type 2, date-range overlaps, incremental refresh)
- Building ETL pipelines for commission processing and financial data integration
- Implementing dimensional models and client-level reporting tables (e.g. churn at client × advisor × month granularity)
- Developing BI dashboards and reporting infrastructure

**Recent project — Churn predictive system (Faz Capital):** End-to-end pipeline for client-level churn prediction: PostgreSQL table and stored procedure with incremental refresh, Airflow DAG, feature engineering (temporal lags, NPS integration, advisor aggregates), and a modeling baseline in Python (XGBoost, LightGBM, Random Forest) with Optuna tuning, SHAP interpretation, and strict leakage control (BOM/lagged features only). Delivered DQA, EDA, and phase documentation in a structured tracker.

---

## Academic & Projects

MSc in Applied Data Science at Utrecht University; BSc in Economics with a data science specialization from the same institution.

**Recent work:** Recurrent transformer for **chess move prediction** (PyTorch): custom encoder with From/To prediction heads and shared recurrent blocks, trained from scratch on engine-generated data. Built for the INFOMTALC tournament; model on [Hugging Face](https://huggingface.co/Izzent/recurrent-transformer-chess).

Interests: quantitative methods, data engineering, and turning research ideas into scalable systems.

---

## Technical Stack

**Databases:** PostgreSQL, dimensional modeling, temporal data architecture, incremental refresh patterns  
**Data engineering:** ETL pipelines, data quality (DQA), migrations, Airflow DAGs  
**Analytics:** BI, dashboards, financial reporting  
**ML / research:** Python (pandas, scikit-learn, XGBoost, LightGBM, Optuna, SHAP), R (Rmd reports), PyTorch, transformers, training and deploying small models
