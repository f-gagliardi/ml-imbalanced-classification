Title

Predicting 30-Day Hospital Readmission in Diabetic Patients.

Project Summary

This project investigates the prediction of 30-day hospital readmissions among diabetic patients using structured clinical and hospitalization data. The task is formulated as a binary classification problem, where readmissions within 30 days (represented by class 1) represent approximately 11% of the dataset, resulting in a strongly imbalanced setting.

A key methodological challenge concerns data leakage prevention, as each row corresponds to a hospital encounter rather than a unique patient. To ensure proper generalization assessment, the train-test split was performed at the patient level, preventing overlap of individuals across datasets. Alternative strategies (e.g., selecting only first or last admissions) were evaluated but not adopted in order to preserve data richness while maintaining methodological rigor.

Beyond predictive performance, the project critically examines whether meaningful predictive signal can be extracted from structured clinical variables.

The analysis emphasizes:
Robust methodology
Data leakage prevention
Class imbalance handling
Model comparison
Critical evaluation of model limitations

This project was developed as part of a Artificial Intelligence Methods course and focuses on methodological aspects of supervised learning under class imbalance.

Dataset

Diabetes 130-US Hospitals for Years 1999-2008
Source: UC Irvine Machine Learning Repository

Due to licensing and size constraints, the dataset is not included in this repository.
Download it from: https://archive.ics.uci.edu/dataset/296/diabetes+130-us+hospitals+for+years+1999-2008

Methodology

Preprocessing and exploratory analysis
Prevention of data leakage
Models
Validation strategy and advanced optimization
evaluation metrics
alternative problem reformulations

Results
Model					Precision (Class 1)	Recall (Class 1)	F1-Score (Class 1)	AUC-ROC
Logistic Regression (Balanced)	0.1824	0.5349	0.2720	0.6657
Balanced Random Forest	0.1688	0.6419	0.2673	0.6617
XGBoost (Balanced)	0.1808	0.5044	0.2662	0.6441
Neural Networks	0.1733	0.6218	0.2711	0.6703

