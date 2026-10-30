# Day 27 — Model Evaluation & Performance Metrics

**30-Day Data Analytics Cookbook | From Foundations to Real-World Impact**

> A model that predicts is useful. A model that predicts reliably is valuable.

## What you will learn
- Evaluate regression and forecasting models using **MAE, MSE, RMSE, MAPE, WAPE and R²**.
- Identify systematic overprediction or underprediction using **forecast bias**.
- Compare candidate models on the same test observations.
- Visualize forecasts and residuals.
- Use chronological holdout and rolling-origin backtesting.
- Benchmark models against a simple **naive forecast**.

## Practical use case
Evaluate two hypothetical models predicting monthly citizen-grievance volumes in an urban local body. All example data is **synthetic**, not official Greater Chennai Corporation data.

## Files
- [`Day_27_Model_Evaluation_Performance_Metrics.ipynb`](Day_27_Model_Evaluation_Performance_Metrics.ipynb) — executable tutorial, visualizations, baseline, and exercises.

## Requirements
Python 3.10+ and Jupyter Notebook or JupyterLab.

```bash
pip install numpy pandas matplotlib scikit-learn jupyter
jupyter notebook Day_27_Model_Evaluation_Performance_Metrics.ipynb
```

## Key concepts

| Metric | Interpretation | Watch out for |
|---|---|---|
| MAE | Average absolute error | Treats large and small errors linearly |
| MSE | Average squared error | Units are squared |
| RMSE | Error with extra penalty for large misses | Sensitive to outliers |
| MAPE | Average percentage error | Undefined if actual values include zero |
| WAPE | Total absolute error relative to total actual magnitude | Undefined when total actual magnitude is zero |
| R² | Improvement over a constant-mean reference | Can be negative |
| Bias | Average predicted minus actual | Positive = overprediction |

**Evaluation rule:** Never randomly shuffle a forecasting series into training and test data. Use chronological holdout or rolling-origin evaluation, and prevent future-data leakage.

## Exercises
1. Add a constant forecast and compare results.
2. Simulate a large error and inspect RMSE.
3. Explore MAPE with zero actual values.
4. Evaluate only the last six rolling forecasts.

## Real-world relevance
Forecast evaluation can support municipal complaint staffing, solid-waste logistics, property-tax planning and seasonal preparedness. Accuracy must be considered alongside operational consequences.

## Series
- **Day 26:** Time Series Analysis & Forecasting
- **Day 27:** Model Evaluation & Performance Metrics
- **Day 28:** Data Storytelling & Communicating Insights

**Data analytics is not about dashboards. It is about decisions.**
