# 📊 Customer Churn Analytics & Retention Strategy Dashboard

## 📌 Executive Summary

In a subscription-based telecom business, customer churn directly impacts revenue stability, customer lifetime value (CLV), and acquisition cost efficiency.

This project delivers an **end-to-end churn analytics solution**, combining structured ETL in SQL Server with an executive-level Power BI dashboard to uncover churn drivers, customer risk segments, and actionable retention strategies.

Rather than stopping at descriptive analytics, this project frames churn as a **strategic business problem**, translating data patterns into commercially relevant insights.

---

## 🎯 Business Objectives

The project aims to:

* Quantify overall churn exposure and revenue risk
* Identify high-risk customer segments
* Understand behavioral and contractual drivers of churn
* Detect service-level weaknesses
* Provide a foundation for churn prediction modeling
* Support marketing & retention campaign targeting

---

## 🛠 Tools & Technologies

* **SQL Server (SSMS)** – ETL, data cleaning, staging & production layer
* **Power BI** – Data modeling, DAX measures, executive dashboard
* **Python** – Predictive modeling & ML experimentation
* **Data Warehousing Concepts** – Staging → Production → BI Views
* **Consulting Framework Applied** – Segmentation, Risk Profiling, Revenue Impact Thinking

---

# 🏗 Project Architecture

## STEP 1 — SQL ETL Layer

* Created dedicated database: `db_Churn`
* Imported raw CSV into staging table (`stg_Churn`)
* Performed:

  * Null diagnostics
  * Data type adjustments
  * Standardization using `ISNULL`
* Promoted clean data into production table (`prod_Churn`)
* Created analytical views:

  * `vw_ChurnData`
  * `vw_JoinData`

This ensures:
✔ Data integrity
✔ Reusability
✔ Scalability for recurring loads

---

## STEP 2 — Data Modeling in Power BI

### Derived Analytical Columns

* **Churn Status (Binary)**
* **Monthly Charge Range Segmentation**
* **Age Group Mapping with Custom Sorting**
* **Tenure Group Segmentation**
* **Service Unpivot Transformation**

These transformations enable multi-dimensional analysis across:

* Demographics
* Geographic exposure
* Account behavior
* Service adoption
* Revenue contribution

---

## 📊 Executive Dashboard Structure

### 1️⃣ Top KPI Panel

* Total Customers: **6,418**
* New Joiners: **411**
* Total Churn: **1,732**
* Churn Rate: **26.99%**

A churn rate of ~27% signals significant retention pressure in a competitive telecom environment.

---

# 🔍 Key Analytical Insights

## 👥 1. Demographic Risk Profiling

* Customers aged **>50 represent 42.5% of total customer base (2,729 users)**.
* This segment has the largest absolute churn exposure.
* Female customers account for the majority of churn share (>50%).

**Consulting Interpretation:**
Older customers represent revenue concentration risk.
Retention strategy must prioritize loyalty reinforcement and contract stabilization within this segment.

---

## ⏳ 2. Tenure vs Churn Behavior

Across tenure groups:

* Customer count ranges from **962 to 1,943**
* Churn rate ranges between **25.05% – 27.73%**
* Highest divergence occurs in customers with **>24 months tenure**

**Interpretation:**
Long-tenured customers are numerous but still exhibit churn vulnerability.

This indicates:

* Possible contract expiry effects
* Competitive targeting
* Price sensitivity over time

Retention campaigns should activate **pre-expiry engagement programs** before 24 months.

---

## 💳 3. Payment Method Risk Exposure

Churn Rate by Payment Method:

* **Mailed Check: 37.82% (Highest Risk)**
* Bank Withdrawal: 34.43%
* Credit Card: 14.80% (Lowest Risk)

**Consulting Insight:**
Manual payment methods correlate strongly with churn.

Implication:

* Customers paying via mailed check are less digitally integrated.
* Promote auto-payment incentives to reduce churn risk.

---

## 📄 4. Contract Structure Impact

* Month-to-Month contracts show highest churn (~46%+)
* 2-Year contracts show minimal churn (~2.7%)

**Strategic Recommendation:**
Introduce structured discount migration:
Month-to-Month → 1-Year → 2-Year

Contract length is the strongest structural churn stabilizer.

---

## 🌍 5. Geographic Concentration

Top churn rate states show significant variation, with certain regions exceeding 50%.

This suggests:

* Regional competitive intensity
* Service quality variability
* Local pricing pressure

Further operational audit recommended in high-churn states.

---

## 🧠 6. Primary Churn Drivers

Churn Category Distribution:

* **Competitor is the dominant reason (761 cases)**
* Followed by Attitude & Dissatisfaction
* Price-related churn remains significant

This confirms churn is primarily:

* Competitive displacement
* Experience-driven, not purely pricing-driven

Retention strategy must focus on:

* Competitive positioning
* Service quality reinforcement
* Customer experience monitoring

---

## 📡 7. Service-Level Weakness Signals

Certain services show disproportionately high churn participation.

Possible interpretations:

* Weak perceived value
* Service reliability issues
* Poor bundling strategy

Further deep dive recommended into:

* Internet type performance (Fiber shows high churn exposure)
* Device Protection & Add-on services

---

# 📈 Strategic Recommendations

Based on the analysis:

### 1️⃣ Contract Optimization Strategy

Migrate high-risk month-to-month customers to longer-term agreements.

### 2️⃣ Payment Automation Campaign

Incentivize digital auto-pay conversion.

### 3️⃣ Competitor Defense Program

Target customers nearing renewal with:

* Personalized offers
* Loyalty pricing
* Service upgrade bundles

### 4️⃣ Segment-Based Retention

Prioritize:

* Age > 50
* Tenure > 24 months
* Mailed Check users

### 5️⃣ Future Phase — Predictive Modeling

Develop ML model (Logistic Regression / XGBoost) to:

* Predict churn probability
* Score customers
* Trigger automated retention workflows

---

# 🧩 Business Value Delivered

This project demonstrates:

* End-to-end analytics ownership (Data → ETL → Modeling → Visualization → Strategy)
* Ability to convert raw data into business recommendations
* Commercial awareness beyond dashboarding
* Consulting-style problem framing

---

# 📌 Why This Project Matters

Churn analytics is not about counting lost customers.
It is about understanding:

* Revenue leakage
* Behavioral risk signals
* Structural weaknesses in product and pricing strategy

This project positions data as a **decision-enabling asset**, not just a reporting function.

* Or tailor it specifically for consulting / tech / telco recruiters 🚀


## 📸 Dashboard Preview
