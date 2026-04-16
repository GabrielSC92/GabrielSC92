# Gabriel Silva Cheinquer

**Hybrid Data Scientist / Data Engineer** at Faz Capital (XP Investimentos)  
**MSc Applied Data Science** at Utrecht University

I build end-to-end data products: data modeling, ETL orchestration, feature engineering, predictive modeling, and production scoring workflows for business decisions.

---

## Current Focus

- **MSc Thesis:** *REM with Multiple Receivers*  
  Testing when multi-receiver event data can be transformed into dyadic form while preserving valid inference.  

- **Applied ML in production (Faz Capital):**  
  Churn risk systems with monthly scoring, monitoring, and retraining logic in Airflow + PostgreSQL.

---

## Selected Impact

### Client Churn Prediction (FBI-1058) - Productionized
Built and deployed an end-to-end client churn pipeline for ~13K clients with monthly scoring.

- Delivered XGBoost classification baseline around **AUC-ROC 0.75**
- Implemented 5-tier risk scoring for retention prioritization
- Deployed scoring + monitoring DAG chain:
  `refresh -> verify -> score -> backfill actuals -> monitor AUC -> retrain_if_drift`
- Added intervention logging architecture for future uplift/causal analysis

### Advisor Churn Prediction (FBI-2313) - In active development
Designed the advisor-side risk framework under rare-event constraints.

- Built advisor-month feature spine and materialized table (`rpt_advisor_churn_model`)
- Deployed monthly Airflow refresh pipeline with procedure-level quality controls
- Completed data quality, cleaning, and EDA phases with documented signal findings
- Framed outcome as a practical ranked risk watchlist with survival-analysis-compatible design

### Churn Modeling Framework (Faz Capital)
End-to-end modeling stack spanning R and Python for feature engineering, model selection, and business translation.

- Feature pipeline: temporal lags, momentum, ratio features, leakage-safe definitions
- Modeling workflow: VIF -> LASSO -> Stepwise AIC and tree-based models with Optuna
- Interpretation and decision support via SHAP and tiered risk outputs

---

## What I Do Best

- **Data engineering for analytics:** PostgreSQL modeling, temporal logic, robust ETL and Airflow orchestration
- **Predictive modeling in business settings:** strong baseline design, class-imbalance handling, leakage control, practical evaluation
- **Production-oriented analytics:** build systems that run monthly, generate actionable outputs, and can be monitored over time
- **Research-to-application translation:** bring academic rigor into deployable workflows

---

## Technical Stack

**Data Engineering:** PostgreSQL, Airflow, dbt, ETL pipelines, dimensional modeling  
**Modeling:** Python (XGBoost, LightGBM, Optuna, SHAP, scikit-learn), R (tidyverse, glmnet, R Markdown)  
**ML Systems:** feature pipelines, time-aware validation, drift monitoring, retraining triggers  
**Infra:** Docker, Git, SQLite/PostgreSQL

---

## Links

- [Thesis-MSc-ADS-REM](https://github.com/GabrielSC92/Thesis-MSc-ADS-REM)
- [INFOMTALC_Transformers_Research](https://github.com/GabrielSC92/INFOMTALC_Transformers_Research)
- [BSc Thesis - Roman Roads and Trade Costs](https://github.com/GabrielSC92/Thesis-Gabriel/tree/main)
