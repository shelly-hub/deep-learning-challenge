# deep-learning-challenge

## Overview
Alphabet Soup, a nonprofit organisation needs a tool which could be used to select applicants that could have high rate of success after receiving fundings.

Thus, this challenge utilises machine learning method and neural networks to make a model that could be used for the company to predict potential successful applicants in the future. 

The extensive hyperparameters in neural networks is being trialed and analysed in order to increase model performance.

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
   - Neurons: 80 and 30
   - Layers: 2
   - Activation functions: relu and sigmoid

2. Were you able to achieve the target model performance?
   
   - No. Model accuracy is below 75%

4. What steps did you take in your attempts to increase model performance?
   
Using original data preprocessing method, changing hyperparameters do not help to increase model performance.
Therefore, data is added in the analysis in order to help to improve model accuracy

   - Data is added by adding the deleted column "EIN", this has improved model from 0.72 to 0.73 accuracy
   - Adding optimum layers to 3, and increasing neurons from 80 to 200 does improve a little. 
   - Maintain activation function to only: relu. Activation without relu will decrease the accuracy
   

## Summary
The overall model performance is around 0.73 accuracy.
As this model is used to make recommendation for company, hence accuracy around 70-75% is desirable. 
To further increase accuracy, it is recommended to use Random Forests classification algorithm for this dataset. 
Random forests could identify which column that has the highest weightage to make strongest decision, thus could help to improve the model performance. 

## References
Python | Pandas dataframe.replace()(N.D.). GeeksforGeeks. Retrieved on: 24/07/2023, from:<https://www.geeksforgeeks.org/python-pandas-dataframe-replace/>

https://colab.research.google.com/github/tensorflow/docs/blob/master/site/en/tutorials/keras/save_and_load.ipynb

Piyush Chanchal: "Is 80% accuracy good in machine learning"(N.D.). Quora. Retrieved on: 25/07/2023, from<https://www.quora.com/What-accuracy-should-I-consider-in-machine-learning-Do-I-need-to-train-my-model-and-the-last-accuracy-of-the-training-epoch-x-is-the-accuracy-that-I-show-as-my-result>

