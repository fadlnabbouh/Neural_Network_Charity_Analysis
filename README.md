# Neural_Network_Charity_Analysis

## Overview

The purpose of this analysis was to develop a deep learning model using TensorFlow to predict the success rate of applicants to Alphabet Soup.

## Results

Data Preprocessing
- The IS_SUCCESSFUL variable is the target variable for this classifier
- The features used to predict the target variable were: application type, affiliation, classification, use case, organization, status, income amount, special considerations, and ask amount.
- EIN and Name were not target variables nor features and were therefore removed from the dataset.

Compiling, Training, and Evaluating the Model
- I started off with using 8 neurons in the first layer and 5 in a second hidden layer with one output dimension to represent the binary classification. I used the relu activation function within the hidden layers to account for complex, non linear features and the sigmoid function in the output layer to provide the probability of the classification or result of the classifier. 
- To improve accuracy, I increased the number of neurons per layer and increased the number of layers. I also tried increasing the number of epochs. The highest accuracy was achieved via increasing the number of layers and units per layer. 
- Unfortunately, the target accuracy was not achieved. The highest achieved accuracy was 73.3%. 

## Summary

In summary, the deep learning network acheived an accuracy of 73.3%. This is just below the desired 75%. Because the number of epochs, layers, and units per layer were increased with no real change, as well as different activation functions tested, it is likely that there is insufficient data or features used that were not predictive in the dataset. A future step would be to try and drop noisey features. In addition, I would try using a different classifier model, such as a simple logistic regression or a random forest classifier. Both require less computing power and will likely provide a similar result. 