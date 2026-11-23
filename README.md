# E-commerce Customer Behaviour Analytics

**HCLTech Career Shaper Programme · III Year Industry Project No. 51 · 2025-26**
Learner: Shivani · ABES Engineering College

Analysis of 500 e-commerce clickstream sessions: conversion funnel, page/device behaviour, time on page, data-quality audit, hypothesis tests and a predictive check.

## Live dashboard
Streamlit app: **<https://ecommerce-customer-behavior-analytics-alozebnhqjqcw6eaordr6f.streamlit.app/>**

## Key findings
- Add-to-cart rate **35.0%** (matches the 35% reference); cart → purchase **18.3%** vs 68% reference.
- **30.2%** of sessions contain logical contradictions (e.g. purchase without add-to-cart).
- Device, page type and time on page show **no statistically significant** link to purchase (all p > 0.17); models score ROC-AUC 0.47-0.52 (chance level).

## Repository contents
| File | Purpose |
|---|---|
| `app.py` | Streamlit dashboard (filters, funnel, page/device, time, data quality, tests) |
| `ecommerce_analysis.py` | Full analysis script (cleaning, 7 figures, tests, SQL, models) |
| `EDA_Notebook.ipynb` | Same analysis as an executed Jupyter notebook |
| `dataset.csv` | Source data (500 sessions, 8 columns) |
| `dataset_cleaned.csv` | Cleaned data with validation flags and derived features |
| `data_dictionary_completed.csv` | All 16 columns described |
| `docs/` | Project report and synopsis (Word) |

## Run locally
```bash
pip install -r requirements.txt
streamlit run app.py          # dashboard
python ecommerce_analysis.py  # analysis script (writes figs/, dataset_cleaned.csv)
```

## Privacy (DPDP Act 2023)
`user_id` is a pseudonymous token; no names, e-mails, phone numbers or IPs are used. Data was provided by the programme for learning.

## Tools
Python, pandas, NumPy, SciPy, scikit-learn, Matplotlib, Seaborn, Plotly, SQLite, Streamlit, Jupyter.
