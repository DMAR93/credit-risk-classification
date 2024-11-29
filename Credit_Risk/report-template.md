# Credit Risk Analisis Report

## Overview of the Analysis

**Explain the purpose of the analysis:**  The goal of this analysis is to assess the creditworthiness by
predicting the loan outcome basing on historical lending data. This analysis uses a machine learning to
develop a classification model to aid in risk evaluation.

**Explain what financial information the data was on, and what you needed to predict.:**  The dataset 
includes financial information related to lians, with features like loan amount, interest rate and borrower 
data. The target Variable is Loan Status.
**Provide basic information about the variables you were trying to predict (e.g., `value_counts`).:**   
Variable Loan Status. 0 = Healthy loans and 1 = High-risk loans.
**Describe the stages of the machine learning process you went through as part of this analysis.:**  
* **Data preprocessing:** Features X and Labels y (Loan status), were separated. Also the data was split
 into training and testing sets using and 80-20 split
* **Model Selection and training:** The model used was Logistic Regression, a widely used algorithms for 
binary classification.
* **Model Evaluation:** Performance metrics like "Accuracy", "Precision", "Recall" and "F1-score were 
used to evalueated the model.

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine
learning models:

### Logistic Regression Model Performance:
**Accuracy:** 99%
**Precision:**
* Healthy Loans = 0.99
* Hight Risk Loans = 0.86

**Reacall:**
* Healthy Loans = 0.99
* Hight Risk Loans = 0.94

So as a results we could see that the accuracy show us that it correctly classifies loans with hight
reliabilty with a 99% of accuracy. The precision show us that no healthy loans are predicted as high risk
on the other hand hight risk loans with 86% evidence that there are some False positives results. finally
in Recall high risk loans with 94% meaning the model effectively identifies most high-risk loans, with
small numbers missed. 


## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

The logistic regression model performs really well, achieving high accuracy, achieving high accurracy, 
precision, recall and F1-scores. These metrics indicate that the model is both effective and reliable for predicting credit
risk.

**Recomendations:**
* Adopt the Logistic Regression Model: Its high accuracy and balanced metrics make it suitable for production.
* Business Priority: Focus on recall for high-risk loans (1), as identifying as many high-risk loans as possible is critical
for minimizing financial loss. the model alreadyachieve a recall of 94%for this category, which is excellent.

**Future Steps:**
- Explore other models
- Try to optimize the logistic regression model
- try to get more feature especification 
