## Overview 
Using TensorFlow, design a neural network, or deep learning model, to create a binary classification model that can predict if an Alphabet Soup–funded organization will be successful based on the features in the dataset.  

## Results 
### Data Preprocessing 
The EIN and NAME columns were dropped, columns with more than 10 unique values were grouped together, and categorial variables were encoded using one-hot encoding. 

### Compiling, Training, and Evaluating the Model
For the neural network, there are two hidden layers. The first has eight neurons and uses the ReLu activation function. The second hidden layer has five neurons and again uses the ReLu activation function. The output layer uses the Sigmoid activation function because of the classification problem we're trying to solve; whether or not a charity is worth funding due to the many features provided in the dataset. 

<img width="612" alt="Screen Shot 2021-11-12 at 11 20 45 AM" src="https://user-images.githubusercontent.com/85901073/141499650-1b46da30-16d4-4459-913b-1d177fe404e8.png">

### Optimization
The model was optimized in the file AlphabetSoupCharity_Optimization.ipynb in order to achieve a target predictive accuracy higher than 75%. 
To start, I removed the STATUS and SPECIAL_CONSIDERATIONS columns in the dataframe along with EIN and NAME that were removed the first time around. For the first adjustment to the model, I tried the adding neurons to each hidden layer. The first layer had 15 neurons and the second layer 8 and ran it for 50 epochs. Both loss and accuracy were not changing so I didnt run the model for longer. The loss was approximately 0.5574 and the accuracy was 0.7308, which is not a much of an improvement from the original model. For the second adjustment to the model, I added a third hidden layer with the activation function relu. This model performed much worse with a loss of 0.6908 and an accuracy score of 0.5355. For the third attempt, the optimizer was changed to adagrad. This model worked better than my previous optimization attempts with a loss of 0.5624 and accuracy of 0.7282, but this isn't any significant improvement from any of the models. 

## Summary

