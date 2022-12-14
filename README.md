# Neural_Network_Charity_Analysis

## Overview of the Analysis
Beks has come a long way since her first day at that boot camp five years ago—and since earlier this week, when she started learning about neural networks! Now, she is finally ready to put her skills to work to help the foundation predict where to make investments.

With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to help Beks create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team, Beks received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as the following:

- EIN and NAME—Identification columns
- APPLICATION_TYPE—Alphabet Soup application type
- AFFILIATION—Affiliated sector of industry
- CLASSIFICATION—Government organization classification
- USE_CASE—Use case for funding
- ORGANIZATION—Organization type
- STATUS—Active status
- INCOME_AMT—Income classification
- SPECIAL_CONSIDERATIONS—Special consideration for application
- ASK_AMT—Funding amount requested
- IS_SUCCESSFUL—Was the money used effectively

## Results
### Data Preprocessing
- What variable(s) are considered the target(s) for your model?

We focuseed on the "Is-Successful" variable for this model.

- What variable(s) are considered to be the features for your model?

Application, Name, Type, Affiliation, Classification, Use_Case, Organization, Income_Amt, Special_Considerations, Status, and Ask_Amt

- What variable(s) are neither targets nor features, and should be removed from the input data?

Employer Identification Number(EIN) 
### Compiling, Training, and Evaluating the Model
- How many neurons, layers, and activation functions did you select for your neural network model, and why?

Three hidden layers each with neurons, causing our accuracy to go above 75. We kept the number of epochs constant. The first activation function was "relu" and the secon and third were "sigmoid", further increasing our accuracy.

- Were you able to achieve the target model performance?

Yes

- What steps did you take to try and increase model performance?

The biggest impact was changing our Name column to data points. 

## Summary
If I were to recommend a new model, a Random Forest model would probably be good for further analysis. This problem falls under a classification style problem, which Random Forest is good with.
