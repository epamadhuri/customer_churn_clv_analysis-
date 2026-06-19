# customer_churn_clv_analysis-
Built an end‑to‑end data science project integrating churn prediction and Customer Lifetime Value (CLV) estimation using Random Forest and XGBoost.
# Customer Churn Prediction & CLV Estimation

## 📌 Project Overview
This project analyzes customer data to:
- Predict **churn probability** (likelihood of a customer leaving).
- Estimate **Customer Lifetime Value (CLV)** using regression.
- Combine churn + CLV to identify **high-value customers at risk of churn**.
- Provide actionable business insights for retention and growth.

---

## 📂 Dataset Details
The project uses six files provided in the case study:
1. **Customer Demographics** – age, gender, location.
2. **Subscription Details** – type, contract length, tenure.
3. **Usage Data** – frequency of interactions, last activity.
4. **Support Calls** – number of support interactions.
5. **Spend Data** – total spend, transaction history.
6. **Churn Labels** – whether the customer churned (1) or stayed (0).

---

## ⚙️ Workflow
1. **Data Preparation**
   - Load and merge six datasets.
   - Handle missing values, encode categorical features.
   - Feature engineering: ratios (usage per month, support per month).

2. **Churn Prediction**
   - Random Forest Classifier.
   - Confusion matrix + accuracy evaluation.
   - Feature importance visualization.

3. **CLV Estimation**
   - Target transformation (`log(total_spend)`).
   - XGBoost Regressor for regression.
   - Feature importance visualization.

4. **Segmentation**
   - Combine churn probability + predicted CLV.
   - Create 4 customer segments:
     - High Value – High Risk
     - High Value – Low Risk
     - Low Value – High Risk
     - Low Value – Low Risk

5. **Visualization**
   - Confusion matrix heatmap.
   - Feature importance bar charts.
   - Scatter plot of churn vs CLV.
   - Segmentation scatter plot.

6. **Business Insights**
   - Retention focus on **High Value – High Risk** customers.
   - Upselling opportunities for **High Value – Low Risk** customers.
   - Monitoring churn drivers in **Low Value – High Risk** group.
   - Maintain cost-effective engagement for **Low Value – Low Risk**.

---

## 📊 Results
- **Churn Model Accuracy:** ~XX% (replace with your result).
- **CLV Model R²:** ~YY (replace with your result).
- **Key Drivers of Churn:** [list top features].
- **Key Drivers of CLV:** [list top features].

---

## 💡 Business Recommendations
- Prioritize retention campaigns for **high-value customers at risk of churn**.
- Focus upselling/cross-selling on loyal high-value customers.
- Use churn drivers to improve service for at-risk groups.
- Maintain efficient engagement for stable low-value customers.

---

## 🚀 How to Run
1. Open the notebook in **Google Colab**.
2. Upload the six dataset files.
3. Run cells step by step:
   - Data preparation
   - Churn prediction
   - CLV estimation
   - Segmentation & insights
4. Review visualizations and final recommendations.

---

## 📌 Conclusion
This project demonstrates how combining churn prediction with CLV estimation provides actionable insights. Businesses can identify which customers are both valuable and at risk, enabling smarter retention strategies and maximizing long-term revenue.
