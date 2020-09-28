# NeuralNetworks_DeepLearning

This project is to help a non-profit foundation who dedicates to help organizations that protect the environment, improve people's well-being and unify the world to analyze which orgnizations are worth to donate to and which are too high risk.

We used supervised learning models for this project to make the predictions. We trained and compared Nerual Network model and some other machine learning models' performance.

## Techniques used in this Project
 - Use TensorFlow to implement neural network models and deep neural network.
 - Use testing accurracy score to explain how different neural network structures change algorithm performance.
 - Use testing accurracy score to compare the differences between the traditional machine learning classification and regression models and the neural network models.
 - Use Keras Sequential model’s save method to export the entire model (weights, structure, and configuration settings) 
 
## Data Preprocessing

 - Low variance variables 
  - Numerical variable(s)
  
  [Variable Statistics](https://github.com/karenmxm/NeuralNetworks_DeepLearning/blob/master/Images/Stats.png)
  
  <img src= https://github.com/karenmxm/NeuralNetworks_DeepLearning/blob/master/Images/Stats.png width=50%>

## Nerual Network Model 
  - Two hidden layers were used for the Neural Network model. 
  - The choosing of the number of neurons is based on rule of thumb that the number of neurons is 2-3 times of inputs. There are 69 inputs, so 138 neurons are used in the first layer and 30 neurons in the second hidden layer. 
  - The higest predictive accuracy score I acheived is 0.7341 which is lower than the target model performance 0.75. 
  - To increase model performance, I tried the following steps:
    - I leave out noisy variables from features. Bucketed two categorical variables to avoid some of the categories have too few data. Scaled data to avoid outliers.
    - I tried different number of hidden layers. I tried from 1 to 5 hidden layers and found 2 hidden layers works best.
    - I tried different activation functions including relu, tanh and sigmoid functions. I found sigmoid function works better.
    - I tried three different epochs: 100, 200 and 300 and used 100 epochs.

## Alternative Models
I campared Nerual Network model performance with Random Forest, Gradient Boosting Trees, Logistic Regression and SVM models. I found Gradient Boosting Trees can acheive similar accuracy to Nerual Network for this dataset. The training Accuracy score is 0.746. And the validation Accuracy score is 0.731.

| Machine Learning Model   | Accuracy | Benefits | limitations |
| :------------------------|----------|----------|-------------|
| Nerual Network           | Training: 74.56% Testing: 73.41%    | | |
| Logistic Regression      | 72.3%    | Easy to implement. Tuning of hyperparameters not needed.| Lack flexibility. Might suffer from model mis-specification.|
| Random Forest            | Training: 73.9%; Testing: 72.9%  | Reduce the risk of overfitting and hgher accuracy than Decision Tree model.| Computation relatively expensive.|
| Gradient Boosting Tree   | Training: 74.6%; Testing: 73.1%  | Good model performence. Less prone to overfitting.| Hard to tune as there are too many hyperparameters. |
| SVM                      | Training: 72.6%; Testing: 72.2%  | Computation faster. | Poor performence.|
