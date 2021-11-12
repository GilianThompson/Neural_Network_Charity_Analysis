### Overview 
Using TensorFlow, design a neural network, or deep learning model, to create a binary classification model that can predict if an Alphabet Soup–funded organization will be successful based on the features in the dataset.  

### Results 
## Data Preprocessing 

## Compiling, Training, and Evaluating the Model
For the neural network, there are two hidden layers. The first has eight neurons and uses the ReLu activation function. The second hidden layer has five neurons and again uses the ReLu activation function. The output layer uses the Sigmoid activation function because of the classification problem we're trying to solve; whether or not a charity is worth funding due to the many features provided in the dataset. 

The model was able to achieve an accuracy score of 0.9998 with a loss of 1.9984e-04 after training for only 20 epochs. Although these scores are incredibly high, it could mean that the model is overfit to the data. 
