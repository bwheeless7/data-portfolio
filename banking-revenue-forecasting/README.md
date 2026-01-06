# **Banking Revenue Forecasting & Growth Optimization**

## **Business Problem**

Accurate revenue forecasting is essential for strategic planning, resource allocation, and growth management in financial institutions.  
This project builds a data-driven system to **forecast future revenue**, evaluate growth trends, and translate findings into executive decision support.

---

## **Objective**

- Forecast monthly banking revenue with high accuracy  
- Quantify growth trends over time  
- Provide actionable insights for budgeting, staffing, and growth investments

---

## **Data Overview**

The dataset represents monthly banking performance with customer and revenue attributes, including:

- Customer counts and activity levels  
- Transaction behavior  
- Revenue components (fees, interest, total revenue)  
- Customer demographics and credit metrics

---

## Project Architecture


```
banking-revenue-forecasting/
├── data/
│ ├── banking_revenue_data.csv
│ └── revenue_forecast_by_segment.csv
│
├── notebooks/
│ ├── 01_data_generation_and_eda.ipynb
│ ├── 02_revenue_forecasting_and_growth_modeling.ipynb
│ ├── 03_customer_lifetime_value_and_growth_optimization.ipynb
│ └── 04_business_strategy.ipynb
│
└── README.md
```


---

## **Methodology**

1. Data generation and exploratory analysis  
2. Time series aggregation and preprocessing  
3. Revenue forecasting using Holt-Winters exponential smoothing  
4. Model evaluation using MAPE  
5. Customer Lifetime Value (CLV) modeling  
6. Customer segmentation by CLV tiers  
7. Growth opportunity identification and optimization  
8. Executive-level strategy development

---

## **Key Results**

### **Revenue Forecasting Performance**

| Metric | Value |
|------|------|
| Mean Absolute Percentage Error (MAPE) | **0.53%** |

The model produces highly reliable forecasts, enabling confident financial planning.

### **Growth Assessment**

- Revenue remained **stable with low volatility**  
- Year-over-year growth remained consistent  
- Customer engagement and monetization demonstrated strong stability within the dataset

### **Customer Value Segmentation**

Customers were segmented into four strategic tiers:

- **Low Value**  
- **Mid Value**  
- **High Value**  
- **VIP**

This segmentation provides the foundation for targeted growth and retention strategies.

---

## **Business Impact**

### **Key Insights**

- Forecasting accuracy supports precise budgeting and investment planning  
- Stable growth trends enable predictable scaling decisions  
- CLV segmentation identifies high-impact customer groups for revenue optimization

### **Actionable Recommendations**

1. Prioritize **VIP and High-CLV customers** for retention and premium services  
2. Design growth programs to convert **Mid-CLV customers into High-CLV**  
3. Maintain engagement programs to prevent Low-CLV customers from churn  
4. Use forecast projections to align hiring, capital investment, and marketing spend

---

## **Tools & Technologies**

- Python, Pandas, NumPy  
- Statsmodels (Holt-Winters forecasting)  
- Scikit-learn  
- Matplotlib  
- Jupyter Notebook

---

## **How to Reproduce**

```bash
git clone https://github.com/bwheeless7/data-portfolio.git
cd data-portfolio/banking-revenue-forecasting
pip install -r requirements.txt
```

Run notebooks in order:

1. `01_data_generation_and_eda.ipynb`  
2. `02_revenue_forecasting_and_growth_modeling.ipynb`  
3. `03_customer_lifetime_value_and_growth_optimization.ipynb`  
4. `04_business_strategy.ipynb`
