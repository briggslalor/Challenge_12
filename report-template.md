# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

In this project and analysis, the goal was to analyze potential loans and predict whether or not they are healthy or high-risk loans. The analysis is conducted on the financials of potential borrowers, inlcuding their income, debt-to-income ratio, number of accounts, derogatory marks and total debt. Given these variables and the desired loan size and interest rate, we attempted to build a model that could predict whether or not the loan is a healthy option. 

Using data collected from 77,536 loans and their outcomes, a model was built using supervised machine learning techniques and the Logistic Regression model. The data was first split into 70% training data and 30% testing data. Next a logistic regression model was fit to the training data. Finally, the fitted model was applied to the testing data to determine its ability to predict known loan outcomes. Once the original data was tested, the model was run again but with the addition of resampling the data before fitting the model. Due to inbalances in the initial data classes, it was important to test the data again using the oversampling method. This allowed for a more accurate and sensitive model to be constructed. 

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
  
  *Accuracy: 95.2%
  
  *Precision: 
      `0` Class: 100%
      `1` Class: 85%
      
  *Recall:
      `0` Class: 99%
      `1` Class: 91%



* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

  *Accuracy: 99.4%
  
  *Precision: 
      `0` Class: 100%
      `1` Class: 84%
      
  *Recall:
      `0` Class: 99%
      `1` Class: 99%



## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

Based on the results of both models, I would recommend the resampled model as being a better option for the project. While the accuracy score is slighlty higher for the second model, it also increases the recall for the unhealthy loan class, `1`, while on sacrificing 1% in the precision. I believe that this is an important difference and trade off as its more important to correctly predict potentially unhealthy loans and deny them. 

If you do not recommend any of the models, please justify your reasoning.
