# 📊 Credit Risk Assessment - Exploratory Data Analysis (EDA)

## 🔹 Project Overview

Credit risk assessment is a critical process for financial institutions to evaluate the likelihood of borrowers defaulting on their loans. This project performs Exploratory Data Analysis (EDA) on a Credit Risk dataset to uncover patterns, trends, and key factors influencing loan approval decisions and borrower risk profiles.

The analysis focuses on demographic information, financial status, employment history, loan characteristics, and credit history to generate actionable insights that support better lending decisions.

---

## 🎯 Problem Statement

Banks and lending institutions face significant challenges in identifying high-risk borrowers and minimizing loan defaults. The objective of this project is to analyze borrower and loan-related attributes to understand the factors affecting loan approval and credit risk through data visualization and statistical analysis.

---

## 🎯 Objectives

- Analyze borrower demographics and financial profiles.
- Identify key factors affecting loan approval.
- Examine relationships between income, loan amount, and interest rates.
- Understand patterns associated with borrower risk.
- Generate insights to support credit risk assessment.
- Improve decision-making for lending institutions.

---

## 📂 Dataset Information

### Dataset Summary

| Attribute | Value |
|------------|--------|
| Total Records | 32,581 |
| Total Features | 12 |
| Domain | Finance |
| Dataset Type | Structured CSV |

### Features

- person_age
- person_income
- person_home_ownership
- person_emp_length
- loan_intent
- loan_grade
- loan_amnt
- loan_int_rate
- loan_percent_income
- cb_person_default_on_file
- cb_person_cred_hist_length
- loan_status

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## 🔍 Data Cleaning Process

### Missing Value Handling

| Column | Missing Values |
|----------|---------------|
| person_emp_length | 895 |
| loan_int_rate | 3116 |

Missing values were treated using **Median Imputation** because the distributions contained outliers and were skewed.

### Duplicate Removal

- Identified 165 duplicate records.
- Removed duplicates to ensure accurate analysis.

### Outlier Treatment

Outliers were detected using the **IQR Method**.

Removed outliers from:
- person_age

Retained outliers in:
- person_income
- loan_amnt
- loan_int_rate

These values were considered valid financial observations rather than errors.

---

## 📈 Exploratory Data Analysis

### Univariate Analysis

Visualizations Used:

- Histogram
- Count Plot
- Distribution Plot

Key Findings:

- Most borrowers belong to the 20–30 age group.
- Income distribution is highly right-skewed.
- Majority of applicants earn below ₹200,000 annually.
- Loan approval rate is significantly higher than rejection rate.
- RENT and MORTGAGE are the most common home ownership categories.

---

### Bivariate Analysis

Visualizations Used:

- Scatter Plot
- Grouped Count Plot
- Comparative Bar Charts

Key Findings:

- Higher-income individuals tend to request larger loans.
- Loan grade strongly impacts approval status.
- Renters have a relatively higher rejection rate.
- Loan purpose influences approval outcomes.

---

### Multivariate Analysis

Visualizations Used:

- Pair Plot
- Correlation Heatmap
- Multi-dimensional Scatter Plot

Key Findings:

- Higher interest rates are associated with increased credit risk.
- Loan-to-income ratio significantly affects approval decisions.
- Age and credit history length show a positive relationship.
- Lower loan grades correspond to riskier borrower profiles.

---

## 📊 Key Insights

✅ Majority of borrowers are young adults.

✅ Income alone does not determine loan approval.

✅ Loan grade is a strong indicator of creditworthiness.

✅ Higher interest rates are associated with higher-risk borrowers.

✅ Home ownership status influences loan approval trends.

✅ Credit history length positively contributes to borrower reliability.

---

## 💼 Business Impact

The insights generated from this analysis can help:

- Improve loan approval processes.
- Identify high-risk borrowers early.
- Reduce default rates.
- Enhance credit risk management.
- Support data-driven lending strategies.

---

## 📁 Project Structure

```bash
Credit-Risk-Assessment-EDA/
│
├── credit_risk_dataset.csv
├── Credit_Risk_Analysis.ipynb
├── Credit_Risk_Analysis_Presentation.pptx
├── README.md
│
└── images/
    ├── age_distribution.png
    ├── income_distribution.png
    ├── loan_status_distribution.png
    ├── correlation_heatmap.png
    └── pairplot.png
```

---

## 🚀 How to Run the Project

### Clone Repository

```bash
git clone https://github.com/Mohit242004/Credit-Risk-Assessment-EDA.git
```

### Install Dependencies

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### Launch Jupyter Notebook

```bash
jupyter notebook
```

Open:

```bash
Credit_Risk_Analysis.ipynb
```

---

## 📌 Conclusion

The Credit Risk Assessment EDA project successfully identified the major factors influencing borrower risk and loan approval outcomes. Loan grade, interest rate, loan-to-income ratio, income level, and credit history emerged as significant indicators of creditworthiness.

These insights can assist financial institutions in making informed lending decisions, minimizing default risk, and improving overall risk management strategies.

---

## 👨‍💻 Author

### Mohit Chaudhari

🎓 B.Tech (Computer Science & Engineering)

📊 Aspiring Data Analyst | Data Science Enthusiast

🔗 LinkedIn: https://www.linkedin.com/in/mohit-chaudhari-028301259

🔗 GitHub: https://github.com/Mohit242004

---

⭐ If you found this project useful, don't forget to Star the repository.
