# Salifort Motors Employee Attrition Prediction

## Overview
This project was completed as the capstone for the **Google Advanced Data Analytics Certificate**. The objective was to analyze employee survey data from Salifort Motors and build a predictive model to identify employees at risk of leaving the company.

The project combines **data cleaning, exploratory data analysis (EDA), classification modeling, model evaluation, and business recommendations** to support HR decision-making and improve employee retention.

## Business Problem
Salifort Motors is experiencing a high rate of employee turnover. Replacing employees is costly and time-consuming due to recruiting, onboarding, and training expenses.

The goal of this project is to:
- predict whether an employee is likely to leave the company
- identify the main factors associated with turnover
- provide actionable recommendations to improve retention

## Dataset
The dataset contains employee-level survey information, including:
- satisfaction level
- last evaluation
- number of projects
- average monthly hours
- time spent at company
- work accident
- promotion in the last 5 years
- department
- salary
- employee attrition (`left`)

### Data cleaning
- Removed **3,008 duplicate rows**
- Final dataset used for modeling: **11,991 unique employee records**
- Renamed columns for consistency and readability
- Checked for missing values and outliers

## Tools and Libraries
- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **scikit-learn**

## Project Workflow
1. **Data loading and inspection**
2. **Data cleaning**
3. **Exploratory data analysis**
4. **Feature encoding**
5. **Train/test split**
6. **Model building**
   - Decision Tree
   - Random Forest
7. **Model evaluation**
8. **Business interpretation and recommendations**

## Exploratory Data Analysis
EDA showed that employee turnover was associated with:
- lower satisfaction levels
- higher number of projects
- longer average monthly working hours
- longer time at the company
- lower salary levels

Turnover was also observed across multiple departments, with larger counts in departments such as sales, technical, and support.

## Models Built

### 1. Decision Tree
Performance on the test set:
- **Accuracy:** 0.9670
- **Precision:** 0.8859
- **Recall:** 0.9197
- **F1-score:** 0.9025
- **ROC-AUC:** 0.9480

### 2. Random Forest
Performance on the test set:
- **Accuracy:** 0.9857
- **Precision:** 0.9914
- **Recall:** 0.9217
- **F1-score:** 0.9553
- **ROC-AUC:** 0.9785

## Best Model
The **Random Forest** model performed better overall and was selected as the final model.

## Most Important Features
The top predictors of employee attrition were:
1. **satisfaction_level**
2. **number_project**
3. **time_spend_company**
4. **average_monthly_hours**
5. **last_evaluation**

These results suggest that employee turnover is mainly driven by **low satisfaction, heavy workload, and tenure-related factors**.

## Key Insights
- Employees who left the company tended to report **lower satisfaction**
- Employees who left often had **more projects** and **worked longer hours**
- Employees with **low and medium salary levels** showed higher turnover
- Promotion appears to be associated with **lower attrition**
- Workload and employee experience are strongly linked to retention

## Business Recommendations
Based on the analysis, Salifort Motors should consider:
- reviewing workload distribution across teams
- monitoring employees with high project counts and long monthly hours
- improving employee satisfaction tracking and follow-up
- strengthening career development and promotion pathways
- targeting retention efforts toward employees showing signs of disengagement or overwork

## Repository Contents
- `Salifort_Employee_Attrition_Prediction.ipynb` → complete notebook with code, outputs, and interpretation
- `HR_capstone_dataset.csv` → dataset used in the analysis

## Conclusion
This project demonstrates how machine learning can support HR analytics by identifying employees at risk of leaving and revealing the factors most strongly associated with turnover. The final Random Forest model provided strong predictive performance and generated actionable business insights that can help improve employee retention.

## Author
**Francis Cebrián Ruiz**
