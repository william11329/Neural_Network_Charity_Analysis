# Neural_Network_Charity_Analysis
## Overview
This project allows us to analyze the impact of funding contributions of an upwards of 34k orginizations with applications submitted in order to recieve funding.

We utilize Tensorflow Keras models with dense hidden layers along with a binary classifier to evaluate the dataset with hopes of predicting which applicants would be successful when funded by Alphabet Soup.

## Results

### Data Preprocessing
- The column titled "IS_SUCCESSFUL" is the target for this model. It contains binary data reflecting whether or not a donation from Alphabet Soup was used succesfully.

- The columns AFFILIATION, APPLICATION_TYPE, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, ASK_AMT, SPECIAL_CONSIDERATIONS are the features of this model.

- The columns EIN and NAME are identification information, they can, and have been have been removed from the input data.

### Compiling,Training, and Evaluating the Model
- This model was made up of two hidden layers with 80 neurons and 30 neurons.

- My hidden layers utilized the ReLU functions and my output layers utilized the Sigmoid function. These functions were chosen to speed up the training process. The model uses adam as the optimizer and sets the loss function to binary_crossentropy.

- This models performance was to reach a 75% accruacy. After several attempts I was still unable to reach that percentage for my accuracy.

- To increase the accuracy of the model bucketing to the ASK_AMT feature was attempted, increasing the number of hidden layers, as well as experimenting with the number of neurons for hidden layers. Unfortunately my highest accuracy model was at 72.6%.

## Summary
While the goal of 75% accuracy was presented, I was only able to obtain a 72.6% accuracy. Several 
attempts lead me to try adding neurons, or changing hidden layers as well as using different activation functions with not much difference.

## Possible Recommendations
A possible alternative could be a Random forest classifier model. It would be appropriate for this type of 
binary classification problem and could offer comparable results to deep learning models with only 2 hidden
layers.