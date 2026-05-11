# Day 12 – Handling Missing Data
## Why Missing Data Is an Analytical Problem, Not Just a Technical Issue

Many beginners treat missing data as a minor inconvenience.

In reality, missing data is one of the most important analytical risks in practical analytics.

Poor handling of missing values can:

- Distort trends
- Bias conclusions
- Mislead dashboards
- Damage model reliability
- Hide operational failures

This chapter explores how analysts should understand, investigate, and handle missing data using the NYC 311 Service Requests dataset.

---

# Dataset Context

**Dataset:** NYC 311 Service Requests (Kaggle)  
**Domain:** Citizen complaints / service operations / urban governance

This dataset contains multiple real-world missing value situations:

- Missing closure dates
- Incomplete location information
- Partial agency fields
- Missing geographic coordinates
- Inconsistent operational records

---

# Objectives of This Chapter

This notebook and analysis aim to illustrate:

- Types of missing data
- How missingness affects analysis
- Why deletion can distort conclusions
- Practical missing value handling techniques
- When to drop, fill, or preserve missing data

---

# Notebook Contents

The accompanying Python script demonstrates:

✔ Identifying missing values  
✔ Measuring missingness percentages  
✔ Visualizing missing data patterns  
✔ Dropping missing values carefully  
✔ Filling missing values using defaults or statistics  
✔ Preserving analytically meaningful missingness  
✔ Creating missing-value indicator flags  

---

# Key Lessons

## Missing Data Is Often Informative

Missingness may indicate:

- Delays
- Failures
- Human behavior
- Process inefficiency

---

## Deleting Rows Can Distort Reality

Removing incomplete records may unintentionally remove:

- High-risk cases
- Delayed operations
- Exceptional events

---

# Files Included

- `day12_handling_missing_data.py`
- `README.md`

---

# Closing Thought

Strong analysts do not merely remove missing values.

They investigate what the missingness means.

---

Part of the Series:
**30 Days of Data Analytics – From Foundations to Decision Intelligence**
