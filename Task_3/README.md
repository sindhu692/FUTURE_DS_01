# 📊 Funnel Performance & Growth Insights

## 📌 Project Overview

This project analyzes lead conversion performance and revenue growth using a Power BI dashboard built from cleaned CRM deal data.

The dashboard provides actionable insights into:

* Lead conversion effectiveness
* Revenue contribution by lead source
* Customer value trends
* Monthly performance patterns
* Lead behaviour insights

---

## 🎯 Business Objectives

✔ Measure lead-to-customer conversion performance
✔ Identify high-performing lead sources
✔ Track revenue contribution patterns
✔ Understand customer value distribution
✔ Monitor monthly growth trends

---

## 📂 Dataset

**Primary Dataset:** CRM Deals Data

Key fields used:

* lead_type
* business_segment
* declared_monthly_revenue
* won_date
* lead_behaviour_profile
* month & year

---

## 🧹 Data Preparation

Data cleaning and preprocessing were performed using Python.

### Steps performed:

* Removed duplicates
* Handled missing values
* Standardized categorical fields
* Converted date columns
* Created derived metrics

📄 Notebook: `notebook/Data_cleaning.ipynb`

---

## 📐 Data Modeling & Measures (Power BI)

### ✅ Customers (Converted Leads)

```
Customers =
CALCULATE(
    COUNTROWS('cleaned_deals'),
    NOT(ISBLANK('cleaned_deals'[won_date]))
)
```

### ✅ Total Leads

```
Total Leads = COUNTROWS('cleaned_deals')
```

### ✅ Conversion Rate

```
Conversion Rate =
DIVIDE([Customers], [Total Leads])
```

### ✅ Funnel Stage Column

```
Funnel Stage =
IF(
    ISBLANK('cleaned_deals'[won_date]),
    "Lead",
    "Customer"
)
```

---

## 📊 Dashboard KPIs

* **Total Leads**
* **Customers**
* **Conversion Rate**
* **Average Customer Value**
* **Total Revenue**

---

## 📈 Dashboard Visuals & Insights

### 🔹 Lead Count by Lead Type

Identifies which sources generate the highest volume of leads.

### 🔹 Customer Value by Lead Type

Shows which lead sources produce higher-value customers.

### 🔹 Revenue by Lead Type

Highlights top revenue-driving channels.

### 🔹 Average Customer Value by Segment

Helps identify profitable customer segments.

### 🔹 Monthly Customers vs Leads Trend

Tracks growth patterns and seasonal trends.

### 🔹 Lead Behaviour Profile Performance

Reveals which behaviour patterns convert best.

---

## 🧠 Key Insights

✔ Online channels generate the majority of leads
✔ Industry leads show higher customer value
✔ Peak conversions occur during mid-year months
✔ Behaviour-driven leads demonstrate stronger conversion potential

---

## 🛠 Tools & Technologies

* **Python (Pandas, NumPy)** — data cleaning
* **Power BI** — dashboard & analytics
* **GitHub** — version control & documentation

---

## 🖼 Dashboard Preview

![Dashboard Preview](images/dashboard_preview.png)

---

## 🚀 How to Use

1. Download the `.pbix` file from the **dashboard** folder
2. Open in Power BI Desktop
3. Refresh data if needed
4. Explore insights using filters & visuals

---

## 📌 Project Value

This dashboard demonstrates:

✔ Data cleaning & preprocessing
✔ Data modeling & DAX measures
✔ Business intelligence storytelling
✔ KPI & performance tracking
✔ Executive-ready dashboard design

---

## 👩‍💻 Author

** K.Sindhu Sree**

---

⭐ If you found this project useful, consider giving it a star!
