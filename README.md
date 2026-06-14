# Telecom Customer Churn Prediction

## Project Overview
This project analyzes a dataset of 7,000+ subscriber records to identify the primary drivers of customer attrition and build predictive models that flag high-risk accounts for proactive retention campaigns.

## Key Results
* **79% Recall:** Optimized predictive models to minimize false negatives, ensuring the business captures the highest percentage of actual churners.
* **Balanced Handling:** Countered a severe native class imbalance (73% active vs. 27% churned) by operationalizing cost-sensitive learning techniques.
* **Actionable Insights:** Isolated critical contract and service-related friction points that directly trigger customer attrition.

## Tech Stack
* **Language:** Python
* **Data Wrangling:** Pandas, NumPy
* **Visualization:** Matplotlib
* **Machine Learning:** Scikit-Learn (Logistic Regression, Random Forest)

## Pipeline Summary

1. **Data Cleaning:** Processed raw inputs and converted missing/coerced string data in `TotalCharges` to real numeric values.
2. **EDA Insights:** * **Contract Architecture:** Month-to-month contracts showed a **42.7%** churn rate compared to just **2.8%** for two-year accounts.
   * **Service Friction:** `Fiber Optic` users churned at **41.9%**, more than double that of `DSL` users (**19.0%**).
3. **Preprocessing:** Applied binary mapping, one-hot encoding, and statistical feature scaling (`StandardScaler`).
4. **Model Performance (Test Matrix):**

| Model | Precision (Churn) | Recall (Churn) | F1-Score | Accuracy |
| :--- | :---: | :---: | :---: | :---: |
| **Logistic Regression (Balanced)** | `0.50` | **`0.79`** | `0.61` | `0.74` |
| **Random Forest (Balanced)** | `0.53` | `0.71` | `0.61` | `0.76` |

## 📈 Strategic Takeaways
* **Target Month-to-Month Users:** Implement automated, early-lifecycle promotions to incentivize transitions to long-term commitments.
* **Audit Fiber Optic Setup:** Investigate the high attrition rate among fiber-optic users to uncover potential product, pricing, or installation instability.
