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

### Changing the model to try and achieve the 75% accuracy goal.

Attempt 1: Removed additional feature, that is the 'SPECIAL_CONSIDERATIONS' column. Rest of the model components stayed the same, we increased the accuracy to 72.6%.

![2nd attemp Accuracy](https://user-images.githubusercontent.com/100821974/179638372-da6daa13-abad-4348-959d-5f24c48ea6b9.png)


Attempt 2: Adding Additional neurons to hidden layers and additional hidden layers are added. Accuracy did not increase or decrease it remained at 72.6%.

![3rd attemp Deep model Accuracy](https://user-images.githubusercontent.com/100821974/179638588-5af912c5-ca2f-4ca5-8955-bf0763ed0448.png)
![3rd attemp accuracy](https://user-images.githubusercontent.com/100821974/179638692-d94a92c7-3450-4002-b84a-908b6b38291a.png)

Attempt 3: Changing activation function of output layer from "sigmoid" to "tanh." The accuracy of the model did not change for the 72.6%.

![4th Attempt changed output layer to tanh](https://user-images.githubusercontent.com/100821974/179639161-f72173da-fce2-48bf-9e17-b4b9dfef5e1f.png)
![4th Attempt Accuracy](https://user-images.githubusercontent.com/100821974/179639172-a0b66708-6844-4c3c-8b5a-e99fcc3403a9.png)

## Summary

The model ended up with the accuracy score of 72.6% after optimization. The initial neural network had a accuracy score of 72.5%. We succeeded in a minor accuracy increase.  We could further optimize our neural network by removing more features or simply adding more data to the dataset to increase accuracy, possible achieving the 75% goal.
