# 🚀 Customer Churn Analysis

### 📓 Notebook: [Project TCA.ipynb](./Project%20TCA.ipynb)

### 🧾 Summary Report: [Customer Churn Analysis Summary.pdf](./Customer%20Churn%20Analysis%20Summary.pdf)

---

## 🎯 Problem Statement

This project dives deep into a telecom dataset of **7,043 customers** to uncover what truly drives **customer churn** — why customers leave and what factors influence their decisions.
With **26.54%** of customers having already churned, the challenge is clear: **identify the pain points** and **build strategies to retain customers** before they walk away.

---

## ⚙️ Project Workflow

### 1️⃣ **Data Loading**

* Imported `Customer Churn.csv` into a Pandas DataFrame.
* Used `.head()` and `.info()` to understand structure, columns, and data types.

### 2️⃣ **Data Cleaning & Preprocessing**

* Replaced blank spaces in `TotalCharges` (for zero-tenure customers) with “0” and converted it to float.
* Verified data quality — no missing values or duplicate `customerID`s found.
* Converted `SeniorCitizen` values (0/1) into human-readable labels ("No"/"Yes").

### 3️⃣ **Exploratory Data Analysis (EDA)**

Uncovered patterns and churn behavior using **Matplotlib** and **Seaborn** visualizations:

📊 **Key Analyses:**

* **Churn Distribution:** 26.54% overall churn rate.
* **Demographics:** Gender and senior citizen status examined for churn impact.
* **Tenure:** High churn observed among **newer customers**.
* **Contract Type:** **Month-to-Month** plans show highest churn.
* **Payment Method:** **Electronic Check** users churn more often.
* **Services Impact:** Evaluated how features like `TechSupport`, `OnlineBackup`, and `DeviceProtection` affect churn — customers **without** these add-ons are more likely to leave.

### 4️⃣ **Insight Synthesis**

Combined data stories into actionable insights — summarized in the [Summary PDF](./Customer%20Churn%20Analysis%20Summary.pdf).

---

## 📈 Key Visualizations

### 🔹 Churn Distribution

![Churn Pie Chart](https://user-images.githubusercontent.com/102996550/...)
*(Replace placeholder with actual uploaded image link)*

### 🔹 Churn vs Tenure

![Churn vs Tenure Histogram](https://user-images.githubusercontent.com/102996550/...)
*(Replace placeholder with actual uploaded image link)*

---

## 💡 Major Insights (from Summary Report)

### 🔍 **Key Findings**

* **Overall Churn:** 26.54% (1,869 out of 7,043 customers).
* **Contract Type:** Month-to-Month users churn **2x more** than long-term ones.
* **Tenure:** New customers show highest churn risk.
* **Payment Method:** Electronic Check users are the most unstable group.
* **Senior Citizens:** Churn at **41.7%**, nearly double non-seniors.
* **Internet Service:** **Fiber Optic** users churn more than DSL users.
* **Add-On Services:** Lack of `OnlineSecurity`, `Backup`, or `TechSupport` increases churn risk dramatically.

---

## 🧠 Conclusion

Customer churn is concentrated among:

* **Low-tenure** users
* **Month-to-month** contracts
* **Senior citizens**
* **Fiber Optic** internet users
* **Electronic Check** payment users
* And customers **without** additional security/support services

The story is simple — **engagement and perceived value** determine loyalty.

---

## 🎯 Recommendations

To reduce churn and boost retention:

1. **Incentivize long-term contracts** (1-year / 2-year plans).
2. **Engage new customers early** — the first few months are critical.
3. **Investigate senior & fiber user dissatisfaction** — pricing, service quality, or complexity.
4. **Simplify or upgrade payment experiences**, especially for Electronic Check users.
5. **Promote add-on services** like Tech Support and Online Security to improve user stickiness.

---

## 🏁 Final Thoughts

This analysis goes beyond numbers — it helps businesses **see the human side of churn**.
By understanding what makes customers stay or leave, telecom companies can design better experiences, improve satisfaction, and ultimately **build loyalty that lasts**.
✨ *Data doesn’t lie — it tells the story you need to hear.*

---
