# Customer Churn Analysis

### Notebook Link : [Project TCA.ipynb](./Project%20TCA.ipynb)
### Summary Link : [Customer Churn Analysis Summary.pdf](./Customer%20Churn%20Analysis%20Summary.pdf)

## 📊 Problem Statement

[cite_start]This analysis explores a dataset of 7043 telecom customers to understand the factors driving customer churn[cite: 2]. The goal is to identify key characteristics and service interactions associated with customers leaving the service, thereby highlighting areas for potential improvement in retention strategies. [cite_start]Approximately 26.54% of the customer base has churned, indicating a significant need to address customer retention[cite: 3, 4].

## ⚙️ Steps Followed

1.  **Load Data:** The dataset (`Customer Churn.csv`) was loaded into a Pandas DataFrame. Initial inspection was done using `.head()` and `.info()` to understand the structure and data types.
2.  **Data Cleaning & Preprocessing:**
    * The `TotalCharges` column contained blank spaces for customers with zero tenure; these were replaced with "0" and the column was converted to a float data type.
    * Checked for any remaining null values across the dataset using `.isnull().sum()`. No other nulls were found.
    * Checked for duplicate `customerID` entries; none were found.
3.  **Data Transformation:** The `SeniorCitizen` column, originally encoded as 0 and 1, was converted to "no" and "yes" respectively for better readability in visualizations.
4.  **Exploratory Data Analysis (EDA):**
    * Used Matplotlib and Seaborn libraries to create various visualizations to understand churn patterns.
    * [cite_start]Analyzed the overall churn distribution using a countplot and calculated the churn percentage (26.54%) using a pie chart[cite: 3].
    * Investigated churn based on demographic features like `gender` and `SeniorCitizen` using countplots and stacked bar charts.
    * [cite_start]Examined the relationship between `tenure` and churn using a histogram, revealing higher churn among newer customers[cite: 8, 9].
    * [cite_start]Analyzed the impact of `Contract` type on churn using a countplot, showing significantly higher churn for Month-to-Month contracts[cite: 5, 6].
    * [cite_start]Visualized churn rates across different `PaymentMethod` options, highlighting Electronic Check users as having higher churn[cite: 11].
    * [cite_start]Generated countplots for various services (`PhoneService`, `MultipleLines`, `InternetService`, `OnlineSecurity`, `OnlineBackup`, `DeviceProtection`, `TechSupport`, `StreamingTV`, `StreamingMovies`) against churn status to identify service-related churn factors[cite: 15, 18, 19, 20, 21, 22, 23].
5.  **Summary and Insights:** Findings from the EDA were synthesized, key churn drivers identified, and recommendations were formulated (detailed in the Summary PDF and Insights section below).

## 📈 Key Visualizations

### Churn Distribution (%)
![Churn Pie Chart](https://user-images.githubusercontent.com/102996550/...) *(Self-correction: Placeholder - you would need to generate and upload this image to GitHub and replace the URL)*

### Churn vs Tenure
![Churn vs Tenure Histogram](https://user-images.githubusercontent.com/102996550/...) *(Self-correction: Placeholder - you would need to generate and upload this image to GitHub and replace the URL)*

## 💡 Insights (Based on `Customer Churn Analysis Summary.pdf`)

The analysis revealed several key factors strongly correlated with customer churn:

### [1] Key Findings
* [cite_start]**Overall Churn Rate:** 26.54% (1869 out of 7043 customers)[cite: 3].
* [cite_start]**Contract Type:** Month-to-Month contracts have a significantly higher churn rate compared to One-year or Two-year contracts[cite: 5, 6].
* [cite_start]**Tenure:** Newer customers (low tenure) are much more likely to churn; loyalty increases with longer tenure[cite: 8, 9, 10].
* [cite_start]**Payment Method:** Electronic Check users show a considerably higher propensity to churn[cite: 11, 12].
* [cite_start]**Senior Citizens:** Representing 16.2% of the base, senior citizens churn at a higher rate (41.7%) compared to non-seniors (23.6%)[cite: 13, 14].
* [cite_start]**Internet Service:** Customers with Fiber Optic service churn more often than those with DSL or no internet[cite: 15, 16].
* [cite_start]**Add-on Services:** Lack of key add-ons (Online Security, Online Backup, Device Protection, Tech Support) correlates with higher churn rates[cite: 18, 19, 20, 21, 22, 23]. [cite_start]Customers with these services exhibit better retention[cite: 24].

### [2] Conclusion
[cite_start]Churn is concentrated among customers with **low tenure**, **month-to-month contracts**, **senior citizens**, those using **Fiber Optic** internet, and those paying via **Electronic Check**[cite: 26, 27, 28]. [cite_start]Furthermore, not subscribing to value-added security and support services is strongly linked to higher churn[cite: 28].

### [3] Recommendations
[cite_start]Retention efforts should prioritize[cite: 29]:
* [cite_start]Incentivizing longer contract terms (One-year, Two-year)[cite: 30].
* [cite_start]Targeting support and engagement initiatives towards new customers in their initial months[cite: 31].
* [cite_start]Investigating reasons for high churn among senior citizens and Fiber Optic users (e.g., pricing, service issues)[cite: 32].
* [cite_start]Understanding and addressing friction points related to Electronic Check payments[cite: 33].
* [cite_start]Promoting the benefits of add-on security and tech support services to increase customer loyalty[cite: 33].
