# NeuralNetworks_DeepLearning

## Nerual Network Model
  - I used two hidden layers for my Neural Network model. 
  - The choosing of the number of neurons is based on rule of thumb that it is 2-3 times of inputs.There are 138 neurons in the first layer and 10 neurons in the second hidden layer. 
  - The higest predictive accuracy score I acheived is 0.73 which is lower than the target model performance 0.75. 
  - To increase model performance, I tried the following steps:
    - I increased the number of hidden layers. I tries through 1 to 5 hidden layers and found 2 hidden layers works best.
    - I tried different activation functions including relu, tanh and sigmoid functions. I found sigmoid function works better.
    - I tried three different epochs: 100, 200 and 300.

## Alternative Models
I campared Nerual Network model performance with Random Forest, Gradient Boosting Trees, Logistic Regression and SVM models. I found Gradient Boosting Trees can acheive similar accuracy to Nerual Network for this dataset. The training Accuracy score is 0.735. And the validation Accuracy score is 0.729.
