# Sequential-Nerual-Network

Sudent Project for UC Davis MSBA

Model Summary

## Step 1: Define the Model. Setting up the layers.

Per rules of thumb, one hidden layer would suffice for vast number of applications. This dataset is not a complicated one and therefore one hidden layer is selected.
Additionally, the amount of nodes usually falls under 2/3 of the input layer. In our case we have 8 inputs and therefore we can experiment with 4-6 nodes. After comparing, 5 nodes seemed to yield lower MSE.
Activation function: After trying sigmoid and relu, relu seemed to yield better result than sigmoid. Sigmoid could be more commonly used in classification questions, and in our case we are solving a regression problem, hence selecting relu.

## Step2: Compile the Model with optimizer, loss function and metrics.

Metrics: We select RMSE as metrics to better evaluate the result of a regression (numerical) output.

## Step 3: Fit the Model

epochs / batch size: As we ae using Stochastic Gradient Descent as our optimizer, we choose the batch size of 1 to iterate through one sample at a time. As for number of iteration of the dataset, we choose epoch = 100 as commonly used. In theory, epoch is usually large to allow the learning algorithm to run until the error from the model has been sufficiently minimized.

## Step 4: Evaluate the Model

The model has a low RMSE of 0.087 and MSE of 0.0075.
