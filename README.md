# Multiclass-classification-for-MNIST
Multi Layer Neural Network for binary and multi-class classification
The ipython notebook is divided into the following sections:

1. Data preparation
2. Feedforward
3. Loss computation
4. Backpropagation
5. Parameter updates
6. Model training and predictions

## Data Preparation
Firstly, we load the data using the function load_data(). The function data_wrapper() is then applied to the data to get the train and test data in the desired shape. Please note that the code needs to take a batch of data points as the input. Hence, be careful while checking the dimensions.

 You already know that we have 28x28 greyscale images in the MNIST dataset. Hence, each input image is a vector of length 784. The ground truth labels of a batch are stored in a matrix which is converted to a one-hot matrix. Also, the output of the model is a softmax output of length 10.
 
## Loss Calculation
The loss used for multiclass classification is the cross-entropy loss.

## Back Propagation
The parameters dictionary is getting updated in place at each step.
The memories from L_layer_forward consisting of the tuple memory = (linear_memory, activation_memory) for each layer is used in backpropagation
The backpropagation process will run in a loop from the last layer to the first, and each loop will compute the gradients for Z,H,W,b.

## Parameter Updates
In this section, you have to define the function that updates the weights and biases for all the layers using a 'for' loop.

## Model Training
This is the final step in which you combine all the functions created above to define an 'L_layer_model'. 
