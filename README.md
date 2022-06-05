# Neural_Network_Charity_Analysis
An evaluation of a charity's likelihood to succeed using neural networks

## Overview
Using a dataset on successful and unsucessful charity's a neural network was created to evaluate the likelihood of success. Several models of the neural model were create to try and optimize the prediction.


## Results
### Data Preprocessing

- The target variable
  - Both Models
    - 'IS_SUCCESFUL'  

- The feature vairables
  - Final Model
    - 'INCOME_AMT'
  - Initial Model
    - 'APPLICATION_TYPE'
    - 'AFFILIATION'
    - 'CLASSIFICATION'
    - 'USE_CASE'
    - 'ORGANIZATION'
    - 'STATUS'
    - 'INCOME_AMT'
    - 'SPECIAL_CONSIDERATIONS'
    - 'ASK_AMT'
- Ignored Variables
  - Final Model
    - 'EIN'
    - 'NAME'
    - 'APPLICATION_TYPE'
    - 'AFFilIATION'
    - 'CLASSIFICATION'
    - 'USE_CASE'
    - 'ORGANIZATION'
    - 'STATUS
    - 'SPECIAL_CONSIDERATIONS'
    - 'ASK_AMT'
  - Initial Model
    - 'EIN'
    - 'NAME'

### Compiling, Training and Evaluating the Model
- Neurons, Layers and Activation Functions
  - Initial Model
    - There were two layers with 80 and 30 neurons respectively. They both used 'Relu' as the Activation function and the output layer used 'Sigmoid'
  - Final Model
    - There were three layers with 20, 10 and 5 neurons respectively. The first layer used 'Swish' function while the second and third layer used 'Relu' and the output layer used 'Sigmoid'
    - The decrease in neurons did not impact the accuracy of the model. Using the swish function seemed to improve the rate at which the model attained its maximum accuracy.
- Target Model Performance
  - The final model was not able to achieve the 75% accuracy
- Model Optimization
  - Removal of all features except 'INCOME_AMT'
  - Adding a third hidden layer
  - Changing the first hidden layer actication function to 'Swish'

## Summary
The Neural network created to evaluate the likelihood of success of a charity performed poorly only having an accuracy 53%. It might be better to use some form of supervised learning like a SVM as only one feature was used in the model to predict success.
