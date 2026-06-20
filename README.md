Credit Risk Assessment - Exploratory Data Analysis (EDA)
📌 Project Overview

This project focuses on performing Exploratory Data Analysis (EDA) on a Credit Risk dataset to identify key factors influencing loan approval decisions and borrower risk profiles.

The analysis examines borrower demographics, financial background, loan characteristics, and credit history to uncover meaningful patterns and trends that help understand creditworthiness and lending risks.

🎯 Problem Statement

Financial institutions face significant challenges in assessing borrower credit risk and minimizing loan defaults.

The objective of this project is to analyze borrower behavior, loan attributes, and credit history through EDA techniques to identify factors that impact loan approval and credit risk.

🎯 Objectives
Analyze borrower demographic profiles
Identify important credit risk indicators
Study relationships between income and loan characteristics
Understand factors affecting loan approval
Discover patterns in borrower credit behavior
Generate insights for risk management and lending decisions
💼 Business Use Cases
Loan approval decision support
Borrower risk assessment
Creditworthiness evaluation
Default risk identification
Financial loss reduction
Better lending strategy formulation
📊 Dataset Information
Dataset Details
Feature	Description
Records	32,581
Columns	12
Type	Structured CSV
Domain	Finance / Credit Risk
Key Features
person_age
person_income
person_home_ownership
person_emp_length
loan_intent
loan_grade
loan_amnt
loan_int_rate
loan_percent_income
cb_person_default_on_file
cb_person_cred_hist_length
loan_status
🛠 Technologies Used
Python
NumPy
Pandas
Matplotlib
Seaborn
Jupyter Notebook
🔍 EDA Process
1. Data Understanding
Loaded dataset
Examined dataset structure
Checked data types
Reviewed statistical summary
2. Data Cleaning
Handled missing values
Removed duplicate records
Treated unrealistic age outliers
Verified data consistency
3. Missing Value Treatment
Column	Missing Values
person_emp_length	895
loan_int_rate	3116

Median imputation was used because these features contained outliers and skewed distributions.

4. Duplicate Removal
165 duplicate records identified
Duplicates removed to prevent biased analysis
5. Outlier Treatment

Applied IQR method on:

person_age

Outliers in financial variables such as:

person_income
loan_amnt
loan_int_rate

were retained because they represent genuine borrower behavior.

📈 Univariate Analysis
Visualizations Used
Histogram (Age Distribution)
Histogram (Income Distribution)
Count Plot (Loan Status)
Count Plot (Home Ownership)
Count Plot (Loan Intent)
Key Findings
Majority of borrowers are aged 20–30 years.
Income distribution is highly right-skewed.
Most applicants earn below ₹2,00,000 annually.
Approximately 78% of loans are approved.
RENT and MORTGAGE categories dominate home ownership.
📊 Bivariate Analysis
Visualizations Used
Scatter Plot: Income vs Loan Amount
Loan Grade vs Loan Status
Home Ownership vs Loan Status
Loan Intent vs Loan Status
Key Findings
Higher-income borrowers tend to request larger loans.
Loan grade strongly influences approval decisions.
Renters show relatively higher rejection rates.
Certain loan purposes exhibit different approval patterns.
📉 Multivariate Analysis
Visualizations Used
Pair Plot
Correlation Heatmap
Multi-dimensional Scatter Plot
Key Findings
Higher interest rates are associated with non-approved loans.
Loan-to-income ratio significantly impacts approval outcomes.
Age and credit history length show strong correlation.
Lower loan grades generally indicate higher risk borrowers.
🔥 Important Insights

✅ Younger borrowers form the majority of applicants.

✅ Loan approval is highly influenced by loan grade.

✅ Higher loan-to-income ratios increase credit risk.

✅ Interest rate is a strong indicator of borrower risk.

✅ Home ownership status contributes to approval likelihood.

✅ Credit history length positively impacts creditworthiness.

📷 Sample Visualizations
Age Distribution
Income Distribution
Loan Status Distribution
Income vs Loan Amount
Loan Grade vs Loan Status
Correlation Heatmap
Pair Plot
📁 Project Structure
Credit-Risk-EDA/
│
├── credit_risk_dataset.csv
├── Credit_Risk_Analysis.ipynb
├── Credit_Risk_Analysis_Presentation.pptx
├── README.md
│
└── images/
    ├── age_distribution.png
    ├── income_distribution.png
    ├── loan_status.png
    ├── heatmap.png
    └── pairplot.png
🚀 How to Run
Clone Repository
git clone https://github.com/yourusername/credit-risk-eda.git
Install Required Libraries
pip install pandas numpy matplotlib seaborn jupyter
Launch Notebook
jupyter notebook

Open:

Credit_Risk_Analysis.ipynb
📌 Conclusion

This EDA project successfully identified the major factors influencing credit risk and loan approval decisions. Analysis revealed that loan grade, interest rate, income, credit history length, and loan-to-income ratio are among the most influential variables affecting borrower risk.

The insights obtained can help financial institutions improve risk assessment, optimize lending strategies, and reduce potential loan defaults.
