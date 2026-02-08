# Value-Based Churn Retention System

A value-based churn retention system that prioritizes customers by **net revenue impact instead of churn risk alone**, delivered through **decision-ready Power BI dashboards**.


## Business Problem
Customer churn reduces revenue, but retention budgets are limited.  
Treating all churners equally leads to wasted spend on low-value customers.



## Objective
Maximize **net retained revenue** by targeting only **high-risk, high-value customers** instead of attempting to retain everyone.


## Dataset Overview
- Total customers analyzed: **1,761**
- Observed churn rate: **27%**
- Customer behavior, service usage, and billing data
- Customer Lifetime Value (CLV) and retention cost were estimated using transparent, documented assumptions for prioritization logic

---

## Solution Overview
- Predicted customer churn probability using machine learning
- Estimated customer-level value (CLV) and retention cost
- Calculated **Expected Value** for each customer
- Ranked customers by **economic priority**
- Delivered decisions through interactive **Power BI dashboards**

---

## Core Logic
Customer-level prioritization is driven by **Expected Value**:

(Expected Customer Value × Churn Probability) − Retention Cost

This ensures retention spend is focused where it generates positive financial return.

---

## Key Results
- **14.99% of customers** were identified as economically viable retention targets
- Value-based targeting delivers an estimated **₹91.22K net revenue impact**
- A focused retention strategy avoids spending on low-value churn, improving overall efficiency

---

## Dashboards
The project includes three decision-focused Power BI dashboards:

1. **Executive Overview**  
   - Overall churn impact  
   - Retention coverage (14.99%)  
   - Net revenue impact (₹91.22K)

2. **Retention Priority List**  
   - Ranked list of customers by Expected Value  
   - Clear identification of who to retain and who to allow churn

3. **Churn Drivers & Risk Segmentation**  
   - Churn patterns by contract type and tenure  
   - Identification of high-risk, high-value customer segments

*(Screenshots included in the repository)*


## Explainability & Trade-offs
- Random Forest model used for churn prioritization accuracy
- Logistic Regression and segment-level analysis used for interpretability
- SHAP was intentionally excluded due to high computational cost relative to incremental business insight for this use case


## Business Recommendation
Retention incentives should be **allocated only to high-value churn-risk customers**, while allowing low-value churn where retention cost exceeds expected return.

This approach improves profitability without increasing retention spend.


## Tools
- Python (pandas, scikit-learn)
- Power BI
- VS Code

