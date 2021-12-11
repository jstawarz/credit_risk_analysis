# Credit Risk Analysis

## Overview of Analysis

In this analysis, we are working with Jill, a data scientist at Lending Club. Fast Lending, wants to use machine learning to predict credit risk.
They believe that by implementing machine learning, they will be able to provide a quicker and more reliable loan experience. The company also hopes
that the machine learning algorithms built will more accurately predict good candidates for loans, and ultimately lead to lower default rates.

### Purpose

The purpose of this project will be to build several machine learning algorithms to evaluate credit card risk. Once developed, we will evaluate
the performance of the models to determine if they should be used to predict credit card risk.

## Results

### Random Oversampling

- Accuracy Score: 67.2%
- Precision High Risk: 1%
- Precision Low Risk: 100%
- Recall High Risk: 66%
- Recall Low Risk: 68%

![This is an image](https://github.com/jstawarz/credit_risk_analysis/blob/main/resources/oversampling.png)

### SMOTE

- Accuracy Score: 66.7%
- Precision High Risk: 1%
- Precision Low Risk: 100%
- Recall High Risk: 72%
- Recall Low Risk: 62%

![This is an image](https://github.com/jstawarz/credit_risk_analysis/blob/main/resources/smote.png)

### Cluster Centroid

- Accuracy Score: 51.2%
- Precision High Risk: 0%
- Precision Low Risk: 100%
- Recall High Risk: 58%
- Recall Low Risk: 44%

![This is an image](https://github.com/jstawarz/credit_risk_analysis/blob/main/resources/cluster_centroid.png)

### SMOTEENN

- Accuracy Score: 68.0%
- Precision High Risk: 1%
- Precision Low Risk: 100%
- Recall High Risk: 76%
- Recall Low Risk: 60%

![This is an image](https://github.com/jstawarz/credit_risk_analysis/blob/main/resources/smoteenn.png)

### Random Forest 

- Accuracy Score: 64.8%
- Precision High Risk: 56%
- Precision Low Risk: 100%
- Recall High Risk: 30%
- Recall Low Risk: 100%

![This is an image](https://github.com/jstawarz/credit_risk_analysis/blob/main/resources/random_forest.png)

### Easy Ensemble

- Accuracy Score: 92.2%
- Precision High Risk: 6%
- Precision Low Risk: 100%
- Recall High Risk: 91%
- Recall Low Risk: 9%

![This is an image](https://github.com/jstawarz/credit_risk_analysis/blob/main/resources/easy_ensemble.png)


## Summary

When looking at the machine learning models, the model with the highest accuracy score is the Easy Ensemble model with 92.2%. However, 
as credit risk is inherently imbalanced, it is important to take into consideration the precision and recall scores as well. 

With regard to precision versus recall, in this case, recall or sensitivity is more important as Lending Club will want to ensure that 
high risk loans are accurately identified as such. Additionally, we can look for the model that has the least amount of high risk loans
misidentified as low risk loans. Here, the model with the highest recall rate for high risk loans is aslo the Easy Ensemble model with 91%. 

Owing to the high accuracy rate, and high recall rate for high risk loans, I would recommend using the Easy Ensemble model. 


