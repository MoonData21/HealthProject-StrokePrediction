# HealthProject-StrokePrediction

Stroke Prediction Using Machine Learning

This project explores the development of machine learning models to predict stroke risk using a small set of key health and lifestyle indicators. The dataset was preprocessed, resampled for balance, and evaluated using Stratified K-Fold Cross-Validation to ensure fair model comparison.

Feature Overview
Feature	Type / Range	Explanation
hypertension	Binary (0 or 1)	0 → No, 1 → Yes
heart_disease	Binary (0 or 1)	0 → No, 1 → Yes
avg_glucose_level	Continuous (56.11 – 271.74)	Average blood glucose level measured for the patient
bmi	Continuous (16.4 – 60.2)	Body Mass Index of the patient
gender	Categorical (0–2)	0 → Female, 1 → Male, 2 → Other
ever_married	Binary (0 or 1)	0 → No, 1 → Yes
work_type	Categorical (0–4)	0 → Govt_job, 1 → Never_worked, 2 → Private, 3 → Self-employed, 4 → Children
Residence_type	Binary (0 or 1)	0 → Rural, 1 → Urban
smoking_status	Categorical (0–3)	0 → Unknown, 1 → Formerly smoked, 2 → Never smoked, 3 → Smokes
Model Evaluation

Two machine learning models were trained and evaluated:

Random Forest Classifier

XGBoost Classifier

Each model was assessed across five cross-validation folds, measuring accuracy, ROC-AUC, and F1 score.

Cross-Validated Performance Summary
Model	Mean Accuracy	Mean ROC-AUC	Mean F1 Score
Random Forest	0.782 ± 0.003	0.858 ± 0.006	–
XGBoost	0.919 ± 0.004	0.971 ± 0.003	0.925 ± 0.004

Interpretation:
The XGBoost model demonstrates superior classification ability, achieving higher accuracy, better discrimination (ROC-AUC), and stronger balance between precision and recall (F1-score).
