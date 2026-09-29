# customer_behavior_analysis
Data analytics project showcasing customer behavior analysis using Python,sql and power bi
📊 Data Analytics Project
📌 Overview

This project demonstrates an end-to-end Data Analytics workflow, starting from raw data loading and cleaning in Python, followed by Exploratory Data Analysis (EDA), SQL analysis using MySQL, and finally the creation of an interactive Power BI dashboard.

The main objective of the project is to transform raw data into meaningful insights that can support data-driven business decisions.

📂 Dataset

The project uses a structured dataset containing customer and purchase-related information.

The dataset was initially loaded and explored using Python to understand:

Number of rows and columns
Data types
Missing values
Duplicate records
Unique values
Numerical and categorical variables
Data quality issues

The dataset was then cleaned and prepared for further analysis.

🛠️ Tools & Technologies
Tool	Purpose
Python	Data loading, cleaning and EDA
Pandas	Data manipulation and cleaning
MySQL	SQL-based data analysis
Power BI	Interactive dashboard and visualization
Google Colab	Python analysis environment
🔄 Project Workflow

The project follows these main steps:

Raw Dataset
     ↓
Load Data in Python
     ↓
Data Cleaning
     ↓
Exploratory Data Analysis (EDA)
     ↓
Export Cleaned Dataset
     ↓
Load Data into MySQL
     ↓
SQL Analysis
     ↓
Power BI Dashboard
     ↓
Business Insights & Results
1️⃣ Data Loading

The dataset was imported into Python using Pandas.

Key activities included:

Loading the dataset
Checking dataset shape
Inspecting columns and data types
Understanding the structure of the data
Identifying potential data quality issues

Example:

import pandas as pd

df = pd.read_csv("dataset.csv")

df.head()
df.info()
df.shape
2️⃣ Data Cleaning

Data cleaning was performed to improve the quality and consistency of the dataset.

The main cleaning activities included:

Handling missing values
Removing duplicate records
Correcting data types
Standardizing categorical values
Handling inconsistent values
Checking for invalid or unexpected data
Preparing the cleaned dataset for analysis

After cleaning, the dataset was validated before moving to the analysis stage.

3️⃣ Exploratory Data Analysis (EDA)

EDA was performed to understand patterns, trends, and relationships within the data.

The analysis included:

Descriptive statistics
Distribution analysis
Category-wise analysis
Customer segmentation
Purchase behavior analysis
Correlation analysis
Trend identification
Visualization of important variables

Python libraries such as Pandas, Matplotlib, and Seaborn were used for EDA.

4️⃣ SQL Analysis — MySQL

After cleaning the dataset, it was imported into MySQL Server for further analysis.

SQL queries were used to answer business-related questions such as:

How many customers are there?
What is the average purchase amount?
What is the total revenue?
Which customer segments generate the most revenue?
How does spending differ by subscription status?
Which categories have the highest sales?
What are the key customer purchasing patterns?

SQL concepts used in the project include:

SELECT
WHERE
GROUP BY
ORDER BY
HAVING
CASE
Aggregate functions such as COUNT(), SUM(), and AVG()
JOIN
Common Table Expressions (CTEs)

Example:

SELECT 
    subscription_status,
    COUNT(customer_id) AS total_customers,
    ROUND(AVG(purchase_amount), 2) AS average_spend,
    SUM(purchase_amount) AS total_revenue
FROM cleaned_purchase_data
GROUP BY subscription_status
ORDER BY total_revenue DESC;
5️⃣ Power BI Dashboard

The cleaned and analyzed data was used to build an interactive Power BI dashboard.

The dashboard is structured into different sections to make the analysis easy to understand.

📌 Dashboard Sections
Overview

Provides a high-level summary using important KPIs such as:

Total Customers
Total Revenue
Average Purchase Amount
Number of Purchases
Customer Analysis

Shows customer-related insights such as:

Customer segments
Subscription status
Purchasing behavior
Customer distribution
Purchase Analysis

Highlights:

Purchase trends
Category performance
Average spending
Revenue contribution
Key Insights

Summarizes the most important findings from the analysis in a business-friendly format.

📈 Dashboard

The Power BI dashboard provides interactive visualizations that allow users to explore the data using filters, slicers, charts, and KPI cards.

Dashboard Preview:

Add your Power BI dashboard screenshot here.

Example:

![Power BI Dashboard](images/dashboard.png)
🎯 Results & Insights

The project converts raw customer and purchase data into actionable insights.

The analysis helps identify:

Customer purchasing patterns
Differences between customer segments
Revenue contribution across categories
Spending behavior based on subscription status
Important trends and relationships in the data

These insights can help businesses better understand their customers and make informed decisions.

▶️ How to Run the Project
Step 1 — Clone the Repository
git clone <your-github-repository-url>
Step 2 — Install Required Python Libraries
pip install pandas numpy matplotlib seaborn
Step 3 — Run the Python Notebook

Open the .ipynb file using:

Jupyter Notebook
JupyterLab
Google Colab

Run the notebook from beginning to end to perform data loading, cleaning, and EDA.

Step 4 — Load the Cleaned Dataset into MySQL

Export the cleaned dataset from Python and import it into your MySQL database.

Then execute the SQL queries provided in the SQL folder.

Step 5 — Open the Power BI Dashboard

Open the .pbix file using Microsoft Power BI Desktop.

If required, update the data source connection and refresh the dashboard.

📁 Project Structure
Data-Analytics-Project/
│
├── dataset/
│   └── raw_dataset.csv
│
├── cleaned_data/
│   └── cleaned_dataset.csv
│
├── python/
│   └── data_analysis.ipynb
│
├── sql/
│   └── analysis_queries.sql
│
├── powerbi/
│   └── dashboard.pbix
│
├── images/
│   └── dashboard.png
│
└── README.md
💡 Key Skills Demonstrated

This project demonstrates practical experience in:

Data Cleaning
Exploratory Data Analysis
Python & Pandas
SQL & MySQL
Data Visualization
Power BI Dashboard Development
Business Analysis
Data Storytelling
Extracting Business Insights from Data
👨‍💻 Author

Abhay Lohekar

Data Analytics Enthusiast

Skills: Python | Pandas | SQL | MySQL | Power BI | Data Analysis | Data Visualization
