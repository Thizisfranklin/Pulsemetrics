# PulseMetrics — Product Metrics Layer + Root-Cause Copilot

> This project is currently in active development

PulseMetrics is an e-commerce product analytics system that standardizes KPI definitions, monitors funnel and revenue performance, detects unusual metric movement, and helps investigate likely root causes faster.

## Business Problem
E-commerce teams often struggle with inconsistent KPI definitions, slow root-cause investigations, and dashboards that show what changed but not why it changed. PulseMetrics was built to create a shared metrics layer, detect unusual KPI movement, and guide investigation into likely causes.

## Project Goal
Build an end-to-end metrics and monitoring workflow that:
- standardizes core e-commerce KPIs
- validates data quality
- detects metric anomalies
- supports root-cause investigation
- provides rule-based and later LLM-assisted explanations

## Core Features
- KPI metrics layer for funnel, retention, and revenue metrics
- SQL-based metric definitions
- data quality checks
- anomaly detection for KPI shifts
- root-cause drilldowns by segment
- rule-based copilot suggestions
- optional LLM explanation layer
- dashboard / visualization layer

## KPI Coverage
Initial KPIs include:
- Conversion Rate
- Add-to-Cart Rate
- Checkout Completion Rate
- Average Order Value
- Cart Abandonment Rate
- Repeat Purchase Rate

## Tech Stack
- SQL
- Python
- PostgreSQL
- Pandas
- Streamlit
- Power BI
- Git/GitHub

### Planned Additions
- LLM-generated explanations
- automatic SQL suggestions
- natural-language investigation summaries
- Docker
- dbt
- Tableau

## Dataset
This project uses an e-commerce event and transaction dataset with tables for:
- users
- sessions
- events
- orders
- products
- channels

## Project Structure
```text
[pulsemetrics/
│
├── README.md
├── requirements.txt
├── .gitignore
├── data/
│   ├── raw/
│   └── processed/
│
├── sql/
│   ├── schema.sql
│   ├── metrics.sql
│   ├── data_quality_checks.sql
│   └── anomaly_queries.sql
│
├── notebooks/
│   ├── 01_exploration.ipynb
│   ├── 02_kpi_analysis.ipynb
│   └── 03_root_cause_analysis.ipynb
│
├── src/
│   ├── ingest_data.py
│   ├── metrics_layer.py
│   ├── dq_checks.py
│   ├── anomaly_detection.py
│   ├── root_cause_rules.py
│   └── llm_explanations.py
│
├── app/
│   └── streamlit_app.py
│
├── docs/
│   ├── kpi_dictionary.md
│   ├── architecture.png
│   └── case_study.md
│
└── dashboard/
    └── powerbi_screenshots/]
