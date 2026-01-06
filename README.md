# 📉 Telco Customer Churn Analysis (Python)

## 📌 Project Overview
This project analyzes customer churn behavior in a telecommunications company to understand **why customers leave** and **which customer segments are most at risk**.  
The analysis focuses on **exploratory data analysis (EDA)** to generate **business-relevant insights** that can support customer retention strategies.

---

## 🗂 Data Source
- **Dataset:** IBM Telco Customer Churn Dataset
- **Source:** Kaggle / IBM Analytics
- **Records:** ~7,000 customers
- **Format:** CSV

---

## ❓ Business Questions
This analysis aims to answer:
1. What is the overall customer churn rate?
2. Which contract types are associated with higher churn?
3. How does customer tenure relate to churn?
4. Do payment methods influence churn behavior?
5. Which customer segments are most at risk of churning?

---

## 🧹 Data Preparation & Cleaning
Key data preparation steps:
- Converted `TotalCharges` from object to numeric format
- Removed a small number of rows with missing `TotalCharges`, which were caused by new customers with zero tenure
- Verified that the target variable `Churn` contains only valid categories (`Yes`, `No`)

After cleaning:
- 7,032 customer records remained for analysis

---

## 📊 Key Insights

### 1️⃣ Overall Churn Rate
- The overall churn rate is approximately **26.6%**
- This level is relatively high for a subscription-based business, indicating a retention challenge

---

### 2️⃣ Contract Type & Churn
- **Month-to-month contracts** show the highest churn rate
- Long-term contracts (one-year and two-year) are associated with significantly lower churn

**Interpretation:**  
Low switching costs and lack of commitment contribute to higher churn among month-to-month customers.

---

### 3️⃣ Tenure & Churn
- Customers in their **first 12 months** have the highest churn rate
- Churn decreases steadily as customer tenure increases

**Interpretation:**  
Early-stage customers represent the most critical retention segment.

---

### 4️⃣ Payment Method & Churn
- Customers using **electronic check** exhibit higher churn compared to those using automatic payment methods
- Automatic payments (credit card or bank transfer) are associated with lower churn

**Interpretation:**  
Higher payment friction may increase the likelihood of churn.

---

## 💡 Business Recommendations

- **Strengthen early-stage onboarding** to improve retention during the first year
- **Encourage migration from month-to-month to long-term contracts** using incentives or discounts
- **Promote automatic payment methods** to reduce payment friction
- **Segment retention strategies** based on tenure, contract type, and payment behavior

---

## 🛠 Tools & Libraries
- Python
- pandas
- matplotlib
- seaborn

---

## 📌 Notes & Limitations
- The analysis is descriptive and does not include predictive modeling
- Behavioral usage data was not available and could further enhance churn understanding
- Results are based on historical data and should be validated with ongoing monitoring

---

## 🚀 Next Steps
Potential extensions of this analysis include:
- Cohort-based churn analysis
- Predictive churn modeling
- Measuring the impact of retention initiatives over time

---

## 👤 Author
Junior Data Analyst Portfolio Project  
Python-based exploratory data analysis
