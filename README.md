# 🏦 Banking Customer Financial Analytics & Intelligence System

> An end-to-end financial analytics project analyzing 42,770 banking customer records to identify subscription patterns, segment financial risk, and predict term deposit conversions using Python, SQL, Power BI, and Machine Learning.

---

## 📌 Business Problem

A Portuguese bank ran telephone marketing campaigns to sell term deposits but achieved only an **11.51% conversion rate** — meaning **88.49% of campaign resources were wasted**.

**Key Questions This Project Answers:**
- Which customer segments are most likely to subscribe?
- Which months deliver the highest conversion rates?
- Can we predict future subscribers before making the call?
- What financial risk factors influence subscription decisions?

---

## 🎯 Project Objectives

- Perform exploratory data analysis to identify patterns in customer behavior
- Build SQL queries to extract actionable business insights
- Develop an interactive Power BI dashboard for stakeholder reporting
- Train a Machine Learning model to predict customer subscription probability
- Deliver consulting-style business recommendations

---

## 🛠️ Tools & Technologies

| Category | Tools |
|---|---|
| **Data Analysis** | Python (Pandas, NumPy, Matplotlib, Seaborn) |
| **Database & SQL** | SQLite, SQL queries |
| **Business Intelligence** | Power BI Desktop |
| **Machine Learning** | Scikit-learn (Logistic Regression) |
| **Development Environment** | Jupyter Notebook |

---

## 📁 Project Structure

```
banking-financial-analytics/
│
├── notebooks/
│   ├── 01_data_cleaning.ipynb       # Data cleaning, EDA, SQL queries
│   └── 02_ml_model.ipynb            # ML model training and prediction
│
├── data/
│   └── bank_cleaned.csv             # Cleaned dataset (42,770 records)
│
├── dashboard/
│   └── Bank_Marketing_Dashboard.pbix  # Power BI 4-page dashboard
│
└── README.md
```

---

## 📊 Dataset

- **Source:** UCI Bank Marketing Dataset
- **Records:** 45,211 raw → 42,770 after cleaning
- **Features:** 17 columns including age, job, balance, loan status, contact month
- **Target:** Term deposit subscription (Yes/No)

---

## 🔍 Key Findings

### 📈 Conversion Insights
- Overall conversion rate: **11.51%**
- **March** delivers the highest conversion at **52.09%** — 4.5x the average
- **May** is the worst month at only **6.57%** conversion

### 👥 Customer Segmentation
- **Students** show the highest conversion at **28.93%**
- **Retired customers** follow at **22.21%**
- **Blue-collar workers** show the lowest at **7.22%**

### 💰 Financial Risk Analysis
- Customers with **no loan and no housing** convert at **18.07%** — 3x higher than those with both
- **Self-employed** subscribers hold the highest average balance of **₹3,079**
- **Tertiary-educated** customers hold **25% higher** average balances

### 📞 Campaign Effectiveness
- **Call duration** is the strongest predictor of subscription
- **Cellular contact** reaches the most customers
- Customers with **no financial obligations** are 3x more likely to subscribe

---

## 🤖 Machine Learning Model

| Metric | Value |
|---|---|
| **Algorithm** | Logistic Regression |
| **Training Set** | 34,216 records (80%) |
| **Test Set** | 8,554 records (20%) |
| **Accuracy** | **88.95%** |
| **True Negatives** | 7,435 |
| **True Positives** | 174 |

### Sample Prediction:
```python
# New customer prediction
new_customer = {
    'age': 35, 'balance': 2000, 'duration': 300,
    'campaign': 2, 'pdays': -1, 'previous': 0
}
# Output: WILL NOT SUBSCRIBE (10.37% probability)
```

---

## 📋 Power BI Dashboard

4-page interactive dashboard covering:
- **Page 1:** Executive Summary — KPIs, total customers, conversion rate
- **Page 2:** Customer Analysis — age, education, marital status
- **Page 3:** Campaign Performance — monthly trends, contact type
- **Page 4:** Risk Analysis — loan status, housing impact

---

## 💡 Business Recommendations

1. **Concentrate 70% of campaign budget in March, September, and December** — these 3 months deliver 45%+ conversion rates vs 6-10% in May-July

2. **Prioritize student and retired customer segments** — they convert at 28.9% and 22.2% respectively vs 7.2% for blue-collar workers

3. **Target debt-free customers first** — customers with no loan and no housing convert at 18% — nearly 3x the overall average

---

## 🚀 How to Run

**Clone the repository:**
```bash
git clone https://github.com/shashank-joshi/banking-financial-analytics.git
```

**Install dependencies:**
```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

**Run notebooks:**
```bash
jupyter notebook
```
Open `01_data_cleaning.ipynb` → Run all cells
Open `02_ml_model.ipynb` → Run all cells

---

## 👤 Author

**Shashank Joshi**
MBA Finance | Business Analytics Minor
Tirpude Institute of Management Education, Nagpur

📧 joshishashank15@gmail.com
🔗 [LinkedIn](https://www.linkedin.com/in/shashank-joshi-450393220)

---

## 📌 Note

This project was built as part of my portfolio to demonstrate end-to-end financial analytics capabilities spanning data engineering, business intelligence, and predictive modeling — targeting roles in Financial Analysis, Business Analysis, and Data Analysis.
