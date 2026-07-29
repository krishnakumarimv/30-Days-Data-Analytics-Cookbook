# Day 17 – Correlation vs. Causation

## Why Relationships in Data Can Be Misleading

One of the most common mistakes in data analytics is assuming that **because two variables are related, one must be causing the other**.

In reality, correlation simply indicates that two variables move together in some way. It **does not** prove that one variable directly influences the other.

Understanding this distinction is one of the most important analytical skills. Misinterpreting correlation as causation can result in poor business decisions, ineffective policies, misleading reports, and unreliable predictive models.

In this chapter, we use the **NYC 311 Service Requests** dataset to explore statistical relationships while demonstrating why analysts must combine numerical evidence with domain knowledge before drawing conclusions.

---

# Dataset Context

**Dataset:** NYC 311 Service Requests (Kaggle)

**Domain:** Urban Governance / Citizen Complaints / Municipal Service Operations

The dataset includes:

- Complaint Creation Date
- Complaint Closed Date
- Resolution Time
- Complaint Type
- Borough
- Agency
- Complaint Status

These operational variables allow us to investigate relationships between service metrics while understanding the limitations of statistical association.

---

# Why Correlation Matters

Organizations frequently analyze relationships between variables to answer questions such as:

- Does higher complaint volume increase resolution time?
- Do certain complaint types take longer to resolve?
- Does seasonality influence service demand?
- Are workload and response time connected?

Correlation helps identify these patterns.

However, identifying a relationship is only the beginning of the analysis.

The next—and far more important—question is:

> **Does this relationship represent cause and effect?**

Without answering this question carefully, analysts risk making incorrect recommendations.

---

# Correlation Explained

Correlation measures the **strength and direction of the relationship** between two numerical variables.

The correlation coefficient ranges from **−1 to +1**.

| Correlation Coefficient | Interpretation |
|-------------------------|----------------|
| +1.0 | Perfect Positive Correlation |
| +0.7 to +0.9 | Strong Positive Relationship |
| +0.3 to +0.6 | Moderate Positive Relationship |
| 0 | No Linear Relationship |
| -0.3 to -0.6 | Moderate Negative Relationship |
| -0.7 to -0.9 | Strong Negative Relationship |
| -1.0 | Perfect Negative Correlation |

A positive correlation means both variables generally increase together.

A negative correlation means one variable increases while the other decreases.

A value near zero indicates little or no linear relationship.

---

# What is Causation?

Causation means that a change in one variable **directly produces** a change in another variable.

Unlike correlation, causation requires strong supporting evidence.

Analysts should consider:

- Business processes
- Domain expertise
- Experimental validation
- Time sequence
- External influencing factors

Statistical association alone is never enough to establish causality.

---

# Why Correlation Does Not Always Mean Causation

Several situations create misleading relationships.

## 1. Confounding Variables

Sometimes two variables appear related because both are influenced by a third factor.

Example:

- Heavy rainfall
- Increase in pothole complaints
- Increase in water leakage complaints

Rainfall is the underlying cause.

Potholes do not create water leaks.

---

## 2. Coincidental Relationships

Occasionally, two completely unrelated variables move together purely by chance.

These are known as **spurious correlations**.

Without domain knowledge, such relationships may appear meaningful even though they have no logical connection.

---

## 3. Reverse Causality

Sometimes analysts incorrectly assume the direction of influence.

For example:

Higher complaint volume may increase average resolution time.

It would be incorrect to conclude that longer resolution time causes additional complaints.

Understanding the sequence of events is essential.

---

# Objectives of This Chapter

This notebook demonstrates:

- Understanding correlation coefficients
- Calculating correlations using Pandas
- Creating correlation matrices
- Visualizing relationships using scatter plots
- Identifying misleading relationships
- Recognizing confounding variables
- Applying business interpretation before drawing conclusions

The emphasis is on **analytical reasoning rather than statistical calculation alone**.

---

# Notebook Contents

The accompanying Jupyter Notebook includes practical demonstrations of:

✔ Loading and preparing the NYC 311 dataset

✔ Creating numerical variables

✔ Computing correlation coefficients

✔ Building a correlation matrix

✔ Visualizing relationships using scatter plots

✔ Interpreting statistical relationships

✔ Understanding hidden variables

✔ Distinguishing association from causation

✔ Business interpretation of analytical results

---

# Business Interpretation

Suppose we observe a strong positive correlation between:

- Complaint Volume
- Average Resolution Time

Does this automatically prove that increasing complaints causes slower service?

Not necessarily.

Other contributing factors may include:

- Staffing shortages
- Weather conditions
- Infrastructure failures
- Holiday periods
- System outages
- Operational priorities

A responsible analyst investigates these possibilities before reaching conclusions.

---

# Practical Example

Imagine the following observation:

| Variable | Trend |
|----------|-------|
| Rainfall | Increased |
| Pothole Complaints | Increased |
| Water Leakage Complaints | Increased |

A simple correlation analysis would show that pothole complaints and water leakage complaints move together.

However, the true cause is rainfall.

Without understanding the operational context, an analyst could incorrectly conclude that potholes somehow create water leakage.

This illustrates why domain knowledge is as important as statistical analysis.

---

# Key Lessons

Good analysts do not stop after calculating correlation.

They ask:

- Why does this relationship exist?
- Is another factor influencing both variables?
- Does the timing support causation?
- Is there operational evidence?

Reliable analytics combines statistics with critical thinking.

---

# Practical Relevance

Understanding correlation is essential in:

- Business Intelligence
- Public Administration
- Healthcare Analytics
- Banking
- Retail
- Manufacturing
- Smart City Analytics
- Predictive Modeling
- Policy Evaluation

Correct interpretation improves the quality of evidence-based decision-making.

---

# Files Included

- **Jupyter Notebook** – Correlation analysis using NYC 311 Service Requests
- **README.md** – Conceptual explanation and business interpretation

---

# Closing Thought

Correlation helps us discover patterns.

Causation explains **why those patterns exist**.

Successful analysts do not confuse association with evidence.

They investigate relationships, validate assumptions, and combine statistical analysis with domain expertise before making decisions.

> **Correlation tells us that two variables move together. Causation tells us why they do. Understanding the difference is the hallmark of a skilled data analyst.**

---

## Part of the Series

**30 Days of Data Analytics – From Foundations to Decision Intelligence**

### Repository

**https://github.com/krishnakumarimv/30-Days-Data-Analytics-Cookbook**
