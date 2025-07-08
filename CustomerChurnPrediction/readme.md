# 🛒 Retail Market Analysis — Repeat Purchase Prediction

This project predicts whether a **new customer** is likely to become a **repeat buyer** based only on their **first purchase** information.

---

## 📌 **Project Goals**

- Build a **realistic, deployable machine learning pipeline** to predict repeat purchasing with **no data leakage**.
- Use only features available at the **moment of first checkout**, such as basket size, spending, time, and country.
- Provide actionable insights for marketing and retention teams.

---

## ✅ **Key Features**

- **Leakage-free:** Target label created strictly from future purchases, not used in features.
- **Robust modeling:** Tested Logistic Regression, Decision Tree, XGBoost; finalized on **Random Forest** for best trade-off between performance, simplicity, and interpretability.
- **Handles imbalance:** Uses `class_weight='balanced'` instead of synthetic oversampling.
- **Full pipeline:** Data cleaning, feature engineering, train/test split, hyperparameter tuning (`GridSearchCV`), model evaluation, and feature importance analysis.

---

## 📊 **Performance**

| Metric | Value |
|--------|-------|
| **Test Accuracy** | ~59% |
| **Recall (Repeat Buyers)** | ~76% |
| **Precision (Repeat Buyers)** | ~66% |
| **Test Set Size** | 1,302 |
| **Key Metric Impact** | Supports lifting repeat purchase rate by ~5% → +8–12% projected Customer Lifetime Value |

---

## 🔑 **Features Used**

- **Quantity:** Total items in first basket.
- **Total Spending:** Total value of first purchase.
- **Avg Unit Price:** Average price per item in first order.
- **Country:** Encoded country of customer.
- **DayOfWeek:** Day the order was placed (0 = Monday).
- **Hour:** Hour the order was placed (0–23).

---

## 🚀 **Business Benefit**

This model can be deployed to **flag high-risk one-time buyers** and enable **targeted retention actions** (discounts, onboarding, loyalty perks).  
A realistic lift of **5% in repeat purchase rate** can increase **Customer Lifetime Value (CLV)** by up to **8–12%**.

---

## ⚙️ **Tech Stack**

- Python
- pandas, NumPy
- scikit-learn
- XGBoost (compared, not final)
- Seaborn, Matplotlib

---
