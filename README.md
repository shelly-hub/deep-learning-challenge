# deep-learning-challenge

## Overview
Alphabet Soup, a nonprofit organisation needs a tool which could be used to select successful applications to receive the fundings.

Thus, this challenge utilises machine learning method and neural networks to make a model that could give best results to predict future organisations that would be the potential successful applicants.

The extensive hyperparameters in neural networks is being trial and analysed in order to increase model performance.

The dataset used to make model prediction is provided in CSV file that contains funding information from more than 34000 organisations. 

## Results

### Data Preprocessing

1. The variable(s) for the target(s) of the model
   - "IS_SUCCESSFUL"
2. The variable(s) for the features of the model
   -  "APPLICATION_TYPE"
   -  "AFFILIATION",
   -  "CLASSIFICATION",
   -  "USE_CASE",
   -  "ORGANIZATION",
   - "STATUS",
   - "INCOME_AMT",
   - "SPECIAL_CONSIDERATIONS",
   -  "ASK_AMT"
3. The variables(s) that should be removed from the input data because they are neither targets nor features
   - "EIN"
   - "NAME"

### Compiling, Training, and Evaluating the Model
1. How many neurons, layers, and activation functions are selected for the neural network model
   - Neurons:
   - Layers:
   - Activation functions:

2. Were you able to achieve the target model performance?
   
   -Unfortunately,No. Model accuracy is below 75%

4. What steps did you take in your attempts to increase model performance?
   
   Big networks not recommended, since it is only """ observations 
   - Adding optimum layers to 3
   - Maintain activation function to only: relu
   - Create binnings for column "income_amt"

## Summary
The overall model performance is not very desirable at at around 72% accuracy.
It is recommended to use Random Forests classification algorithm for this dataset. 
Random forests could identify which column that has the highest weightage to make strongest decision, thus could help to improve the model performance. 

