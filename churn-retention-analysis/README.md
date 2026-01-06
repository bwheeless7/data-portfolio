# **Customer Churn & Retention Analysis**

## **Business Problem**

Customer attrition directly impacts revenue and long-term growth for digital banks.  
This project builds a machine learning system to **predict customer churn** and generate **actionable retention strategies**.

---

## **Objective**

- Predict customer churn with high accuracy  
- Identify the strongest behavioral drivers of attrition  
- Translate model insights into concrete business actions for retention

---

## **Data Overview**

The dataset represents customer demographics, transaction behavior, account activity, and product usage for a digital bank’s customer base.  
Key feature categories include:

- Transaction behavior  
- Engagement and activity metrics  
- Demographics and account characteristics  

---

## **Project Architecture**

```text
churn-retention-analysis/
├── data/
│   └── BankChurners.csv
|   ├── cleaned_churn_data.csv
├── notebooks/
│   ├── 01_problem_definition_and_eda.ipynb
│   └── 02_modeling_and_optimization.ipynb
└── README.md
```

---

## **Methodology**

1. Exploratory Data Analysis and Feature Understanding  
2. Data Cleaning and Preprocessing  
3. Baseline Model Development  
4. Advanced Model Training (XGBoost, Random Forest, Logistic Regression)  
5. Hyperparameter Optimization  
6. Decision Threshold Optimization  
7. Feature Importance & Business Interpretation  

---

## **Key Results**

### **Baseline Models — ROC-AUC**

| Model | ROC-AUC |
|------|--------|
| Logistic Regression | 0.9188 |
| Random Forest | 0.9848 |
| XGBoost | **0.9927** |

### **Optimized XGBoost Performance**

| Metric | Value |
|------|------|
| ROC-AUC | **0.9925** |
| Accuracy | 0.96 |
| Precision | 0.96 |
| Recall | 0.90 |
| F1-score | 0.93 |

### **Top Drivers of Churn**

| Feature | Importance |
|--------|-----------|
| Total_Trans_Ct | 0.20185 |
| Total_Revolving_Bal | 0.12374 |
| Total_Relationship_Count | 0.10342 |
| Total_Trans_Amt | 0.05556 |
| Total_Ct_Chng_Q4_Q1 | 0.04033 |
| Months_Inactive_12_mon | 0.03666 |

*(Additional features documented in notebook)*

---

## **Business Impact**

### **Key Insights**

- **Customer engagement and transaction behavior** are the strongest predictors of churn  
- **Inactive months and declining transaction activity** sharply increase attrition risk  
- **Income level and card type** enable targeted retention segmentation  

### **Actionable Recommendations**

1. Prioritize retention for customers with **high transaction count but declining engagement**  
2. Launch re-engagement campaigns for users with **multiple inactive months**  
3. Tailor incentives by **income bracket and card category** to maximize ROI  

---

## **Tools & Technologies**

- Python, Pandas, NumPy  
- Scikit-learn, XGBoost  
- Matplotlib, Seaborn  
- Jupyter Notebook  

---

## **How to Reproduce**

```bash
git clone https://github.com/bwheeless7/data-portfolio.git
cd data-portfolio/churn-retention-analysis
pip install -r requirements.txt
```

Run notebooks in order:

1. `01_problem_definition_and_eda.ipynb`  
2. `02_modeling_and_optimization.ipynb`
