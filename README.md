# Manufacturing Process Analytics
> Stage 1 of the "Data-Driven Engineering & Decision Making" portfolio.

[![View Report](https://img.shields.io/badge/View-Live_HTML_Report-blue)](https://tsl4yer.github.io/manufacturing-process-analytics/reports/reports.html)
[![Python](https://img.shields.io/badge/Python-3.9+-yellow)](#)
[![License: MIT](https://img.shields.io/badge/License-MIT-green)](#)

## Summary
Analyzed 10,000 machine operation cycles from the AI4I 2020 Predictive Maintenance dataset to identify root causes of equipment failure. Applied feature engineering (mechanical power, thermal gradient), statistical driver analysis, and decision tree modeling to rank failure predictors. 

Headline result: Rotational speed (RPM), tool wear, and mechanical power accounted for over 80% of predictive model decisions; the mechanical failure rate escalated to 15.5% once a tool entered the critical wear stage.

## Key Findings
- **Overstrain** was **70.6%** higher in failed runs than normal runs (p < 0.001)
- Failure rate escalates from **2.09%** (High Grade) to **15.5%** (Critical wear stage)
- **Heat Dissipation Failure (HDF)** accounts for **33.9%** of all machine failures
- MTBF proxy: **29** cycles between failures

## Tech Stack
Python · pandas · numpy · scikit-learn · Plotly · Seaborn · Quarto

## Results
| Metric | Value |
|--------|-------|
| Dataset size | 10,000 × 14 |
| Overall failure rate | 3.39% |
| MTBF proxy | 29 cycles |
| Dominant failure mode | HDF (33.9% of failures) |
| Decision tree ROC-AUC | 0.9047 |
| Critical-wear failure rate | 15.5% |

## How to Run
```bash
pip install -r requirements.txt
jupyter notebook notebooks/analysis.ipynb
