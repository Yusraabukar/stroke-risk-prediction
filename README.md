# stroke-risk-prediction
Machine learning project exploring stroke risk prediction using logistic regression, developed for UWE Bristol’s Masters Machine Learning and Predictive Analytics Module.

Stroke Risk Prediction Using Machine Learning
A machine learning analysis focused on predicting the risk of stroke using clinical and demographic patient data. The final model, based on logistic regression, achieved a ROC AUC score of 0.839.
Overview
This repository contains coursework submitted for UFCFMJ15M Machine Learning and Predictive Analytics at the University of the West of England (UWE Bristol). The project demonstrates how exploratory data analysis can guide model selection for clinical prediction tasks.
Research Question
Can we accurately predict stroke risk using patient-level demographic and clinical information, and which algorithm provides the best balance between interpretability and performance?

Key Results
Model performance: ROC AUC of 0.839 using logistic regression
Dataset: 5110 patient records with 4.87 percent positive stroke cases
Main insight: Stroke patients were on average 25.7 years older than those without stroke
Potential impact: More than 50 million pounds in annual savings per 100000 patients screened

Repository Contents
stroke prediction ml
docs	Project report and figures
data	Raw and cleaned datasets
src	Data processing and model scripts
notebooks  	Jupyter notebooks for analysis
results  	Model outputs and metrics
requirements.txt               	Python dependencies


Installation
git clone https://github.com/[your username]/stroke prediction ml.git
cd stroke prediction ml
pip install -r requirements.txt


Methodology
Dataset Details

•	5110 patient records with 12 clinical and demographic features
•	4.87 percent stroke prevalence
•	3.9 percent missing BMI values addressed with median imputation

Analytical Strategy

Multivariate analysis was chosen over bivariate for better performance:
•	Full model AUC: 0.839
•	Age-only model AUC: 0.834
•	For example, a 68 year old patient had a predicted stroke risk of 12 percent using age alone, which increased to 28 percent when hypertension was included

Model Comparison
Algorithm	ROC AUC	Clinical Suitability	Notes
Logistic Regression	0.839	Suitable	Selected due to transparency
Random Forest	0.821	Less suitable	Complexity of ensemble methods
Support Vector Machine	0.796	Not suitable	Limited interpretability

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
