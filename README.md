# EasyVisa-Predicting-Visa-Approvals-with-Machine-Learning


## Project Overview

The **EasyVisa Project** aims to facilitate the visa approval process by building machine learning models that predict the likelihood of visa certification. The goal is to assist the Office of Foreign Labor Certification (OFLC) in making informed decisions by analyzing key factors influencing visa applications.

## Business Problem

The **Immigration and Nationality Act (INA)** allows foreign workers to enter the U.S. for employment. The increasing number of visa applications has made manual processing challenging. This project proposes a machine learning solution to predict whether a visa will be **certified** or **denied** based on applicant and job characteristics.

## Solution Approach

- Perform **Exploratory Data Analysis (EDA)** to identify insights and patterns.
- Preprocess data to handle missing values, outliers, and categorical variables.
- Build multiple classification models and apply hyperparameter tuning.
- Evaluate models using metrics like **F1 Score**, **Accuracy**, and **Recall**.

## Dataset Overview

- **Data Source**: Provided dataset containing information about visa applicants and employers.
- **Features Include**:
  - Education Level
  - Job Experience
  - Prevailing Wage
  - Wage Unit
  - Continent of Origin
  - Region of Employment
- **Target Variable**: Visa Status (Certified or Denied)

## EDA Highlights

- Applicants with **higher education** (Master’s or Doctorate) have a higher chance of visa certification.
- Visa applications from **Asia** and **Europe** are certified more often than those from other continents.
- **Annual wage units** are more commonly associated with successful visa applications.
- **Job experience** significantly influences certification outcomes.

## Models Used

- **Decision Tree Classifier**
- **Random Forest Classifier**
- **Bagging Classifier**
- **AdaBoost Classifier**
- **Gradient Boosting Classifier**
- **XGBoost Classifier**
- **Stacking Classifier**

## Model Evaluation

- The **Tuned Gradient Boosting Classifier** showed the best results with balanced recall and precision.
- **F1 Score** was used as the primary metric to reduce both **false positives** and **false negatives**.

| Model                     | Train F1 Score | Test F1 Score |
|----------------------------|----------------|---------------|
| Decision Tree              | 0.81           | 0.81          |
| Tuned Gradient Boosting    | 0.83           | 0.82          |
| XGBoost (Tuned)            | 0.83           | 0.82          |
| Stacking Classifier        | 0.83           | 0.81          |

## Recommendations

- **OFLC** can use the **Tuned Gradient Boosting Classifier** for effective decision-making.
- Emphasize **education level**, **job experience**, and **prevailing wage** when evaluating applications.
- Prioritize applications with a higher likelihood of approval to ensure workforce availability in critical sectors.
