# Flight Disruption Prediction Using Machine Learning at King Khalid International Airport

## Overview
This project focuses on predicting flight disruptions at King Khalid International Airport (KKIA) using supervised machine learning techniques. The objective is to classify flights as either disrupted or non-disrupted based on historical aviation data and operational features.

The project applies a complete machine learning pipeline including data preprocessing, exploratory data analysis (EDA), feature engineering, model training, model evaluation, and stacking ensemble learning.

---

## Problem Statement
Flight disruptions such as delays and cancellations negatively affect passengers, airport operations, and airline efficiency. Early prediction of disruptions can support proactive planning and better operational decision-making.

This project aims to develop an intelligent prediction system capable of identifying potential disruptions using historical flight records.

---

## Dataset
The dataset used in this project is the King Khalid International Airport (KKIA) Flights Dataset obtained from Kaggle.

### Dataset Features
The dataset includes:
- Airline information
- Aircraft type
- Flight category
- Route details
- Flight status
- Scheduling timestamps
- Airport information

A binary target variable named `isDisrupted` was created using the flight status feature.

---

## Machine Learning Pipeline

### Data Preprocessing
- Handling missing values
- Encoding categorical variables
- Removing unnecessary columns

### Exploratory Data Analysis (EDA)
- Flight status distribution
- Disruption trends
- Time-based analysis
- Feature relationship visualization

### Feature Engineering
- Creating `isDisrupted`
- Extracting hour/day/month features
- Building time-based features

### Models Used

#### Base Learners
- Logistic Regression
- Random Forest
- XGBoost
- CatBoost

#### Meta Learners (Stacking)
- Logistic Regression
- Random Forest

---

## Evaluation Metrics
The models were evaluated using:
- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC

Since the dataset is highly imbalanced, recall and F1-score were considered the most important evaluation metrics.

---

## Results
The stacking approach achieved the best overall performance compared to individual base learners.

### Key Observations
- Logistic Regression achieved high recall but low precision.
- Random Forest and XGBoost produced more stable predictions.
- The stacking model improved overall disruption detection performance.

---

## Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- CatBoost
- Matplotlib
- Seaborn

---

## Future Improvements
- Integrating real-time flight data
- Improving imbalance handling
- Deploying the model as a web application

---

## Team Members
- Khayal Al-Nomis
- Aleen Alzahrani
- Haya Alwuhaibi
- Ruqayah Almousa
- Shahad Alshahrani
- Najaf Almohsen
- 
---

## License
This project is developed for academic purposes.
