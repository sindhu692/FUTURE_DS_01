# TASK 02 – Customer Retention & Churn Analysis

## 📌 Project Title
**Telecom Customer Churn Analytics**

## 🎯 Objective
The objective of this project is to analyze telecom customer data to identify **churn patterns, key retention drivers, and revenue impact**, and to provide **actionable, data-driven recommendations** to reduce customer churn and improve long-term retention.

---

## 🧠 Business Problem
Customer churn is a critical challenge in the telecom industry due to high competition and low switching costs.  
Losing customers leads to:
- Recurring revenue loss  
- Increased acquisition costs  
- Reduced customer lifetime value  

Reducing churn even by a small percentage can significantly improve overall profitability.

---

## 🛠 Tools & Technologies Used
- **Python** (Pandas, NumPy, Matplotlib, Seaborn)
- **SQL (MySQL)** – KPI & churn analysis
- **Tableau** – Interactive dashboard
- **Jupyter Notebook**
- **Excel / CSV datasets**

---

## 📂 Folder Structure

---

## 📊 Dataset Overview
- **Source:** IBM Sample Telco Customer Churn Dataset  
- **Records:** 7,043 customers  
- **Granularity:** Customer-level  
- **Target Variable:** `Churn (Yes / No)`

### Key Data Categories
- Customer Demographics (Gender, Senior Citizen, Partner, Dependents)
- Services Subscribed (Internet, Tech Support, Streaming, Security)
- Account & Billing (Tenure, Contract, Payment Method, Charges)

---

## 🧹 Data Cleaning & Preparation (Python)
Key steps performed in `DATA_CLEANING.ipynb`:
- Standardized column names
- Removed duplicate records
- Fixed incorrect data types
- Handled missing values using median imputation
- Treated outliers using IQR method
- Feature engineering (`avg_monthly_spend`)
- Encoded target variable (`churn_flag`)
- Exported analytics-ready dataset

---

## 🔍 Exploratory Data Analysis (EDA)
### Key Findings:
- **Early-tenure customers (0–12 months)** have the highest churn
- **Higher monthly charges** increase churn probability
- **Month-to-month contracts** show significantly higher churn
- **Electronic check** payment method has the highest churn rate
- Customers without **technical support** churn more frequently

---

## 🗄 SQL Analysis & KPIs
SQL was used to analyze churn drivers and revenue impact:
- Overall churn rate: **26.54%**
- Total customers: **7,043**
- Revenue lost due to churn: **₹2.86M**
- Month-to-month contracts churn rate: **42.71%**
- Electronic check churn rate: **45.29%**

Custom views created:
- `vw_kpis` – Overall churn & revenue metrics  
- `vw_contract_churn` – Contract-level churn analysis  

---

## 📈 Tableau Dashboard
An interactive **Telecom Customer Churn Analytics Dashboard** was built to visualize:
- Overall KPIs (Customers, Churn Rate, Revenue Loss)
- Churn by contract type
- Payment method & internet service impact
- Monthly charges vs churn
- Customer tenure distribution
- Revenue loss by segment

The dashboard enables **business-friendly interpretation** of churn patterns.

---

## 🔑 Key Business Insights
- Month-to-month customers are the **highest-risk segment**
- Early onboarding (first year) is critical to reduce churn
- Automatic payment methods improve retention
- High-paying customers cause **significant revenue loss when churned**
- Technical support plays a strong role in customer retention

---

## 📌 Recommendations
- Promote **long-term contracts** with incentives
- Encourage **automatic payment methods**
- Strengthen **early-stage onboarding programs**
- Improve **fiber optic service quality**
- Implement **targeted retention offers** for high-value customers

---

## 🚀 Future Scope
- Build a **predictive churn model**
- Implement customer risk scoring
- Design personalized retention strategies
- Integrate churn alerts into business dashboards

---

## 📎 Outcome
This project delivers a **real-world, end-to-end churn analysis** combining Python, SQL, and Tableau to support **data-driven retention strategies** and **business decision-making**.

---

📌 **Author:** K.Sindhu Sree
📌 **Role:** Data Science & Analytics Intern  
📌 **Organization:** Future Interns

