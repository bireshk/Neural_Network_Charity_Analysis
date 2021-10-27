# Neural Network Charity Analysis
## Analysis Overview

The purpose of this project is to use deep-learning neural networks with the TensorFlow platform in Python, to analyze and classify the success of charitable donations.
Following methods for the analysis were used:

* preprocessing the data for the neural network model
*	compile, train and evaluate the model and finally,
*	optimize the model

## Results
### Data Preprocessing

* This column IS_SUCCESSFUL is considered as the target for our deep learning neural network. This column contains binary data refering to weither or not the charity donation was used effectively
* The columns APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT are the features for our model
* The columns EIN and NAME are identification information and have been removed from the input data

### Compiling, Training, and Evaluating the Model

* This deep-learning neural network model is made of two hidden layers with 80 and 30 neurons 
The input data has 43 features, the output layer is made of a unique neuron as it is a binary classification.
To speed up the training process, we are using the activation function ReLU for the hidden layers. As our output is a binary classification, Sigmoid is used on the output layer.
For the compilation, the optimizer is adam and the loss function is binary_crossentropy
* The model accuracy is under 75%. NOT a satisfying performance to help predict the outcome of the charity donations
•	To increase the performance of the model, I applied bucketing/binning to the feature ASK_AMT and organized the different values by intervals. We increased the number of neurons on one of the hidden layers, then used a model with three hidden layers. Tried a different activation function (tanh) but none of these helped improve the model's performance.

## Summary
The deep learning neural network model did not achieve the expected target of 75% accuracy. As this target is pretty average I could say that the model is not outperforming.
We could use a supervised machine learning model such as the Random Forest Classifier to combine a multitude of decision trees to generate a classified output and evaluate its performance against our deep learning model.


