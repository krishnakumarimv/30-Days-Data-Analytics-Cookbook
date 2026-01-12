# Day 05 – Data Quality Analytics  
## Accuracy, Completeness, Timeliness, Consistency

This folder contains the **Day 5 analytics cookbook** from the  
**30-Day Data Analytics Series**.

Day 5 focuses on a foundational truth that is often overlooked:

**Most analytics failures are caused by poor data quality, not poor models.**

## Why Data Quality Matters

Dashboards, reports, and forecasts can look impressive.  
But if the underlying data is:

- inaccurate,
- incomplete,
- outdated, or
- inconsistent,

then decisions based on that data are unreliable.

Data quality is therefore **not a technical hygiene task**.  
It is a **decision risk management activity**.

## Dataset Used

**NYC 311 Service Requests**  
Source: Kaggle  

This dataset closely resembles:
- municipal grievance redressal systems,
- public service request portals,
- large-scale operational databases.

As a result, it exposes real-world data quality challenges seen in production systems.

## Notebook Included

### `Day_05_Data_Quality_Analytics_Cookbook.ipynb`

This notebook demonstrates practical, auditable data quality checks, including:

- Scoping data to decision-relevant columns
- Accuracy checks (invalid or malformed values)
- Completeness analysis (missing critical fields)
- Timeliness assessment (decision-window relevance)
- Consistency checks (category stability)
- Duplicate record detection
- Data quality metrics summary

The approach is **tool-light, model-free, and decision-oriented**.

## Key Concepts Demonstrated

- Data quality as a governance issue
- Why analytics fails without trustworthy data
- Measuring data quality before measuring performance
- Simple checks that prevent major analytics failures

## How This Scales

The same data quality framework applies to:
- grievance redressal platforms,
- waste management systems,
- utility service databases,
- revenue and inspection systems.

Only column names change.  
The analytics logic remains the same.

## Series Context

Day 5 completes the **foundation phase** of the series.

From Day 6 onward, the focus shifts toward:
- analytics skills,
- exploratory analysis,
- feature engineering,
- forecasting and decision support,

all built on **trusted data**.

## License / Usage

This notebook is shared for **learning, adaptation, and public-sector analytics practice**.  
Attribution is appreciated.

