📊 Telco Customer Churn Analysis & Insights ✨

🚀 Project Overview

Ever wondered why customers leave a service? 🤔 Customer churn is a critical metric for subscription-based businesses like Telcos. This project performs an Exploratory Data Analysis (EDA) on a popular Telco customer dataset to uncover the key factors driving customers away.

By visualizing customer demographics, account details, and service usage, we identify patterns that predict churn and provide actionable insights to help improve customer retention strategies. Let's dive into the data! 💡

🎯 Key Findings - What Drives Churn?

Our analysis pinpointed several crucial factors linked to higher customer churn:

📉 Overall Churn Rate: Around 26.5% of customers in the dataset churned.

📅 Contract Type: Month-to-Month contracts show significantly higher churn compared to Annual or Two-Year contracts. Flexibility comes at a cost!

⏳ Customer Tenure: Newer customers (low tenure, especially in the first few months) are far more likely to leave. Loyalty builds over time!

💳 Payment Method: Customers paying via Electronic Check churn more often than those using other methods (credit card, bank transfer, mailed check).

👴 Senior Citizens: This group, while smaller, churns at nearly double the rate (~41.7%) of non-seniors (~23.6%).

🌐 Internet Service: Fiber Optic customers have a higher churn rate compared to DSL users. Is the perceived value or service quality not meeting expectations?

🔒 Add-on Services: Customers without value-added services like Online Security, Online Backup, Device Protection, and Tech Support are more likely to churn. These services act as retention anchors!

For a more detailed breakdown, please see the customer_churn_summary.md file.

🛠️ Get Started - How to Run the Analysis

Ready to explore the data yourself? Here’s how:

Clone the Repository:

git clone <your-repository-url>
cd <repository-directory>


Install Dependencies: Make sure you have the necessary Python libraries.

pip install pandas numpy matplotlib seaborn notebook


Launch the Analysis:

Jupyter Notebook: Run jupyter notebook and open Project 1 TCA.ipynb.

Python Script: Execute the Python script directly. The script will print outputs and save plots as PNG files.

python telco_churn_analysis.py


Dataset: The analysis requires the Customer Churn.csv file. (Make sure it's in the root directory or update the script path).

💾 Data Source

This analysis utilizes the standard Telco Customer Churn dataset, often available on platforms like Kaggle. It includes customer demographics, account information, subscribed services, and churn status.

💻 Tech Stack

Language: Python 3.x

Libraries:

Pandas (Data Manipulation)

NumPy (Numerical Operations)

Matplotlib (Plotting)

Seaborn (Enhanced Visualization)

Environment: Jupyter Notebook / Standard Python Interpreter

✨ Visualizations

The analysis generates several plots (saved as .png files) to illustrate the findings, including:

Overall Churn Distribution (Count & Percentage)

Churn Rate by Gender, Senior Citizen Status, Contract Type, Payment Method

Tenure Distribution for Churned vs. Retained Customers

Churn Across Different Subscribed Services (Phone, Internet, Add-ons)

🤝 Contributing

Got ideas to improve this analysis? Contributions, issues, and feature requests are welcome! Please feel free to fork the repository, make changes, and submit a pull request.

Fork the Project

Create your Feature Branch (git checkout -b feature/AmazingFeature)

Commit your Changes (git commit -m 'Add some AmazingFeature')

Push to the Branch (git push origin feature/AmazingFeature)

Open a Pull Request

📄 License

Distributed under the MIT License. See LICENSE file for more information. (Remember to add a https://www.google.com/search?q=LICENSE file if you haven't already).

Thanks for checking out the project! Feel free to reach out with any questions. 😊
