# Credit_Risk_Analysis

## Objective
The objective of this analysis was to analyze an individuals credit risk based off of several collected variables.  Machine learning techniques were used to create a model that could predict whether or not an individual was high risk or not.

## Results
* Naive Random Oversampling
  * High risk: Precision 0.01 Recall 0.6
  * Low risk: Precision 1.00 Recall 0.69
* SMOTE Oversampling
  * High risk: Precision 0.01 Recall 0.54
  * Low risk: Precision 1.00 Recall 0.74
* Underampling
  * High risk: Precision 0.01 Recall 0.53
  * Low risk: Precision 0.99 Recall 0.53
* Combination Sampling
  * High risk: Precision 0.01 Recall 0.72
  * Low risk: Precision 1.00 Recall 0.57
* Balanced Random Forest Classifier
  * High risk: Precision 0.88 Recall 0.37
  * Low risk: Precision 1.00 Recall 1.00
* Easy Ensemble AdaBoost Classifier
  * High risk: Precision 0.09 Recall 0.92
  * Low risk: Precision 1.00 Recall 0.94

## Summary
In summary, all of the models had high precision in detecting individuals deemed low risk.  However, none of the models performed well at predicting high risk individuals as seen from the low precision and recall for each machine learning model.  Given that determining credit risk is very impactful upon an individuals life, I would not recommend any of these models to access credit risk.  The low sensitivity of these models would result in several false positives.  People would be labled as high risk and potentially denied loans that otherwise they would be able to recieve.  This could be unethical for the company issuing the loans.  Alternatively, the low precision of the model indicates that there is an overwhelming number of false negatives.  By not capturing those who are truly high-risk, a company has no clear evidence to access credit risk. 

From these models it is clear that they are unacceptable to use for such a risk-adverse industry.  Perhaps they could be refined to be used as a starting point on a persons credit journey but they definitely do not tell the whole story.
