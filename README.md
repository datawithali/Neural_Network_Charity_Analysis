# Neural_Network_Charity_Analysis

## Neural Networks and Deep Learning Models

## Overview

Compare the differences of the traditional, regression, and neural machine learning models.
Describe the perceptron model and its components.
Using TensorFlow, implement neural network models.
Explain how different neural network structures change algorithm performance.
Preprocess and construct datasets for neural network models.
Compare the differences between neural network models and deep neural networks.
Implement deep neural network models using TensorFlow.
Save trained TensorFlow models for later use.Describe the perceptron model and its components.

## Purpose

A foundation, Alphabet Soup, wants to predict where it should make investments. Goal, use machine learning and neural networks to apply features on a provided dataset to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. Initial file has 34,000 organizations that provides a list of columns that capture metadata about each organization from past successful fundings.

## Results

What variable(s) are considered the target(s) for your model? We'll check to see if the target is marked as successful in the DataFrame, which would indicat that it has been successfully funded by AlphabetSoup.![206861155-e5357c76-7d14-48c6-89d7-fa43de3603f9](https://user-images.githubusercontent.com/109055148/213894514-0f0e5791-099b-42e6-a6fb-86109f6f451c.png)


What variable(s) are considered to be the features for your model? The IS_SUCCESSFUL column was used to feature this dataset.

What variable(s) are neither targets nor features, and should be removed from the input data? Both EIN and NAME columns will not increase the accuracy of the model, they can be removed to improve code efficiency.

How many neurons, layers, and activation functions did you select for your neural network model, and why? The optimized model, layer 1 started with 120 neurons with a relu activation. Layer 2, dropped to 80 neurons and continued with the relu activation. The sigmoid activation appeared to be the better fit for layers 3 40 neurons and layer 4 20 neurons.

![206861026-3b075711-3d35-43f6-be86-ad136070df68](https://user-images.githubusercontent.com/109055148/213894481-5a08b438-bea9-4f10-8434-b146c122bcee.png)


![206861040-82e494d1-097d-4c57-9978-628496ff9c8f](https://user-images.githubusercontent.com/109055148/213894488-8017a0b9-f5fd-4385-ae4e-0cd608b0830b.png)

Were you able to achieve the target model performance? The target for the model was 75%, however, the model accuracy is under 75%. This is not a satisfying performance to help predict the outcome of the charity donations.

What steps did you take to try and increase model performance? Columns were reviewed and the STATUS and SPECIAL_CONSIDERATIONS columns were dropped as well as increasing the number of neurons and layers. Other activations were tried such as tanh, but the range that model produced went from 40% to 68% accuracy. The linear activation produced the worst accuracy, around 28%. The relu activation at the early layers and sigmoid activation at the latter layers gave the best results.


![206861151-448e34b8-569f-4fc7-982d-4ae3efc54152](https://user-images.githubusercontent.com/109055148/213894494-2e0467b4-3361-49f7-8844-37ec6b853ca2.png)

![206861155-e5357c76-7d14-48c6-89d7-fa43de3603f9](https://user-images.githubusercontent.com/109055148/213894522-f0aa7fea-ea92-46b3-8d17-4d54b7bbd9d8.png)

## Summary

The relu and sigmoid activations yielded a 47.7% accuracy, which is well below the target of 75%

