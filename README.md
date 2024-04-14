# Employee Turnover Prediction

## Overview

This project aims to predict employee turnover and identify key factors contributing to employee attrition using machine learning techniques. By analyzing employee data, we aim to assist HR departments in identifying potential leavers and developing strategies to improve employee retention.

## Dataset

The dataset contains the following columns:

| Variable                | Meaning                                               |
|-------------------------|-------------------------------------------------------|
| Age                     | Age of the employee                                   |
| Attrition               | Whether the employee left in the previous year or not |
| BusinessTravel          | How frequently the employees traveled for business purposes in the last year |
| Department              | Department in company                                 |
| DistanceFromHome        | Distance from home in kms                             |
| Education               | Education Level (1:'Below College', 2:'College', 3:'Bachelor', 4:'Master'. 5:'Doctor) |
| EducationField          | Field of education                                    |
| EmployeeCount           | Employee count                                        |
| EmployeeNumber          | Employee number/id                                    |
| EnvironmentSatisfaction | Work Environment Satisfaction Level (1:lowest, 4:highest) |
| Gender                  | Gender of employee                                    |
| JobInvolvement          | Job Involvement Level (1:lowest, 4:highest)           |
| JobLevel                | Job level at company on a scale of 1 to 5             |
| JobRole                 | Name of job role in company                           |
| JobSatisfaction         | Job Satisfaction Level (1:lowest, 4:highest)          |
| MaritalStatus           | Marital status of the employee                        |
| MonthlyIncome           | Monthly income in Indian Rupees per month             |
| NumCompaniesWorked      | Total number of companies the employee has worked for |
| Over18                  | Whether the employee is above 18 years of age or not  |
| PercentSalaryHike       | Percent salary hike for last year                     |
| PerformanceRating       | Performance rating for last year (1:lowest, 4:highest) |
| RelationshipSatisfaction| Relationship satisfaction level                       |
| StandardHours           | Standard hours of work for the employee               |
| StockOptionLevel        | Stock option level of the employee                    |
| TotalWorkingYears       | Total number of years the employee has worked so far  |
| TrainingTimesLastYear   | Number of times training was conducted for this employee last year |
| WorkLifeBalance         | Work life balance level (1:lowest, 4:highest)         |
| YearsAtCompany          | Total number of years spent at the company by the employee |
| YearsSinceLastPromotion | Number of years since last promotion                  |
| YearsWithCurrManager    | Number of years under current manager                 |

## Methodology

1. **Data Cleaning:** Removed unnecessary columns and filled missing values with the mean for numeric columns.
2. **Exploratory Data Analysis (EDA):** Conducted EDA to understand the distribution and correlation of variables with employee attrition.
3. **Data Transformation:** Applied dummy encoding, standardization, dataset splitting, and used SMOTE for addressing class imbalance.
4. **Modeling:** Utilized logistic regression for predicting employee turnover. Focused on optimizing the model to improve recall to minimize Type II errors.
5. **Evaluation:** Compared model coefficients and evaluated model performance using metrics such as accuracy, recall, precision, and the ROC-AUC curve.

## Results

Our model identifies several key factors that are highly correlated with employee attrition, ranked by their impact:

1. Educational level with doctor
2. Single
3. Belongs to sales department
4. Belongs to R&D department
5. Low Work Life Balance

The logistic regression model, optimized for recall, showed promising results in predicting employee turnover, with a detailed analysis of the coefficients to understand the impact of various factors.

## Potential Improvements

- **Causal Inference:** Future work could explore causal inference methods to understand the causality between identified factors and employee turnover. This approach would help in distinguishing correlation from causation, providing more actionable insights for HR strategies.
- **Model Exploration:** Experimenting with other classification algorithms and advanced techniques like ensemble methods could yield better predictive performance.

## Usage

To replicate this analysis, ensure your Python environment matches the versions used in this project:

1. Check the notebook's top section for the Python and library versions (`numpy`, `pandas`, `matplotlib`, `seaborn`, `imblearn`, `sklearn`).
2. Set up your environment to match these versions to avoid compatibility issues.
3. Install required libraries with `pip install library==version`, adjusting for the correct library names and versions.
4. Follow the Jupyter notebook step-by-step for the complete analysis.

## Contributions

This repository is read-only and serves as a showcase of my learning milestones in data science.
