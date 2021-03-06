# Neural_Network_Charity_Analysis

## Overview of the analysis

With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to help Beks create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team, Beks received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years.

## Results

### Data Preprocessing
- What variable(s) are considered the target(s) for your model?
  - "IS_SUCCESSFUL" - Was the money used effectively
- What variable(s) are considered to be the features for your model?
  -  APPLICATION_TYPE — Alphabet Soup application type
  -  AFFILIATION — Affiliated sector of industry
  -  CLASSIFICATION — Government organization classification
  -  USE_CASE — Use case for funding
  -  ORGANIZATION — Organization type
  -  STATUS — Active status
  -  INCOME_AMT — Income classification
  -  ASK_AMT — Funding amount requested
- What variable(s) are neither targets nor features, and should be removed from the input data?
  - EIN, NAME — Identification columns
  - SPECIAL_CONSIDERATIONS — Special consideration for application

### Compiling, Training, and Evaluating the Model
- How many neurons, layers, and activation functions did you select for your neural network model, and why?
  - 2 ReLu layers with 80 and 20 neurons, respectively, as it is the most commonly used activation function. We did not want to add too many layers or neurons in case of overfitting.
  - ![](https://raw.githubusercontent.com/Oysterrr/Neural_Network_Charity_Analysis/main/Resources/d2_model.png)

- Were you able to achieve the target model performance?
  - Unfortunately, we were not able to reach 75% accuracy. 
  - ![](https://raw.githubusercontent.com/Oysterrr/Neural_Network_Charity_Analysis/main/Resources/d2_results.png)
- What steps did you take to try and increase model performance?
  - We first dropped the 'SPECIAL_CONSIDERATIONS' variable from our model. Originally only 'NAME' and 'EIN' were dropped.
  - We experimented with changing the activation layer type, as well as number of layers and epochs. Unfortunately, this also did not give us a satisfactory 75%+ accuracy score.
  - ![](https://raw.githubusercontent.com/Oysterrr/Neural_Network_Charity_Analysis/main/Resources/d3_1.png)
  - ![](https://raw.githubusercontent.com/Oysterrr/Neural_Network_Charity_Analysis/main/Resources/d3_2.png)
  - ![](https://raw.githubusercontent.com/Oysterrr/Neural_Network_Charity_Analysis/main/Resources/d3_3.png)
  - All of the attempts netted an accuracy score in the 72% range.

## Summary
