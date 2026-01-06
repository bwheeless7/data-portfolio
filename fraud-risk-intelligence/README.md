# **Fraud Risk Detection & Transaction Monitoring**

## **Business Problem**

Financial fraud is a major risk for banking institutions, leading to financial losses and reputational damage.  
This project builds a data-driven system to **detect fraudulent transactions** in real-time and provide actionable insights for risk management.

---

## **Objective**

- Identify high-risk transactions using predictive modeling  
- Optimize classification thresholds to balance fraud detection and false positives  
- Provide explainable insights for operational risk mitigation

---

## **Data Overview**

The dataset represents customer transaction behavior, including:

- Transaction amounts and types  
- Transaction fees and interest revenue  
- Customer demographics (age, income, credit score, tenure)  
- Monthly activity and engagement metrics

---

## Project Architecture
```
project3/
├── data/
│ ├── fraud_transactions.csv
│ └── fraud_risk_segmented.csv
├── notebooks/
│ ├── 01_data_generation_and_eda.ipynb
│ ├── 02_fraud_detection_models.ipynb
│ ├── 03_risk_scoring_and_threshold_optimization.ipynb
│ └── 04_executive_strategy_and_impact.ipynb
├── README.md
```


---

## **Methodology**

1. Data exploration and preprocessing  
2. Feature engineering for fraud detection  
3. Baseline model training and comparison (Logistic Regression, Random Forest, XGBoost)  
4. Hyperparameter tuning for best-performing models  
5. Threshold optimization based on business objectives (maximize fraud recall while minimizing false positives)  
6. Feature importance analysis and interpretability  
7. Executive-level insights and recommended mitigation strategies

---

## **Key Results**

### **Baseline Model Performance (ROC-AUC)**

| Model               | ROC-AUC |
|--------------------|---------|
| Logistic Regression | 0.92    |
| Random Forest       | 0.98    |
| XGBoost             | 0.99    |

### **Optimized Model (XGBoost)**

| Metric       | Value  |
|-------------|--------|
| ROC-AUC      | 0.992  |
| Accuracy     | 0.96   |
| Precision    | 0.97   |
| Recall       | 0.80   |
| F1-score     | 0.88   |

### **Top Features Influencing Fraud Detection**

| Feature               | Importance |
|----------------------|-----------|
| `transaction_amount`   | 0.21      |
| `fee_revenue`          | 0.15      |
| `credit_score`         | 0.13      |
| `tenure_months`        | 0.10      |
| `monthly_revenue`      | 0.09      |
| `age`                  | 0.08      |
| `income`               | 0.07      |

---

## **Business Impact**

### **Key Insights**

- High-value transactions and certain fee structures are most predictive of fraud  
- Longer-tenure or high-credit-score customers are not immune to fraud risk  
- Threshold tuning allows operational teams to focus on truly high-risk transactions  

### **Actionable Recommendations**

1. Flag transactions exceeding certain amounts or fee patterns for review  
2. Monitor customers with repeated high-risk signals to prevent losses  
3. Integrate the predictive model into real-time transaction monitoring systems  
4. Use feature importance insights to refine fraud prevention policies

---

## **Tools & Technologies**

- Python, Pandas, NumPy  
- Scikit-learn  
- XGBoost  
- Matplotlib, Seaborn  
- Jupyter Notebook

---

## **How to Reproduce**

```bash
git clone https://github.com/bwheeless7/data-portfolio.git
cd data-portfolio/fraud-risk-detection
pip install -r requirements.txt
```

Run notebooks in order:

1. `01_data_generation_and_eda.ipynb`  
2. `02_fraud_detection_models.ipynb`  
3. `03_risk_scoring_and_threshold_optimization.ipynb`  
4. `04_executive_strategy_and_impact.ipynb`
