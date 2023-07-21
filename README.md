# deep-learning-challenge
## Overview 
* Alphabet Soup is a non-profit foundation that provides funding to various organizations. Using a neural network model, I created a model to help the company predict if an organization will be successful if they are funded by Alphabet Soup. The target tried to reach was a 75% accuracy.
## Results: 
* Data Preprocessing
    * What variable(s) are the target(s) for your model?
      *  The variable that I targeted for my model was the Is_Successful column in the dataset.
    * What variable(s) are the features for your model?
      *  I used the following features in my dataset:
        1. APPLICATION_TYPE
        1. AFFILIATION
        1. CLASSIFICATION
        1. USE_CASE
        1. ORGANIZATION
        1. STATUS
        1. INCOME_AMT
        1. SPECIAL_CONSIDERATIONS
        1. ASK_AMT
    * What variable(s) should be removed from the input data because they are neither targets nor features?
     *  I dropped the EIN and NAME columns from the dataset, as they are not targets or features that are relevant to the model.
* Compiling, Training, and Evaluating the Model
    * How many neurons, layers, and activation functions did you select for your neural network model, and why?
     *  For my first model, I created two hidden layers with 80 neurons for layer one and 30 neurons for layer 2. At first I just wanted to get a    baseline for accuracy to determine if they model would achieve more than 75% accuracy. I used the RELU activation for both layers.
     *  For my second model, I tried to add a third layer and adjusted the neurons for each layer. Layer one had 75 neurons, layer two had 35 neurons and layer 3 had 25 neurons. I also changed the activation in each layer to TANH, instead of RELU.
     *  For my third model, I added a fourth layer and adjusted the neurons again for all layers. Layer one had 55 neurons, layer two had 35 neurons, layer 3 had 45 neurons, and the fourth had 15 neurons.
    * Were you able to achieve the target model performance?
     *  My first model only achieved 72% accuracy with 0.55 loss, and the second model had roughly the same accuracy with a 0.56 loss.
    * What steps did you take in your attempts to increase model performance?
     *  To increase the model performance, I tried to add layers, adjust the number of neurons and change the activation. I adjusted these variables several times before I was able to increase the accuracy of the model.
    
## Summary: 
* The final trained model from the keras tuner achieved 72.559% prediction accuracy with a 0.57 loss, using a sigmoid activation function with input node of 43 and 4 hidden layers with a 55, 35, 45, and 15 neurons split and 100 training epochs. I was not able to achieve the set goal of 75% accuracy in the 3 models that I tested. I would recommend that more hidden layers be added to this dataset with a different neuron split to try and achieve the desired results.
