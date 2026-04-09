
# Telecom Customer Churn Prediction & Analysis

## Business Problem
A new competitor has entered the market with aggressive pricing plans. To protect market share, this project was commissioned to determine if existing customer data can predict churn and to identify the specific behavioral factors that drive customers to leave.

## Project Overview
This project developed a high-accuracy predictive model to identify customers at risk of leaving. By analyzing behavior patterns from **3,151 customers**, the goal was to provide actionable insights for a targeted retention strategy.

---

## Methodology
* **Data Split:** Implemented a rigorous 70/30 split (2,205 training rows / 946 test rows) to ensure the model generalizes to new data.
* **Feature Engineering:** Conducted a deep-dive correlation analysis. Removed redundant variables (Multicollinearity >75%), such as *Age Group* and *Seconds of Use*, to ensure model stability.
* **Model Selection:** Utilized a **Linear Probability Model (LPM)** to provide easily interpretable results for business stakeholders.
<img width="809" height="492" alt="Screenshot 221108" src="https://github.com/user-attachments/assets/7250cec6-59de-42ca-ac63-eb7cd1d34551" />


---

## Key Findings & Model Drivers
The model identified specific "trigger behaviors" that drastically increase the probability of churn:

1.  **Customer Complaints:** The strongest predictor. Filing a complaint increases the probability of churn by **56%**.
2.  **Account Status:** Inactive status correlates with a **24% increase** in churn risk.
3.  **Usage Habits:** Significant decreases in call frequency and charge amounts were identified as statistically significant early warning signs.

<img width="1012" height="545" alt="Screenshot 221129" src="https://github.com/user-attachments/assets/50711fc5-fce3-4951-bd51-99a4a57160e4" />


---

## Model Performance (Validation Results)
On the final 946-row Test Dataset, the model achieved the following benchmarks:

| Metric | Score | Definition |
| :--- | :--- | :--- |
| **Overall Accuracy** | **91.12%** | Total correct predictions vs. total customers. |
| **Recall (Sensitivity)**| **91.28%** | Success rate in identifying actual churners. |
| **Precision** | **89.19%** | Accuracy of the model when flagging a "High-Risk" customer. |


<img width="744" height="485" alt="Screenshot 221148" src="https://github.com/user-attachments/assets/99245d5a-08de-490c-8044-354e08cfb08b" />

---

## Strategic Recommendations
* **Immediate Intervention:** Implement a "Rapid Response" program for any customer who files a complaint. Since complaints are the #1 driver, immediate resolution is the most cost-effective churn reduction strategy.
* **Targeted Loyalty Offers:** Use the 0.5 probability threshold to identify the top 10% of at-risk customers for proactive retention incentives.
* **Monitoring Inactivity:** Automate "Status" change flags in the CRM to trigger immediate re-engagement campaigns.

---

## Technical Skills Demonstrated
* **Tools:** Microsoft Excel (Advanced Regression Toolpak, COUNTIFS, SUMPRODUCT).
* **Statistics:** Multicollinearity (VIF) analysis, P-Value validation, and Residual analysis.
* **Data Science:** Training/Testing validation, Confusion Matrix construction, and Threshold optimization.
