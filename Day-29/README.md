# Day 29 — Building an End-to-End Data Analytics Project

**30-Day Data Analytics Cookbook | From Foundations to Real-World Impact**

## Overview

This capstone-style exercise demonstrates a reproducible **synthetic citizen-grievance analytics project**. It connects a municipal service-delivery question to data generation, quality assurance, cleaning, KPI analysis, exploratory visualization, forecasting baseline evaluation, and a management brief.

> **Data analytics is not about dashboards. It is about decisions.**

## Learning objectives

- Translate operational questions into measurable KPIs.
- Create and validate synthetic grievance data without using personal information.
- Detect duplicate IDs, invalid dates, and inconsistent closure records.
- Calculate intake, resolved, pending, and resolution-time measures.
- Compare monthly registrations and actual monthly closures correctly.
- Prioritize zones and complaint categories by unresolved workload.
- Evaluate a one-month-lag forecasting baseline on a chronological holdout.
- Present a concise executive briefing with actions and limitations.

## Project files

```text
Day_29/
├── README.md
└── Day_29_End_to_End_Data_Analytics_Project.ipynb
```

The notebook automatically creates `day29_outputs/` containing:

| Output | Description |
|---|---|
| `synthetic_grievances_raw.csv` | Synthetic records including injected quality issues |
| `synthetic_grievances_clean.csv` | Validated analysis dataset |
| `quality_audit.csv` | Data-quality counts |
| `kpi_summary.csv` | Executive KPIs |
| `monthly_summary.csv` | Intake, closures, and monthly net flow |
| `zone_summary.csv` | Zone-level workload and performance |
| `category_summary.csv` | Complaint-type workload and performance |
| `registration_cohorts.csv` | Resolution outcomes by registration cohort |
| `forecast_metrics.csv` | Naive forecast MAE, RMSE, and bias |
| `monthly_received_closed.png` | Monthly trend chart |
| `pending_by_zone.png` | Priority-zone visualization |
| `forecast_holdout.png` | Holdout forecast comparison |
| `executive_brief.md` | Automatically generated management briefing |

## Installation

Requires Python 3.10+.

```bash
python -m pip install pandas numpy matplotlib scikit-learn jupyter
jupyter notebook
```

Open `Day_29_End_to_End_Data_Analytics_Project.ipynb` and run all cells in order. The data is generated locally using a fixed random seed, so no external dataset or API is required.

## Analytics workflow

1. **Business understanding:** Define questions and KPIs.
2. **Synthetic data generation:** Simulate 24 months of grievance registrations and closure outcomes.
3. **Quality assurance:** Audit duplicates, malformed registration dates, and inconsistent closure dates.
4. **Data preparation:** Standardize statuses, dates, and derived features.
5. **KPI analysis:** Calculate volume, pending cases, resolution rate, and resolution durations.
6. **EDA:** Examine monthly trends, zone-wise pending workload, and complaint categories.
7. **Model evaluation:** Compare a naive forecast with actual volumes in a six-month holdout.
8. **Decision support:** Export a concise management brief with practical next steps.

## KPI interpretation

- **Resolution rate** = resolved registered complaints / all registered complaints × 100, measured at the fixed observation cutoff.
- **Pending** = registered complaints not resolved by that cutoff.
- **Resolution days** = closure date minus registration date for valid resolved cases.
- **Monthly received** counts registration dates; **monthly closed** counts closure dates. Their difference is a monthly net flow, **not** a direct measurement of the outstanding backlog.
- Recent registration cohorts have had less time to close, so cohort comparisons must account for censoring.

## Model evaluation

The notebook uses a one-month-lag naive baseline and evaluates MAE, RMSE, and signed forecast bias on the final six months. The baseline is intentionally simple; stronger projects should compare seasonal-naive and more advanced methods on equivalent chronological backtests.

## Suggested exercises

1. Add age-bucketed pending workload and zone-by-category analysis.
2. Implement a seasonal-naive forecasting baseline and compare its holdout errors.
3. Add automated quality tests and a data dictionary.
4. Prepare a one-page briefing for an urban local body with three insights and three evidence-based actions.

## Limitations and privacy

**All records are synthetic.** No findings describe actual ULB performance. The exercise simplifies workflow states and does not model reopened grievances or all possible service-level rules. Do not upload personal citizen information, addresses, mobile numbers, or complaint narratives to public repositories.

## Repository

[30-Days-Data-Analytics-Cookbook](https://github.com/krishnakumarimv/30-Days-Data-Analytics-Cookbook)

**Next: Day 30 — Final Capstone, Portfolio Building & the Road Ahead.**
