# Day 28 — Data Storytelling & Communicating Insights

**30-Day Data Analytics Cookbook | From Foundations to Real-World Impact**

> Data analytics is not about dashboards. It is about decisions.

## Overview

Day 28 explores how to turn analytical findings into a decision-ready narrative using evidence, visualizations, and actionable recommendations. The notebook uses **synthetic municipal citizen-grievance data**; it does not represent actual Greater Chennai Corporation performance.

## Learning objectives

- Structure a data story: **What happened? Why does it matter? What should we do next?**
- Calculate complaint intake, resolution throughput ratios, and monthly net inflow.
- Design annotated line and bar charts with insight-led headlines.
- Identify priority zones and categories for further investigation.
- Create a concise executive briefing with an owner, action, and measurable KPIs.
- Communicate uncertainty, assumptions, and metric limitations.

## Notebook

[`Day_28_Data_Storytelling_Communicating_Insights.ipynb`](Day_28_Data_Storytelling_Communicating_Insights.ipynb)

### Contents

1. Generate a six-month synthetic complaint dataset.
2. Calculate performance indicators and compare January with June.
3. Plot complaint intake vs. resolution with an annotation.
4. Visualize monthly resolution throughput against an illustrative target.
5. Rank zones by net inflow and inspect complaint categories.
6. Produce an executive management briefing.
7. Complete five hands-on exercises.

## Requirements

- Python 3.10+
- Jupyter Notebook or JupyterLab
- pandas, numpy, matplotlib, IPython

```bash
python -m pip install jupyter pandas numpy matplotlib ipython
jupyter notebook Day_28_Data_Storytelling_Communicating_Insights.ipynb
```

Run cells from top to bottom. No external dataset, credentials, or database is required.

## Example insight

In the **illustrative** dataset, monthly complaint intake rises from **1,200 to 1,600 (+33.3%)** between January and June. June resolutions total **1,400**, yielding a **monthly throughput ratio of 87.5%** and a **net inflow of 200 cases**. The proposed management response is to investigate zones with the highest net inflow, review case age and bottlenecks, and track weekly outcomes.

**Important:** The monthly throughput ratio is not the same as a cohort resolution rate. Monthly received minus resolved is not automatically the verified backlog; a backlog calculation needs opening pending cases and other adjustments. A target of 95% is illustrative, not an official service standard.

## Practical applications

- Citizen grievance monitoring and management briefings
- Service-delivery review meetings
- Resource allocation and operational follow-up
- Ward/zone performance reporting

## Suggested repository structure

```text
Day_28/
├── Day_28_Data_Storytelling_Communicating_Insights.ipynb
└── README.md
```

## Key takeaway

**A strong data story connects a trustworthy observation to an actionable decision and a measurable result.**

**Next:** Day 29 — Building an End-to-End Data Analytics Project.
