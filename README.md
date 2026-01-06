# Data Portfolio

This repository contains three end-to-end data science projects demonstrating skills in predictive modeling, forecasting, and risk detection for business applications.

---

## **Projects**

### 1. Customer Churn & Retention Analysis
**Objective:** Predict which customers are likely to leave a digital bank and identify actionable insights to improve retention.

**Key Highlights:**
- Baseline models (Logistic Regression, Random Forest, XGBoost) and hyperparameter optimization
- Decision threshold tuning to prioritize at-risk customers
- Feature importance analysis for actionable retention strategy

**Performance:**
- Optimized XGBoost ROC-AUC: 0.9925
- Accuracy: 0.96, Precision: 0.96, Recall: 0.90, F1-score: 0.93

**Top Features:** `Total_Trans_Ct`, `Total_Revolving_Bal`, `Total_Relationship_Count`, `Total_Trans_Amt`

**Notebooks:**
- [`01_problem_definition_and_eda.ipynb`](./churn-retention-analysis/notebooks/01_problem_definition_and_eda.ipynb)  
- [`02_modeling_and_optimization.ipynb`](./churn-retention-analysis/notebooks/02_modeling_and_optimization.ipynb)  

---

### 2. Banking Revenue Forecasting & Growth Optimization
**Objective:** Forecast future banking revenue, quantify growth trends, and provide executive-level planning insights.

**Key Highlights:**
- Time-series revenue forecasting using Holt-Winters Exponential Smoothing
- Growth analysis and segmentation to support strategic planning
- Assessment of customer engagement and monetization stability

**Performance:**
- Forecast Mean Absolute Percentage Error (MAPE): 0.53%

**Notebooks:**
- [`01_data_generation_and_eda.ipynb`](./banking-revenue-forecasting/notebooks/01_data_generation_and_eda.ipynb)  
- [`02_revenue_forecasting_and_growth_modeling.ipynb`](./banking-revenue-forecasting/notebooks/02_revenue_forecasting_and_growth_modeling.ipynb)  
- [`03_forecasting_models.ipynb`](./banking-revenue-forecasting/notebooks/03_forecasting_models.ipynb)  
- [`04_business_strategy.ipynb`](./banking-revenue-forecasting/notebooks/04_business_strategy.ipynb)  

---

### 3. Fraud Risk Detection & Transaction Monitoring
**Objective:** Detect high-risk fraudulent transactions and provide actionable insights for financial risk mitigation.

**Key Highlights:**
- Predictive modeling using Logistic Regression, Random Forest, and XGBoost
- Threshold optimization to maximize fraud recall while minimizing false positives
- Feature importance analysis for actionable fraud mitigation strategies

**Performance:**
- Optimized XGBoost ROC-AUC: 0.992
- Accuracy: 0.96, Precision: 0.97, Recall: 0.80, F1-score: 0.88

**Notebooks:**
- [`01_data_generation_and_eda.ipynb`](./fraud-risk-detection/notebooks/01_data_generation_and_eda.ipynb)  
- [`02_fraud_detection_models.ipynb`](./fraud-risk-detection/notebooks/02_fraud_detection_models.ipynb)  
- [`03_risk_scoring_and_threshold_optimization.ipynb`](./fraud-risk-detection/notebooks/03_risk_scoring_and_threshold_optimization.ipynb)  
- [`04_executive_strategy_and_impact.ipynb`](./fraud-risk-detection/notebooks/04_executive_strategy_and_impact.ipynb)  

---

## **How to Reproduce**

1. Clone the repository:
```bash
git clone https://github.com/bwheeless7/data-portfolio.git
cd data-portfolio
```

2. Install dependencies (example):
```bash
pip install -r requirements.txt
```

3. Run each project's notebooks in order as outlined above.

---

## **Skills & Techniques Summary**

**Programming & Tools:** Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, XGBoost, Statsmodels, Google Colab, Git/GitHub

**Data Processing & EDA:**  
- Data cleaning and preprocessing  
- Feature engineering  
- Aggregation and segmentation  
- Exploratory data analysis with visualizations

**Modeling & Evaluation:**  
- Predictive modeling: Logistic Regression, Random Forest, XGBoost  
- Time-series forecasting: Holt-Winters Exponential Smoothing  
- Hyperparameter tuning and cross-validation  
- Threshold optimization for classification tasks  
- Model performance metrics: ROC-AUC, Precision, Recall, F1-score, MAPE

**Business Application & Insights:**  
- Customer churn prediction and retention strategy  
- Revenue forecasting and growth planning  
- Fraud detection and risk mitigation  
- Translating data insights into actionable recommendations  

---

This portfolio demonstrates end-to-end project execution: data acquisition, analysis, modeling, evaluation, and business impact.
