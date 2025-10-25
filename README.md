📊 Telco Customer Churn Analysis

🚀 Overview

This project dives into a Telco customer dataset to understand the factors contributing to customer churn (customers leaving the service). By analyzing various customer attributes, service subscriptions, and contract details, we aim to identify key drivers of churn and provide actionable insights for improving customer retention.

Understanding why customers leave is crucial for any subscription-based business. This analysis uses exploratory data analysis (EDA) and visualization to uncover patterns and correlations associated with churn.

🎯 Key Findings & Insights

Our analysis revealed several significant factors influencing customer churn:

Overall Churn Rate: ~26.5% of the customers in this dataset have churned.

Contract Flexibility Matters: Customers on Month-to-Month contracts churn at a significantly higher rate than those on longer One-year or Two-year contracts.

Loyalty Grows with Time: Newer customers (low tenure) are much more likely to leave. Retention increases substantially the longer a customer stays.

Payment Method Impact: Using Electronic Check is associated with a notably higher churn rate compared to other payment methods.

Senior Citizens are Higher Risk: While a smaller segment, Senior Citizens churn at almost double the rate (~41.7%) compared to non-seniors (~23.6%).

Fiber Optic Challenges: Customers using Fiber Optic internet show a higher churn rate than DSL users, suggesting potential service or pricing dissatisfaction.

Value-Added Services Boost Retention: Customers without services like Online Security, Online Backup, Device Protection, and Tech Support are more prone to churning. These services seem to enhance customer loyalty.

For a detailed summary, see the customer_churn_summary.md file.

🛠️ How to Use

Clone the repository:

git clone <your-repository-url>
cd <repository-directory>


Ensure you have the required libraries:

pandas

numpy

matplotlib

seaborn

Jupyter Notebook/JupyterLab

pip install pandas numpy matplotlib seaborn notebook


Run the Jupyter Notebook:
Open and run the Project 1 TCA.ipynb notebook to see the full analysis, code, and visualizations.

Dataset: The analysis uses the Customer Churn.csv file. (Ensure this file is present in the repository or provide download instructions if it's external).

💾 Data Source

The dataset used in this analysis is the Telco Customer Churn dataset, commonly found on platforms like Kaggle. It contains information about customer demographics, subscribed services, account details, and churn status.

💻 Technologies Used

Python: Primary programming language.

Pandas: Data manipulation and analysis.

NumPy: Numerical operations.

Matplotlib & Seaborn: Data visualization.

Jupyter Notebook: Interactive coding and analysis environment.

🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the issues page or submit a pull request.

📄 License

This project is licensed under the MIT License - see the https://www.google.com/search?q=LICENSE file for details. (You'll need to add an MIT License file if you choose this license).

Thank you for exploring this customer churn analysis!
