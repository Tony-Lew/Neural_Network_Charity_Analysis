# Neural_Network_Charity_Analysis

## Overview of the Analysis

Using Machine Learning and Neural Networks for this project, We used the features in the dataset to create a binary classifier that will help to predict if the applicants that will be funded by a Charitable organization called Alphabet Soup will be successful. For this analysis we had a dataset containing various measures on 34,000 organizations that have been funded by Alphabet Soup. This project compromised of the following 3 steps:

  - Preprocessing the data for the neural network
  - Compile, Train, and Evaluate the model
  - Optimizing the model
  
## Results

### Data Preprocessing

  - Variable that was considered as the target for my model: IS_SUCCESSFUL Column
  - Variables that were considered features for my model: Every Column except for IS_SUCCESSFUL which is our target and the ones we will drop
  - Variable that were neither targets or features for the dataset: Columns that I dropeed are EIN, NAME because they will have little to no impact om our outcome
  
### Compiling, Training and Evaluating the Model

The number of neurons, layers, and activation functions selected for this neural network model:

For the neural network model we used 2 hidden layers. The first layer contained 80 neurons, and the second layer contained 30. These two hidden layers we used the "relu" activation function. We then finished using an addtional output layer that used the "sigmold" function.
  ![Original Deep Nural Model](https://user-images.githubusercontent.com/100821974/179631442-955d096d-1ab6-4d50-98da-14ddeccf26f9.png)

  
Using this model did we hit the 75% accuracy target? 
  ![Original Deep Nural Model Accuracy](https://user-images.githubusercontent.com/100821974/179631437-e626424e-1a7a-4faf-9cc9-bbdfc011fc43.png)

We did not we only achived a 72.5% Accuracy.
