# Day 15 – Descriptive Statistics

## Understanding Data Before Building Models

Descriptive statistics form the foundation of every data analytics project.

Before building dashboards, creating visualizations, or developing machine learning models, analysts must first understand the characteristics of their data. Summary statistics provide a quick yet powerful overview of a dataset, helping identify patterns, variability, unusual observations, and potential data quality issues.

This chapter demonstrates descriptive statistical analysis using the **NYC 311 Service Requests** dataset—a real-world operational dataset representing citizen complaints and municipal service requests.

---

# Dataset Context

**Dataset:** NYC 311 Service Requests (Kaggle)

**Domain:** Urban Governance / Citizen Complaints / Service Operations

The dataset contains thousands of complaint records including:

- Complaint Type
- Borough
- Agency
- Created Date
- Closed Date
- Resolution Time
- Status

The combination of numerical and categorical variables makes this dataset ideal for learning descriptive statistics.

---

# Objectives of This Chapter

This notebook demonstrates:

- Understanding dataset dimensions
- Summary statistics using Pandas
- Mean, Median and Mode
- Standard Deviation
- Percentiles and Quartiles
- Frequency distributions
- Value counts
- Histograms
- Boxplots
- Business interpretation of statistical measures

The focus is on understanding the data before performing deeper analysis.

---

# Notebook Contents

The accompanying Jupyter Notebook covers:

✔ Loading and exploring the dataset

✔ Dataset structure (`shape`, `info`, `columns`)

✔ Numerical summary using `describe()`

✔ Mean, Median and Mode

✔ Frequency analysis using `value_counts()`

✔ Complaint distribution by Borough

✔ Resolution time statistics

✔ Histograms

✔ Boxplots

✔ Business interpretation

✔ Key analytical observations

---

# Key Concepts

## Measures of Central Tendency

These represent the typical value within a dataset.

- Mean
- Median
- Mode

Each measure provides a different perspective depending on the distribution of the data.

---

## Measures of Dispersion

Understanding variation is just as important as understanding averages.

This notebook introduces:

- Range
- Standard Deviation
- Quartiles
- Percentiles

These measures help assess the consistency and spread of observations.

---

## Frequency Analysis

Frequency distributions answer questions such as:

- Which complaint types occur most often?
- Which borough receives the highest number of complaints?
- Which agencies handle the largest workload?

Understanding frequency is essential for resource allocation and operational planning.

---

## Distribution Analysis

Visualizing distributions helps identify:

- Skewness
- Concentration
- Outliers
- Data spread

These insights guide future analytical and predictive tasks.

---

# Key Lessons

Descriptive statistics transform raw data into meaningful summaries.

They help analysts:

- Understand the dataset
- Detect inconsistencies
- Compare categories
- Identify unusual values
- Support evidence-based decision making

Before asking *"What should happen next?"*, analysts must first understand *"What is happening now?"*

---

# Practical Relevance

Descriptive statistics are used in:

- Business Intelligence
- Public Administration
- Healthcare
- Finance
- Manufacturing
- Retail
- Smart Cities
- Urban Governance

Every analytical project begins with descriptive analysis.

---

# Files Included

- **Jupyter Notebook** – Hands-on descriptive statistics using NYC 311
- **README.md** – Conceptual explanation and statistical guidance

---

# Closing Thought

Descriptive statistics do not solve problems.

They reveal the facts that enable better decisions.

Understanding your data is the first responsibility of every analyst.

---

## Part of the Series

**30 Days of Data Analytics – From Foundations to Decision Intelligence**

Repository:

https://github.com/krishnakumarimv/30-Days-Data-Analytics-Cookbook
