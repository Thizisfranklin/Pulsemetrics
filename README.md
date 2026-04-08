# Pulsemetrics - Product Intelligence & Experimentation System

> This project is currently in active development

**The Business Problem:**  
In product-driven tech companies, distinguishing between statistical noise and true feature impact is critical. When a KPI increases by 1% during an A/B test, relying on basic averages often leads to false positives, wasted engineering time, and poor "ship-or-hold" decisions.

**The Solution:**  
Pulsemetrics is an end-to-end product analytics and experimentation engine designed to monitor performance, evaluate A/B tests, and optimize monetization. It moves beyond isolated analysis by connecting raw user behavior to rigorous statistical testing, enabling data-driven product strategy and clear execution decisions.

## Core Modules

The system is structured into modular components, each responsible for a core part of product analysis and decision-making.

---

### 📊 Metrics Engine (`metrics.py`)
Defines and standardizes core product KPIs such as conversion, retention, and revenue per user using SQL and Python transformations.

- Builds consistent metric definitions across analyses  
- Tracks funnel performance and user behavior  
- Serves as the foundation for all downstream analysis  

---

### 🧪 Experimentation Suite (`experiments.py`)
Processes A/B and multivariate experiment data to evaluate the impact of product changes.

- Applies statistical testing (t-tests, confidence intervals)  
- Measures lift and computes p-values  
- Supports clear ship-or-hold product decisions  

---

### 💰 Pricing & Monetization (`pricing.py`)
Analyzes how pricing strategies, discounting, and segmentation influence conversion, demand, and revenue outcomes.

- Evaluates pricing elasticity and user response  
- Identifies underpricing and overpricing opportunities  
- Supports monetization and revenue optimization decisions  

---
## Tech Stack
- SQL
- Python
- PostgreSQL
- Pandas
- Streamlit
- Git/GitHub

### Planned Additions
- LLM-generated explanations
- automatic SQL suggestions
- natural-language investigation summaries
- Power BI

## Project Structure
```text
[pulsemetrics/
│
├── data/
├── notebooks/
├── src/
│   ├── metrics.py
│   ├── experiments.py
│   ├── pricing.py
│
├── app/
│   └── streamlit_app.py
│
├── README.md ]


