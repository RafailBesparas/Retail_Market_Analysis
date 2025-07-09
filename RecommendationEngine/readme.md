
# 🛍️ Retail Product Recommendation System

This project is a **Neural Collaborative Filtering (NCF)** system built in **PyTorch** to recommend relevant products to retail customers based on their purchase history.

---

## 📌 **Use Case**

- Increase **cross-sell** and **upsell** by recommending products each customer is likely to buy next.
- Personalize the shopping experience for each customer segment.
- Enable marketing teams to launch **targeted promotions** with higher conversion.

---

## ⚙️ **Current Features**

- 📦 Input: Customer-product purchase interactions from transaction data.
- 🔗 Model: PyTorch-based NCF with user & product embeddings.
- 🎯 Output: Top-N product recommendations for each customer.
- ✅ Offline evaluation using **Precision@K** and **Recall@K** metrics.

---

## 🚧 **Known Issues**

- Low initial **Precision@5** and **Recall@5** (~0.4% and 0.1%) indicate room for improvement.
- No advanced **negative sampling strategy** yet.
- No filtering of previously purchased items during recommendation.
- No A/B test or production pipeline integrated yet.

---

## 🔜 **Next Steps**

- Implement more robust **negative sampling** and **hyperparameter tuning**.
- Add real-time inference API for deployment.
- Include filtering to avoid suggesting already purchased items.
- Extend offline evaluation with **MAP@K** and **Hit Rate**.
- Run A/B testing on live traffic to measure uplift in **conversion rate**.

---

## 📊 **Quantifiable Metric**

> ✅ **Current model achieves:**  
> **Precision@5 = 0.0040**  
> **Recall@5 = 0.0010**

This offline metric shows that the system can match real purchases in historical data — the goal is to raise this with better sampling and training.

---

## 🏷️ **Author**

Rafail Besparas
