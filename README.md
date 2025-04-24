# Car Price Prediction Using Linear & Lasso Regression

This machine learning project focuses on predicting car selling prices using a dataset with vehicle-related features. The goal is to build and evaluate regression models to estimate the selling price of a car. Two models — **Linear Regression** and **Lasso Regression** — were used and compared to understand their performance and feature-handling capabilities.

---

## Project Objective  
To implement and evaluate regression models capable of predicting car selling prices based on available dataset features and analyze the effectiveness of Lasso regularization.

---

## What Was Done  
- Loaded and explored the dataset to understand data types and target distribution.
- Split the dataset into training and testing sets with a **test size of 30%** to ensure unbiased evaluation.
- Trained and evaluated two regression models:
  - **Linear Regression**
  - **Lasso Regression**
- Compared both models using key regression metrics: `R² Score`, `MAE`, `MSE`, and `RMSE`.

---

## Regression Model Comparison

| Metric      | Lasso Regression     | Linear Regression    |
|-------------|----------------------|-----------------------|
| **R² Score** | 0.4426               | 0.4426                |
| **MAE**      | 219,446.93           | 219,447.06            |
| **MSE**      | 164,794,680,671.15   | 164,794,708,899.78    |
| **RMSE**     | 405,949.11           | 405,949.15            |

---

## Summary of Key Insights
- Both models **performed identically** across all evaluation metrics.
- **Lasso Regression** did not eliminate or regularize any features, behaving like **plain Linear Regression**.
- This suggests the dataset likely **lacks multicollinearity** or **irrelevant/noisy features** for Lasso to act on.
- An **R² of 0.4426** indicates that the model explains **only 44% of the variance** in car selling prices.

---

## Conclusion
- Lasso Regression provided **no additional benefit** over Linear Regression in this case.
- The limited performance suggests a need for:
  - Inclusion of more relevant features (e.g., **car condition**, **mileage**, **location**).
  - Consideration of **non-linear models** for improved accuracy.
  - Possible improvement in **data quality or granularity**.

---

**Developed by:** *Nischal Baidar*
