# Neural_Network_Charity_Analysis

## Overview of the loan prediction risk analysis:

The purpose of this analysis is to create a binary classifier using neural networks. This classifier is expected to be capable of predicting whether applicants will be successful if funded by Alphabet Soup. Alphabet Soup’s business data includes more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns capturing metadata about each organization. We will use this metadata and neural networks to predict the success rate of organizations. 
## Results:
### Data Processing
* What variable(s) are considered the target(s) for your model?

Variable "IS_SUCCESSFUL" is considered as a target.
* What variable(s) are considered to be the features for your model?

Following variables are used as features for our model:

APPLICATION_TYPE,   AFFILIATION,   CLASSIFICATION,   USE_CASE, ORGANIZATION, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT          
                      
   

* What variable(s) are neither targets nor features, and should be removed from the input data?

We removed "Name" and "EIN" for Deliverable 1,2. For Deliverable 3, "Status" and "EIN" are dropped.
### Compiling, Training, and Evaluating the Model
* How many neurons, layers, and activation functions did you select for your neural network model, and why?

![Model](https://github.com/FatimaJHussain/Neural_Network_Charity_Analysis/blob/main/model.png)
![Result](https://github.com/FatimaJHussain/Neural_Network_Charity_Analysis/blob/main/result.png)


* Were you able to achieve the target model performance?

![Model-Optimization](https://github.com/FatimaJHussain/Neural_Network_Charity_Analysis/blob/main/optimization-model.png)
![Optimization-Results](https://github.com/FatimaJHussain/Neural_Network_Charity_Analysis/blob/main/optimization-results.png)

* What steps did you take to try and increase model performance?


## Summary:

There is a summary of the results 
There is a recommendation on using a different model to solve the classification problem, and justification 
