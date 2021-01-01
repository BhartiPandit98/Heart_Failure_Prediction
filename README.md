# Heart Failure Prediction: Project Overview
- I built a tool that predicts the possibilty of heart failure in a person to slow down the disease progression and improve pateint outcomes
- Scraped clinincal and lifestyle data of over 300 persons

# Code and Resources Used
- Python Version: 3.7
- Packages: Pandas, numpy, Sklearn, Matplotlib, seaborn
- Scaper data: https://github.com/BhartiPandit98/Heart_Failure_Prediction/blob/main/heart_failure_clinical_records_dataset.csv

# Dataset Description
- Age
- Anaemia
- Creatinine Phosphokinase
- Diabetes
- Ejection Fraction
- High Blood Pressure
- Platelets
- Serum Sodium
- Sex
- Smoking
- Time
- Death Event

# Data Cleaning
After scraping the data, I needed to clean it up so that it was usable for our model. I made the following changes:
- Converted the different chemical levels to low, medium and high
- Converted the age group as adult and senior citizen

# EDA
I looked at the distributions of the data and the value counts for the various categorical variables. Below are a few highlights:

![alt](https://github.com/BhartiPandit98/Heart_Failure_Prediction/blob/main/Failure%20Stripplot.JPG)

![alt](https://github.com/BhartiPandit98/Heart_Failure_Prediction/blob/main/Heart%20Failure%20Distribution.JPG)

![alt](https://github.com/BhartiPandit98/Heart_Failure_Prediction/blob/main/Serum%20Sodium%20Distribution.JPG)

# Model Building
First, I transformed the categorical variables into dummy variables. I also split the data into train and tests sets with a test size of 20%.

I tried three different models and evaluated them using F1 Score:

- KNN - F1 score = 0.82
- Decision Tree - F1 score = 0.86
- SVM - F1 score = 0.82
- Logistic Regression - F1 score = 0.86
