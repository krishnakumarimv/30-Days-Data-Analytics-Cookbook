# Day 19 – Hypothesis Testing

## Turning Data Observations into Statistical Evidence

A difference in data does not automatically mean that something has changed.

**Hypothesis testing** helps us determine whether an observed difference provides sufficient statistical evidence to support a conclusion.

This notebook uses a practical **public grievance resolution-time** example.

### What You'll Learn

* Null and alternative hypotheses
* Significance level and p-value
* Independent two-sample t-test
* Welch's t-test
* Confidence intervals
* Cohen's d effect size
* Statistical vs. practical significance
* Why statistical significance does not prove causation

### Practical Example

Suppose:

* Before workflow change → **52 hours** average resolution time
* After workflow change → **47 hours**

The question is:

> **Is the observed reduction statistically significant, or could it be due to normal variation?**

### Hypothesis

**H₀:** There is no difference in mean resolution time.

**H₁:** There is a difference in mean resolution time.

Using:

`α = 0.05`

The notebook demonstrates how to:

1. Create sample data
2. Compare descriptive statistics
3. Visualize the distributions
4. Perform Welch's t-test
5. Interpret the p-value
6. Calculate a 95% confidence interval
7. Calculate Cohen's d
8. Translate statistical results into an operational interpretation

### Important Concepts

**p-value**
Helps evaluate how compatible the observed result is with the null hypothesis.

**Confidence interval**
Provides a range of plausible values for the estimated difference.

**Effect size**
Shows the magnitude of the difference, rather than only whether it is statistically significant.

**Practical significance**
Determines whether the observed effect is meaningful in the real-world context.

### Public Grievance Applications

Hypothesis testing can be used to investigate questions such as:

* Did complaint resolution time change after a process intervention?
* Are resolution times different between departments?
* Are service levels different across zones?
* Is escalation associated with complaint category?
* Did complaint volume change after a policy intervention?

### Key Takeaway

> **Statistical significance is not the same as practical significance—and statistical significance does not automatically establish causation.**

The objective is not simply to calculate a p-value.

The objective is to move from:

**Data → Evidence → Better Decisions**

### Requirements

```text
Python 3.x
pandas
numpy
matplotlib
scipy
jupyter
```

Install dependencies:

```bash
pip install pandas numpy matplotlib scipy jupyter
```

### Files

```text
Day_19_Hypothesis_Testing_Analytics_Cookbook.ipynb
README.md
```

### GitHub Repository

**30 Days of Data Analytics – Analytics Cookbook**

[https://github.com/krishnakumarimv/30-Days-Data-Analytics-Cookbook](https://github.com/krishnakumarimv/30-Days-Data-Analytics-Cookbook)

### Series

**Day 19 – Hypothesis Testing**

Previous: **Day 18 – Sampling Techniques**

Next: **Day 20 – Confidence Intervals**
