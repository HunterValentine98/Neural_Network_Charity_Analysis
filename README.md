# Neural_Network_Charity_Analysis

## Overview of the Analysis
Beks has come a long way since her first day at that boot camp five years ago—and since earlier this week, when she started learning about neural networks! Now, she is finally ready to put her skills to work to help the foundation predict where to make investments.

With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to help Beks create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team, Beks received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as the following:

EIN and NAME—Identification columns
APPLICATION_TYPE—Alphabet Soup application type
AFFILIATION—Affiliated sector of industry
CLASSIFICATION—Government organization classification
USE_CASE—Use case for funding
ORGANIZATION—Organization type
STATUS—Active status
INCOME_AMT—Income classification
SPECIAL_CONSIDERATIONS—Special consideration for application
ASK_AMT—Funding amount requested
IS_SUCCESSFUL—Was the money used effectively

## Results
### Naive Random Oversampling
- Precision Score: 0.01
- Recall Score: 0.71
- F1 Score: 0.02

### SMOTE Oversampling
- Precision Score: 0.01 
- Recall Score: 0.61 
- F1 Score: 0.02

### Undersampling
- Precision Score: 0.01
- Recall Score: 0.69
- F1 Score: 0.01

### Combination Sampling
- Precision Score: 0.01
- Recall Score: 0.70 
- F1 Score: 0.02

### Balanced Random Forest Classifier
- Precision Score: 0.03
- Recall Score: 0.70
- F1 Score: 0.06

### Easy Ensemble AdaBoost Classifier
- Precision Score: 0.09
- Recall Score: 0.92
- F1 Score: 0.16

## Summary
When looking for a model to that predicts bad loans, neither of our oversampling models produced predictions that would be usable for actual use. Our Undersampling model produced similar results, so I would not recommend this model either. Our combination sampling produced a model that with almost identical scores to our Naive Random Sampling model. None of these models should be used for predictions.

When referring to our Classifier results, lets begin with the balanced random forest classifier first. We had a precision score of 0.03, meaning our precision definitely needs to improve(3/100). It was able to detect 70% of bad loans. The F1 score of 0.06 is still extremely low. This model should not be used.

Our Easy Ensemble AdaBoost Classifier produced much better results. Our recall score of 0.92 means we detected 92% of bad scores. Yet our precision score would lead me to believe we still should not use this model. At 0.09, only 9 of 100 bad loan applications the model believed were bad, 9 were actually only bad.
