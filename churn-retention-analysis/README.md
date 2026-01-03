# Customer Churn & Retention Analysis

This repository contains a data science project analyzing customer churn for a digital bank. The goal is to predict which customers are likely to leave and identify actionable insights to improve retention.

---

## Project Structure

- `01_problem_definition_and_eda.ipynb`  
  Covers problem definition, exploratory data analysis (EDA), data cleaning, and preprocessing.

- `02_modeling_and_optimization.ipynb`  
  Covers baseline modeling, hyperparameter optimization, decision threshold tuning, feature importance extraction, and actionable insights.

- `data/`  
  Contains the original dataset and any processed versions used for modeling.

---

## Key Results

**Baseline Models ROC-AUC:**

| Model               | ROC-AUC |
|--------------------|---------|
| Logistic Regression | 0.9188  |
| Random Forest       | 0.9848  |
| XGBoost             | 0.9927  |

**Optimized XGBoost Model Performance:**

| Metric       | Value  |
|-------------|--------|
| ROC-AUC      | 0.9925 |
| Accuracy     | 0.96   |
| Precision    | 0.96   |
| Recall       | 0.90   |
| F1-score     | 0.93   |

**Top Features (by importance in optimized XGBoost model):**

| Feature                         | Importance |
|---------------------------------|-----------|
| `Total_Trans_Ct`                 | 0.20185   |
| `Total_Revolving_Bal`            | 0.12374   |
| `Total_Relationship_Count`       | 0.10342   |
| `Total_Trans_Amt`                | 0.05556   |
| `Total_Ct_Chng_Q4_Q1`            | 0.04033   |
| `Months_Inactive_12_mon`         | 0.03666   |
| `Gender_F`                        | 0.02990   |
| `Total_Amt_Chng_Q4_Q1`           | 0.02815   |
| `Customer_Age`                    | 0.02580   |
| `Contacts_Count_12_mon`           | 0.02526   |
| `Avg_Open_To_Buy`                 | 0.01956   |
| `Income_Category_$60K - $80K`    | 0.01835   |
| `Credit_Limit`                    | 0.01773   |
| `Marital_Status_Married`          | 0.01706   |
| `Card_Category_Silver`            | 0.01702   |

---

## Business Insights

- **High transaction count and revolving balance** are key predictors of churn.  
- **Inactive months and low engagement** correlate strongly with attrition risk.  
- **Income and card category** segments can be used to prioritize retention campaigns.  

**Actionable Recommendations:**

1. Target customers with high `Total_Trans_Ct` and low engagement for retention campaigns.  
2. Offer incentives to users with inactive months or low `Total_Amt_Chng_Q4_Q1`.  
3. Tailor offers by income bracket and card category to maximize retention ROI.

---

## How to Reproduce

1. Clone the repository:  
   ```bash
   git clone https://github.com/bwheeless7/data-portfolio.git
   cd data-portfolio
2. Install dependencies (example using pip):
   ```bash
    pip install -r requirements.txt
3. Run the notebooks in order:
  1. 01_problem_definition_and_eda.ipynb
  2. 02_modeling_and_optimization.ipynb
