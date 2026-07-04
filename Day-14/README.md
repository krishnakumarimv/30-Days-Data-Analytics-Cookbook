# Day 14 – Aggregation vs Granularity

## Why the Level of Detail Determines the Quality of Your Insights

Data analytics is not just about collecting data or building visualizations. It is equally about deciding **how much detail should be retained during analysis**.

One of the most common mistakes made by beginners is summarizing data too early. Aggregation makes large datasets easier to understand, but it can also hide trends, anomalies, seasonal patterns, and operational issues that exist in detailed data.

The same dataset can tell completely different stories depending on whether it is viewed at the city level, borough level, complaint category level, or individual complaint level.

This chapter demonstrates how aggregation changes analytical conclusions using the **NYC 311 Service Requests** dataset.

---

# Dataset Context

**Dataset:** NYC 311 Service Requests (Kaggle)

**Domain:** Urban Governance / Citizen Complaints / Service Operations

The dataset contains highly detailed records including:

- Complaint Type
- Borough
- Agency
- Created Date
- Closed Date
- Resolution Status
- Geographic Location

Because every complaint is stored individually, analysts can aggregate the data in multiple ways depending on the business question.

---

# Objectives of This Chapter

This notebook demonstrates:

- Understanding granularity
- Aggregation using Pandas
- Multi-level GroupBy
- Time-based aggregation
- Pivot tables
- Comparing different aggregation levels
- Understanding information loss
- Choosing the correct analytical level

The emphasis is analytical reasoning rather than programming complexity.

---

# Notebook Contents

The accompanying Jupyter Notebook demonstrates:

✔ Grouping data using `groupby()`

✔ Aggregating complaints by Borough

✔ Aggregating complaints by Complaint Type

✔ Monthly complaint trends

✔ Daily complaint trends

✔ Multiple-level grouping

✔ Pivot tables

✔ Comparing City, Borough and Daily summaries

✔ Visual comparison of different aggregation levels

✔ Business interpretation of summaries

---

# Understanding Granularity

Granularity refers to the level of detail at which data is stored, analyzed or presented.

Higher granularity preserves more operational information.

Lower granularity simplifies reporting but may hide important patterns.

Examples:

| Granularity | Example |
|-------------|---------|
| City | Total complaints |
| Borough | Borough workload |
| Complaint Type | Service demand |
| Daily | Operational events |
| Individual Record | Root-cause analysis |

---

# Why Aggregation Matters

Aggregation converts detailed observations into summarized information.

Examples include:

- Total complaints
- Average resolution time
- Monthly complaint counts
- Complaint percentages

Summaries simplify analysis but also remove detail.

An analyst should always ask:

> **What information disappears after summarization?**

---

# Key Lessons

## Aggregation simplifies analysis

Large datasets become easier to interpret.

---

## Too much aggregation hides reality

Important operational events disappear.

---

## Different questions require different granularity

Executive dashboards require summaries.

Operational investigations require detailed records.

---

## Strong analysts move between both levels

They begin with summaries.

They investigate using detailed records.

---

# Practical Relevance

Aggregation is essential in:

- Business Intelligence
- Urban Governance
- Smart Cities
- Finance
- Healthcare
- Retail
- Manufacturing

Every dashboard, KPI and report depends upon choosing the correct aggregation level.

---

# Files Included

- **Jupyter Notebook** – Aggregation and Granularity Analysis
- **README.md** – Conceptual explanation

---

# Closing Thought

Aggregation shows the bigger picture.

Granularity explains **why** the picture looks that way.

Great analysts know when to zoom out—and when to zoom in.

---

## Part of the Series

**30 Days of Data Analytics – From Foundations to Decision Intelligence**

Repository:

https://github.com/krishnakumarimv/30-Days-Data-Analytics-Cookbook
