# Global Tech Salary Analysis (2020-2024) 📊

## 📋 Project Overview
Understanding salary trends is crucial in the evolving data science field. This project analyzes Data Science salaries from 2020 to 2024 to provide insights into regional variations and compensation factors.

## 🛠️ Tech Stack
- *Tool:* Power BI Desktop
- *Language:* DAX (Data Analysis Expressions)
- *Data Source:* Kaggle (Data Science Salaries)

## 📂 Dataset Structure
The dataset includes the following key features:
- job_title: The specific role (e.g., Data Engineer).
- experience_level: EN (Entry), MI (Mid), SE (Senior), EX (Executive).
- salary_in_usd: Standardized salary for global comparison.
- remote_ratio: Work model (Remote, Hybrid, On-site).

## 💡 Key Insights & DAX Formulas
I created custom measures to drive dynamic insights:
- *Average Salary:* AVERAGE('data_science_salaries'[salary_in_usd])
- *Salary Growth Logic:* Used conditional formatting to highlight YoY trends.

- Total Jobs = COUNTROWS('data_science_salaries')
Median Salary USD = MEDIAN('data_science_salaries'[salary_in_usd])
Median Salary USD = MEDIAN('data_science_salaries'[salary_in_usd])
Status Color = IF([Salary Growth %] > 0, "#00FF00", "#FF0000")
