H1N1 and Seasonal Flu Vaccine Prediction
📌 Project Overview
This project focuses on predicting how likely individuals are to receive H1N1 and Seasonal flu vaccines using machine learning models. The dataset consists of demographic, behavioral, and health-related survey responses from the DrivenData Flu Shot Learning Competition.

The objective is to build robust predictive models that help public health authorities identify groups less likely to be vaccinated and design targeted awareness campaigns.

🎯 Problem Statement
To predict whether an individual is likely to receive the H1N1 vaccine and/or the Seasonal flu vaccine, based on their demographic, behavioral, and health-related characteristics.

📂 Dataset
The dataset comes from the DrivenData Flu Shot Learning Challenge.

training_set_features.csv – 26,707 rows × 36 features

training_set_labels.csv – vaccination labels (h1n1_vaccine, seasonal_vaccine)

test_set_features.csv – 26,708 rows × 36 features

Features include:

Demographics (age group, sex, race, income, marital status, etc.)

Behavioral factors (hand washing, mask usage, social gathering habits, etc.)

Health-related attributes (chronic conditions, insurance, doctor recommendations, etc.)

Opinions on vaccine effectiveness and risks

⚙️ Methodology
1. Data Preprocessing
Missing Value Handling: Used KNN Imputer after encoding categorical variables.

Encoding: Applied Label Encoding for categorical features.

Class Imbalance: Balanced H1N1 vaccine labels using SMOTE oversampling.

2. Exploratory Data Analysis (EDA)
Distribution analysis of vaccine uptake.

Chi-square hypothesis testing to check significance between vaccines and categorical attributes.

3. Models Implemented
Logistic Regression

Decision Tree

Random Forest

Gradient Boosting

Support Vector Machine (SVM)

Naive Bayes

4. Evaluation Metrics
Accuracy

Precision

Recall

F1-score

AUC-ROC (primary metric for model comparison)

📊 Results
Seasonal Vaccine
Best Model: Gradient Boosting (n_estimators=4000)

Accuracy: 85.66%

AUC: 0.93

H1N1 Vaccine
Best Model: Gradient Boosting (n_estimators=700)

Accuracy: 92.02%

AUC: 0.97

Other models like Random Forest and Decision Tree also performed strongly but showed tendencies of overfitting. Logistic Regression and Naive Bayes underperformed compared to ensemble methods.

✅ Conclusion
Gradient Boosting Classifier proved to be the most reliable and robust for both vaccine types.

Ensemble models captured complex patterns better than linear models.

Public health agencies could leverage such models to identify individuals unlikely to get vaccinated and design targeted awareness campaigns.

📦 Tech Stack
Language: Python

Libraries: Pandas, NumPy, Scikit-learn, Imbalanced-learn, Matplotlib, Seaborn

Algorithms: Logistic Regression, Decision Tree, Random Forest, Gradient Boosting, SVM, Naive Bayes