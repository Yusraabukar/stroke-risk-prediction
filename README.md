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

Logistic regression was selected as the final model due to its strong predictive performance (ROC AUC = 0.839) and transparent coefficient structure, making it suitable for clinical deployment. Alternative models (Naïve Bayes, Random Forest, and SVM) were tested but rejected due to weaker performance or limited interpretability.

Key Findings

Risk Factors

Age: Each decade increases stroke odds by ~2.8×

Heart disease: Increases risk by ~3.4×

Hypertension: Raises risk by ~2.3×

High glucose (>126 mg/dL): Raises risk by ~1.9×

Age Threshold Effect

Under 30 years: 0.13% stroke rate

Over 70 years: 17.75% stroke rate (≈133× increase)

Clinical Application

High-risk group (>15% probability): Up to 25 strokes prevented per 1,000 screened

Implementation cost: <£150,000

ROI: Estimated at 10:1, reflecting ~£50–75 million annual savings per 100,000 patients screened

Coursework Objectives Covered

Identified a real-world healthcare problem suitable for machine learning

Analysed dataset properties and feature characteristics

Compared bivariate and multivariate analytical strategies

Selected and evaluated multiple supervised learning algorithms

Applied healthcare-appropriate evaluation metrics (ROC-AUC, sensitivity, specificity, PR-AUC)

Justified model choice and rejected unsuitable alternatives

Limitations

Severe class imbalance (4.87% stroke cases) affects precision performance

Results are based on a single dataset source

Cross-sectional design prevents temporal or longitudinal validation


