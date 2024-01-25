# Cognitive decline  predictor using Meta-Learning Algorithms: Project Overview

Empowering early dementia detection through personalized AI analysis of MRI scans and medical data.

* Maximized dementia prediction accuracy with Bagging, Stacking, and Boosting techniques.
* Tripled detection power: Random Forest bagging, stacked Decision Trees-Naive Bayes-KNN, and XGBoost boosting.
* Boosted prediction performance with ensembles: Bagging, Stacking, and XGBoost.

* Performed various Data Preprocessing techniques such as missing data imputation and removal of multicolinear features to clean and make the data ready for model building

* **Tuned hyperparameters** of the model to achieve best performance.

* Boosting had an accuracy of 86.76%, f1-score of 83.64% and recall of 85.19%

* Model was deployed on a web application built using **Django** available at [Dementia Predictor](https://dementia-predictor.onrender.com/)
___
## Model Performamce
Accuracy, F1-Score and Recall were the metrics used to evaluate the performance of the model

| Method    |  Accuracy (%)  | F1-Score (%) | Recall (%) |
|-----------|---------|-----------|---------|
| Bagging | 85.29   | 82.14 | 85.19 |
| Stacking | 85.29   | 80.77 | 77.78 |
| **Boosting**   | **86.76**   | **83.64** | **85.19** |

Confusion Matrix
|   | 0  | 1  |
|---|----|----|
| 0 | TN | FP |
| 1 | FN | TP |
___
![Web application of the model](plots/cf.png)
___
## Features

|Variable	|Data Object	|Data type|
| ----| ---|----|
|MR Delay	|The number of days between visits by a patient.	|Integer
|Gender|	Gender of a patient (M or F)	|Object
|Hand	|Patient’s dominant hand 	|Object
|Age	|Patient's age at the time of data collection	|Integer
|EDUC	|Years of Education	|Integer
|SES 	|Socioeconomic status is classified into categories from 1 (highest status) to 5 (lowest status)	|Integer
|MMSE	|Mini-mental State Examination score (range is from 0-worst to 30-best)	|Integer
|eTIV	|Estimated total intracranial volume (cm3)	|Integer
|nWBV	|Normalized whole brain volume 	|Float


___
## Model Deployment
The final model with the best score was deployed on a web application built with **Django** with the frontend built with **HTML & CSS** with **Boostrap 4** as the CSS Framework.

![Web application of the model](plots/app.png)
___ 
