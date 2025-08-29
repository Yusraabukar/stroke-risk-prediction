Machine learning project exploring stroke risk prediction using logistic regression, developed for UWE Bristol’s Masters Machine Learning and Predictive Analytics Module.

Stroke Risk Prediction Using Machine Learning

A machine learning analysis focused on predicting the risk of stroke using clinical and demographic patient data. The final model, based on logistic regression, achieved a ROC AUC score of 0.839.

Overview

This repository contains coursework submitted for UFCFMJ15M Machine Learning and Predictive Analytics at the University of the West of England (UWE Bristol). The project demonstrates how exploratory data analysis can guide model selection for clinical prediction tasks.

Research Question:
Can we accurately predict stroke risk using patient-level demographic and clinical information, and which algorithm provides the best balance between interpretability and performance?

Key Results

Model comparison: Logistic Regression (0.839 ROC AUC) outperformed Naïve Bayes (0.825), Random Forest (0.821), and Support Vector Machine (0.796).

Dataset: 5,110 patient records with 4.87% positive stroke cases.

Main insight: Stroke patients were on average 25.7 years older than those without stroke.

Potential impact: More than £50 million annual savings per 100,000 patients screened through targeted prevention.

Repository Contents

data/ – Raw and cleaned datasets

notebooks/ – Data preprocessing, analysis, and model comparison experiments (Logistic Regression, SVM, Naïve Bayes, Random Forest)

readme.md – Project overview

<img width="655" height="237" alt="image" src="https://github.com/user-attachments/assets/6dbd2f99-0fee-479c-9d90-263ba10681f3" />

Logistic regression was selected for its strong performance and clear interpretability, which are essential for clinical deployment.

Key Findings
Risk Factors
•	Age: Each additional decade increases the odds of stroke by 2.8 times

•	Heart disease: Increases risk by 3.4 times

•	Hypertension: 2.3 times higher risk

•	High glucose: 1.9 times higher risk

Age Threshold Effect
•	Under 30 years: 0.13 percent stroke rate
•	Over 70 years: 17.75 percent stroke rate (133 times increase)

Clinical Application
•	High risk group (above 15 percent): Up to 25 strokes prevented per 1000 screened

•	Estimated cost of implementation: Less than 150000 pounds

•	Return on investment estimated at ten to one

Coursework Objectives Covered

•	Identifying a real-world healthcare problem suitable for machine learning

•	Analysing dataset properties and feature characteristics

•	Comparing bivariate and multivariate approaches

•	Selecting and evaluating supervised learning algorithms

•	Applying healthcare-appropriate evaluation metrics

•	Justifying the choice of model and rejecting unsuitable alternatives

Limitations

•	Imbalanced dataset affects precision

•	Results are based on a single source of data

•	The dataset is cross sectional and does not allow temporal analysis
