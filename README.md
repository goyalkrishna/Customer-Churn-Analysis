📊 Telecom Customer Churn Analysis

An in-depth analysis of 7,043 customer records to identify the key drivers of churn and provide actionable retention strategies.

📓 Analysis Notebook: Project TCA.ipynb

📄 Executive Summary: Customer Churn Analysis Summary.pdf

🎯 The Challenge: Why Are Customers Leaving?

This project dives into a telecom dataset to answer one critical question: Why are 26.54% of customers leaving?

The goal is to move beyond the numbers, identify the key drivers of this attrition, and provide a clear action plan to improve customer retention, reduce revenue loss, and strengthen loyalty.

⚙️ Our Analysis Workflow

Load Data: The dataset (Customer Churn.csv) was loaded into a Pandas DataFrame. Initial inspection was done using .head() and .info() to understand the structure and data types.

Data Cleaning & Preprocessing:

Identified and resolved an issue in the TotalCharges column, where blank spaces (for 0-tenure customers) were replaced with "0" and the column type was converted to float.

Conducted a full scan for null values and duplicate customerID entries (none were found).

Data Transformation: The SeniorCitizen column (originally 0/1) was re-encoded to "No" and "Yes" for clearer and more intuitive visualizations.

Exploratory Data Analysis (EDA):

Used Matplotlib and Seaborn to build a visual story of churn patterns.

Analyzed the overall 26.54% churn rate with pie and count plots.

Investigated demographic impacts (gender, SeniorCitizen).

Plotted tenure vs. churn, revealing a critical drop-off in the first few months.

Analyzed the massive impact of Contract type, showing "Month-to-Month" as the highest risk.

Identified "Electronic Check" as the PaymentMethod with the highest churn correlation.

Mapped churn across all services (InternetService, OnlineSecurity, TechSupport, etc.) to find which services improve "stickiness."

Synthesize & Recommend: All visual findings were consolidated into a final summary (see PDF) to build a clear profile of an at-risk customer and propose targeted solutions.

📈 Key Visualizations: The Story in the Data

Churn Distribution (%)

Churn vs. Customer Tenure





Finding: Over 1 in 4 customers (26.54%) has left the service, highlighting a critical retention gap.

Finding: Churn is heavily concentrated among new customers. Loyalty builds significantly after the first year.

Churn by Contract Type

Churn by Payment Method





Finding: "Month-to-Month" contracts are the single biggest risk factor, with a churn rate dramatically higher than 1 or 2-year plans.

Finding: "Electronic Check" users are far more likely to churn, suggesting payment friction or a lack of auto-pay "lock-in."

💡 Insights & Recommendations

🔍 Key Churn Drivers: The "Who" and "Why"

Analysis of the summary PDF reveals a clear profile of the at-risk customer:

⏳ Tenured: They are often new customers (low tenure).

📝 Contractual: They are on a Month-to-Month contract.

👴 Demographic: They are Senior Citizens (41.7% churn rate vs 23.6% for non-seniors).

💻 Service: They use Fiber Optic internet (which, despite being a premium service, has higher churn).

💳 Payment: They pay via Electronic Check.

🛡️ Add-ons: They have not subscribed to "sticky" services like OnlineSecurity, OnlineBackup, or TechSupport.

🚀 Actionable Recommendations: How to Fix It

Based on the data, retention efforts should be surgical and targeted:

✅ Incentivize Loyalty: Create special offers to migrate Month-to-Month customers to 1 or 2-year contracts. The data shows this is the most effective way to secure retention.

🤝 Onboard New Customers: Implement a proactive "first 90 days" engagement program for new customers (especially low-tenure) to offer support and build value.

🔍 Investigate Friction:

Why are Senior Citizens leaving? Is the tech too complex? Is the value proposition unclear?

Why is Fiber Optic churn so high? Investigate service reliability, pricing, and competitor offers.

Why Electronic Check? Analyze this payment journey for friction points and proactively encourage "set it and forget it" auto-pay.

🎁 Bundle for Stickiness: Promote and bundle services like Online Security and Tech Support. The data proves that customers who use these services are far less likely to leave.
