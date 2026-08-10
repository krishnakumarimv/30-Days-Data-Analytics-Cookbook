# Day 18 – Sampling Techniques

## Making Reliable Conclusions from Large Datasets

Sampling is the process of selecting a subset of data from a larger population to perform analysis efficiently.

A good sampling approach should provide a sample that represents the population relevant to the analytical question.

---

## Dataset

**NYC 311 Service Requests**

**Domain:** Urban Governance / Citizen Complaints / Service Operations

The dataset is used to demonstrate practical sampling techniques using Python and Pandas.

---

## What You'll Learn

- Population vs. Sample
- Simple Random Sampling
- Systematic Sampling
- Stratified Sampling
- Sampling Error
- Sampling Bias
- Sampling Variability
- Sample Size
- Choosing the right sampling method

---

## Sampling Techniques

### Simple Random Sampling

Every record has an equal opportunity to be selected.

```python
sample = df.sample(n=10000, random_state=42)
````

### Systematic Sampling

Records are selected at regular intervals.

```python
sample = df.iloc[::10]
```

### Stratified Sampling

The population is divided into groups and samples are selected from each group.

```python
sample = (
    df.groupby("Borough", group_keys=False)
      .apply(lambda x: x.sample(frac=0.10, random_state=42))
)
```

---

## Sampling Error vs. Sampling Bias

**Sampling Error** occurs because a sample represents only part of the population.

**Sampling Bias** occurs when the sampling method systematically overrepresents or underrepresents certain groups.

> A larger sample does not automatically eliminate sampling bias.

---

## Practical Example

In public grievance analytics, a city may have millions of complaints.

If management wants to estimate the percentage of complaints resolved within SLA, analyzing a carefully selected sample can provide a faster estimate.

If complaints differ significantly across zones, wards, departments, or complaint categories, **stratified sampling** may provide better representation.

---

## Key Takeaways

* A sample should represent the population.
* Different analytical problems require different sampling methods.
* Sampling error is expected.
* Sampling bias can distort conclusions.
* Always compare important characteristics of the sample with the population.
* Sample size and sampling method should be considered together.

---

## Files

* `Day_18_Sampling_Techniques.ipynb` – Practical Jupyter Notebook
* `README.md` – Chapter overview

---

## Part of the 30-Day Series

**Day 18 – Sampling Techniques**

Previous: **Day 17 – Correlation vs. Causation**

Next: **Day 19 – Hypothesis Testing**

### Repository

[30 Days of Data Analytics – From Foundations to Decision Intelligence](https://github.com/krishnakumarimv/30-Days-Data-Analytics-Cookbook)

