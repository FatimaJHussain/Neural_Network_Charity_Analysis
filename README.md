# Neural_Network_Charity_Analysis

## Overview of the loan prediction risk analysis:

The purpose of this analysis is to create a binary classifier using neural networks. This classifier is expected to be capable of predicting whether applicants will be successful if funded by Alphabet Soup. Alphabet Soup’s business data includes more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are number of columns capturing metadata about each organization. We will use this metadata and neural networks to predict the success rate of organizations. 
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

Only 72 % accuracy is achieved with the following specifications.
![Model](https://github.com/FatimaJHussain/Neural_Network_Charity_Analysis/blob/main/model.png)
![Result](https://github.com/FatimaJHussain/Neural_Network_Charity_Analysis/blob/main/result.png)


* Were you able to achieve the target model performance?

We aimed to improve the accuracy more than 72% and by using follwoing specifications, we achieved 77% accuracy.

![Model-Optimization](https://github.com/FatimaJHussain/Neural_Network_Charity_Analysis/blob/main/optimization-model.png)
![Optimization-Results](https://github.com/FatimaJHussain/Neural_Network_Charity_Analysis/blob/main/optimization-results.png)

* What steps did you take to try and increase model performance?

We decreased the number of neurons in the second layer and also tried saving the model's weights every 5 epochs, and it helped improving the model accuracy to 77%.
We tried changing activationfunction from Relu to Tanh, but it didnot make any accuracy enhancement.


## Summary:

Neural Networks is used to predict the success of the organization. Instead of NNs, Random Forest algorithm and Logistic Regression can also be used. 
Neural networks are prone to overfitting and can be more difficult to train than a straightforward logistic regression model. Therefore, if you are trying to build a classifier with limited data points (typically fewer than a thousand data points), or if your dataset has only a few features, neural networks may be overcomplicated. Additionally, logistic regression models are easier to dissect and interpret than their neural network counterparts, which tends to put more traditional data scientists and non-data experts at ease. In contrast, neural networks (and especially deep neural networks) thrive in large datasets. Datasets with thousands of data points, or datasets with complex features, may overwhelm the logistic regression model, while a deep learning model can evaluate every interaction within and across neurons. 

Random Forest Again, if we compare both model's predictive accuracy, their output is very similar. Both the random forest and deep learning models were able to predict correctly whether or not a loan will be repaid over 80% of the time. Although their predictive performance was comparable, their implementation and training times were not—the random forest classifier was able to train on the large dataset and predict values in seconds, while the deep learning model required a couple minutes to train on the tens of thousands of data points. In other words, the random forest model is able to achieve comparable predictive accuracy on large tabular data with less code and faster performance. The ultimate decision of whether to use a random forest versus a neural network comes down to preference. However, if your dataset is tabular, random forest is a great place to start.
