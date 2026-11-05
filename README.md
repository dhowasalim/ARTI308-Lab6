# Linear Regression with Python

ARTI308 – Machine Learning lab: predicting values with **Linear Regression** using `scikit-learn`.

## Contents

| File | Description |
|------|-------------|
| `Linear_Regression_with_Python.ipynb` | The full notebook: lab + task solution, executed with outputs |
| `USA_Housing.csv` | Lab dataset: house prices in US regions (5,000 rows) |
| `Ecommerce Customers` | Task dataset: e-commerce customers' yearly spending (500 rows) |
| `requirements.txt` | Python packages needed |

## 1. Lab – USA Housing price prediction

Predict house `Price` from area income, house age, number of rooms/bedrooms and population.

| Metric | Value |
|--------|-------|
| MAE  | ≈ 82,288 |
| RMSE | ≈ 102,279 |

## 2. Task – Ecommerce Customers

Predict a customer's **Yearly Amount Spent** and decide whether the company should focus on its **mobile app** or its **website**.

Steps: load data → explore (head / info / describe + EDA plots) → cleaning (missing, duplicate, negative values) → feature engineering (drop text identifier columns) → train/test split (70/30) → Linear Regression → evaluation.

| Metric | Value |
|--------|-------|
| MAE  | 7.23 |
| RMSE | 8.93 |
| R²   | 0.989 |

| Feature | Coefficient ($ per unit) |
|---------|-------------|
| Avg. Session Length | 25.98 |
| Time on App | 38.59 |
| Time on Website | 0.19 |
| Length of Membership | 61.28 |

**Conclusion:** Length of Membership is the strongest driver of spending, and time on the **app** matters far more than time on the website.

## Run it

```bash
pip install -r requirements.txt
jupyter notebook Linear_Regression_with_Python.ipynb
```
