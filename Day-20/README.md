# Day 20 – Confidence Intervals

## Measuring Uncertainty Around Your Data

A point estimate gives us a single number. A **confidence interval** helps us understand the uncertainty surrounding that estimate.

In this notebook, we use a practical **public grievance resolution-time** example to understand how confidence intervals support better analytical decisions.

### Key Concepts

* Point estimate vs. interval estimate
* Standard error
* Margin of error
* 90%, 95% and 99% confidence levels
* Confidence interval for a mean
* Confidence interval for a proportion
* Effect of sample size on precision
* Confidence interval for differences
* Statistical vs. practical significance
* Precision vs. accuracy

### Practical Example

Suppose a department reports:

**Average grievance resolution time = 48 hours**

Instead of reporting only the average, we can report:

**48 hours (95% CI: 46.5–49.5 hours)**

This provides decision-makers with information about the uncertainty around the estimate.

### Notebook Workflow

```text
Sample Data
     ↓
Point Estimate
     ↓
Standard Error
     ↓
Margin of Error
     ↓
Confidence Interval
     ↓
Interpretation
     ↓
Decision
```

### Python Libraries

```python
numpy
pandas
matplotlib
scipy
```

Install dependencies if required:

```bash
pip install numpy pandas matplotlib scipy
```

### Public Governance Applications

Confidence intervals can be used for:

* Grievance resolution time
* SLA compliance
* Citizen satisfaction
* Property-tax collection
* Waste collection efficiency
* Service response time
* Infrastructure repair time
* Citizen-service adoption

### Important Insight

**Statistical precision is not the same as accuracy.**

A narrow confidence interval does not automatically mean that the estimate is unbiased. Sampling quality and data quality remain critical.

Similarly:

**Statistical significance ≠ Practical significance**

A statistically significant change may not necessarily be important from an operational perspective.

### Key Takeaway

> **Averages tell us where the data is. Confidence intervals tell us how precisely we have estimated it.**

The analytical progression is:

**Observation → Estimation → Uncertainty → Evidence → Decision**

---

## Files

* `Day_20_Confidence_Intervals_Analytics_Cookbook.ipynb`
* `README.md`

## 30 Days of Data Analytics

**Day 20 – Confidence Intervals**

Previous: **Day 19 – Hypothesis Testing**
Next: **Day 21 – Correlation & Regression**
