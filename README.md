# Device Insurance Attach Percentage Analysis & Forecasting

## 📌 Overview
This project presents an end-to-end data analysis of **device insurance attach percentage** across retail stores of *Jumbo & Company*. The objective is to understand attach performance drivers, identify improvement opportunities, segment stores based on behavior, and forecast **January attach percentage** at the store level.

The analysis is designed to be **business-focused, interpretable, and actionable**, aligning with real-world decision-making requirements.

---

## 🎯 Business Problem
Attach percentage represents the proportion of customers who purchase an insurance plan along with a device. For insurance partners like **Zopper**, higher attach percentage directly translates to increased revenue without increasing device sales volume.

The key questions addressed are:
- How does attach percentage behave across months, stores, and branches?
- Which stores consistently perform well or poorly?
- What actionable insights can improve attach performance?
- Can January attach percentage be reasonably forecasted using historical data?

---

## 📂 Dataset Description
- **Granularity:** Store-level, monthly data  
- **Time Period:** August to December  
- **Rows:** 163 stores  
- **Key Columns:**
  - Branch
  - Store Name
  - Monthly Attach % (Aug–Dec)

Zero values are treated as valid business outcomes (months with no insurance sold).

---

## 🧠 Methodology

### 1. Exploratory Data Analysis (EDA)
- Data quality checks (missing values, validity)
- Month-wise descriptive statistics
- Identification of variability across stores

### 2. Feature Engineering
- **Average Attach % (`avg_attach`)** – overall store performance
- **Standard Deviation** – performance consistency across months

### 3. Performance Analysis
- Month-wise trend analysis
- Store-level performance comparison
- Identification of top and bottom performers

### 4. Store Segmentation
Stores are categorized using:
- **Performance:** Low / Mid / High (quartile-based)
- **Consistency:** Consistent / Inconsistent (based on month-to-month variability)

This results in business-friendly segments such as:
- *High + Consistent*
- *Mid + Inconsistent*
- *Low + Inconsistent*

---

## 📊 Trend & Pattern Analysis
- Chronologically ordered month-wise analysis confirms a steady increase in attach percentage from August to December
- Mean and median trends move together, indicating broad-based improvement
- High variability persists across stores, highlighting execution differences

---

## 📈 January Attach % Forecast

### Forecasting Approach
- **Primary Model:** Store-level linear trend extrapolation using Aug–Dec data
- **Target:** Predict January attach percentage per store
- **Output Column:** `Jan_Predicted_Attach`

The approach prioritizes **interpretability and robustness** over complex models due to limited historical data.

### Key Observations
- High-performing stores show continued momentum
- Low-performing stores exhibit flat or near-zero projections
- Negative extrapolations indicate structural underperformance rather than model error

---

## 💡 Key Insights
- Attach percentage improves consistently month-on-month
- Store-level performance differences dominate overall trends
- A small subset of stores contributes disproportionately to high attach %
- Several stores show structurally low or zero attach

---

## 🧾 Business Recommendations
- Replicate best practices from *High + Consistent* stores
- Prioritize *Low + Inconsistent* stores for focused training
- Introduce branch-level performance accountability
- Extend festive-season selling strategies across the year
- Set realistic benchmarks using median-performing stores

---

## 📊 Visualizations Included
- Month-wise attach trend (mean, median, and variability)
- Store-level attach distribution
- Store segmentation (performance vs consistency)
- Sample store-level January prediction illustration

---

## ⚠️ Assumptions & Limitations

### Assumptions
- No major changes in store operations or incentives in January
- Historical attach patterns broadly continue

### Limitations
- Only five months of historical data
- No customer-level or device-level information
- External factors (promotions, staffing) not explicitly modeled

---

## 🛠️ Tech Stack
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Scikit-learn  

---
```
## 📁 Repository Structure
├── notebook/
│ └── attach_analysis.ipynb
├── report/
│ └── Attach_Percentage_Analysis_Report.pdf
├── images/
│ └── charts/
├── data/
└── README.md
```


---

## 🚀 Conclusion
This project demonstrates a complete data science workflow—from business understanding and exploratory analysis to segmentation, recommendations, and forecasting—focused on clarity, interpretability, and real-world applicability.

---

## 📬 Author
**[Yoganshu Sharma]**  

