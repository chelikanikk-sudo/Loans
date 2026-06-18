
## Loans
Loan Analysis Dashboard - Power BI Project

Project Overview

The Loan Default Analysis Dashboard is an interactive Power BI report designed to analyze borrower behavior, identify loan default trends, and evaluate financial risk factors. The dashboard helps financial institutions and lending organizations make data-driven decisions by monitoring applicant demographics, loan performance, and default risk indicators.

Problem Statement

Financial institutions face significant challenges in identifying borrowers who are likely to default on their loans. Traditional reporting methods often fail to provide timely insights into customer profiles, financial conditions, and risk patterns.

This project aims to:

Analyze borrower demographics and financial characteristics.

Identify key factors contributing to loan defaults.

Monitor loan performance trends.

Support risk assessment and lending decisions.

Improve portfolio management and reduce financial losses.

🛠 Tools & Technologies Used

Tool	Purpose

Power BI Desktop	Data Modeling & Visualization

SQL	Data Extraction & Data Preparation

DAX	KPI and Measure Calculations

Excel/CSV Dataset	Source Data

Power Query	Data Cleaning & Transformation


📂 Dataset Information

The dataset contains loan applicant and financial information, including:

Applicant Demographics

Income Details

Employment Information

Credit History

Loan Amount

Loan Status

Default Indicators

Financial Risk Metrics

Data Preparation Steps

Step 1: Data Collection

Imported loan applicant dataset into Power BI Desktop.

Step 2: Data Cleaning

Removed duplicate records.

Handled missing values.

Standardized column formats.

Corrected data types.

Step 3: Data Transformation

Created calculated columns.

Performed data aggregation.

Applied business rules for risk categorization.

Step 4: Data Modeling

Established relationships between tables.

Optimized model for reporting performance.

Step 5: Visualization

Developed interactive dashboard pages.

Added filters and slicers for user analysis.

🗄 SQL Operations Performed

Joined multiple tables using SQL.

Filtered invalid records.

Cleaned and transformed data.

Prepared reporting-ready datasets.


Example:

SELECT *

FROM Applicants A

INNER JOIN Loans L

ON A.Applicant_ID = L.Applicant_ID;

📐 DAX Measures Used

Total Applications
Total Applications = COUNT(Applicants[Applicant_ID])

Total Loan Amount
Total Loan Amount = SUM(Loans[Loan_Amount])

Average Loan Amount
Average Loan Amount =
AVERAGE(Loans[Loan_Amount])

Default Count

Default Count =
CALCULATE(
    COUNT(Loans[Loan_ID]),
    Loans[Loan_Status] = "Default"
)
Default Rate %
Default Rate % =
DIVIDE(
    [Default Count],
    [Total Applications],
    0
)

Average Income

Average Income =
AVERAGE(Applicants[Income])

📊 Dashboard Pages

Page 1: Loan Default Overview

Visuals Used

KPI Cards

Trend Analysis Charts

Loan Default Trends

Risk Monitoring Charts

Slicers and Filters

Purpose

Provides a high-level overview of loan performance and default behavior.

Page 2: Applicant Demographic & Financial Profile

Visuals Used

Donut Chart

Line Charts

Clustered Column Chart

Demographic Analysis

Purpose

Analyzes borrower characteristics such as:

Income Distribution

Employment Status

Applicant Categories

Financial Profiles

Page 3: Financial Risk Metrics

Visuals Used

Line Charts

Ribbon Chart

Decomposition Tree

Purpose

Identifies major risk drivers and evaluates factors influencing loan default probability.

📸 Report Snapshots

Dashboard Overview

<img width="1318" height="742" alt="Image" src="https://github.com/user-attachments/assets/43f79cc4-3ce2-4c5d-91f4-92b27269d518" />


Applicant Demographic Analysis

<img width="1321" height="742" alt="Image" src="https://github.com/user-attachments/assets/837ddb3b-9a02-4127-9b06-d6965c16b851" />


Financial Risk Metrics

<img width="1321" height="745" alt="Image" src="https://github.com/user-attachments/assets/aa104078-d505-446a-8dce-d1e9aeca4d3e" />


🔍 Key Insights

Certain applicant segments exhibit higher default rates.

Income level significantly impacts repayment capability.

Loan amount and repayment history influence default probability.

Risk patterns can be identified through demographic segmentation.

Financial risk metrics assist in proactive lending decisions.

💼 Business Benefits

For Lending Institutions

Reduced loan default risk.

Improved credit assessment.

Better customer segmentation.

Enhanced portfolio monitoring.

Faster decision-making process.

For Management

Real-time visibility into loan performance.

Improved strategic planning.

Data-driven risk management.

🚀 Future Enhancements

Predictive Loan Default Modeling using Machine Learning.

Integration with Real-Time Banking Systems.

AI-Based Risk Scoring.

Customer Churn Analysis.

Credit Score Forecasting.

Automated Alert System for High-Risk Borrowers.

📈 Project Outcomes

Developed an end-to-end Power BI reporting solution.

Transformed raw loan data into actionable insights.

Improved risk visibility and reporting efficiency.

Demonstrated advanced Power BI visualization techniques.

👨‍💻 Author

Kamal Kishore

M.Sc,
M.Phil,
M.Tech,
Data Analyst
Skills:
Power BI |
SQL | 
Excel | 
Python | 
Data Visualization | 
Data Analysis 

⭐ Project Highlights

✔ Data Cleaning & Transformation

✔ SQL Data Preparation

✔ DAX Measures & KPIs

✔ Interactive Power BI Dashboard

✔ Loan Risk Analysis

✔ Financial Performance Monitoring

✔ Business Intelligence Reporting
