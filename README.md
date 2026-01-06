# Data Portfolio – End-to-End Analytics Projects

This repository showcases three end-to-end data science projects focused on banking and finance: churn prediction, revenue forecasting, and fraud detection.

---

## 1. Customer Churn & Retention Analysis
**Goal:** Predict which digital bank customers are likely to leave and derive actionable retention strategies.  
**Highlights:** XGBoost model with ROC-AUC 0.9925; feature importance informs targeted campaigns.  
**Key Features:** `Total_Trans_Ct`, `Total_Revolving_Bal`, `Total_Relationship_Count`, `Total_Trans_Amt`  

---

## 2. Banking Revenue Forecasting & Growth Optimization
**Goal:** Forecast monthly banking revenue, quantify growth trends, and guide strategic planning.  
**Highlights:** Holt-Winters Exponential Smoothing; MAPE 0.53%; assessed customer engagement stability.  

---

## 3. Fraud Risk Detection & Transaction Monitoring
**Goal:** Detect high-risk transactions to mitigate financial fraud.  
**Highlights:** Optimized XGBoost ROC-AUC 0.992; threshold tuning maximizes fraud recall with minimal false positives.  
**Key Features:** Transaction behavior metrics, customer risk scores  

---

## How to Explore

1. Clone repository:
```bash
git clone https://github.com/bwheeless7/data-portfolio.git
cd data-portfolio
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Open notebooks in `/notebooks` folders and run sequentially.

---

## Skills & Techniques

- **Languages & Tools:** Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, XGBoost, Statsmodels, Google Colab, Git/GitHub  
- **Data Prep & EDA:** Cleaning, aggregation, feature engineering, segmentation, visualization  
- **Modeling:** Classification (Logistic Regression, Random Forest, XGBoost), Time-series forecasting, Hyperparameter tuning, Cross-validation, Threshold optimization  
- **Business Impact:** Churn retention strategy, revenue growth planning, fraud risk mitigation, actionable insights for decision-making  

---

This portfolio demonstrates end-to-end execution: from data acquisition and preprocessing to modeling, evaluation, and business-focused recommendations.
