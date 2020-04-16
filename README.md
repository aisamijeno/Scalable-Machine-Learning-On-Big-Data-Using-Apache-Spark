### **IBM Introduction to Deep Learning & Neural Networks with Keras Course Project**

------
This repository is a submission of *Aisa Mijeno* for Scalable Machine Learning On Big Data Using Apache Spark course project.
<br>

#### **Project Description**
****
In this course project, you will build a regression model using the deep learning Keras library, and then you will experiment with increasing the number of training epochs and changing number of hidden layers and you will see how changing these parameters impacts the performance of the model.

#### Dataset
****
For your convenience, the data can be found here again: https://cocl.us/concrete_data. To recap, the predictors in the data of concrete strength include:

* Cement
* Blast Furnace Slag
* Fly Ash
* Water
* Superplasticizer
* Coarse Aggregate
* Fine Aggregate

#### Instructions
****
**PART A**
A. Build a baseline model.

Use the Keras library to build a neural network with the following:
- One hidden layer of 10 nodes, and a ReLU activation function
- Use the adam optimizer and the mean squared error as the loss function.

1. Randomly split the data into a training and test sets by holding 30% of the data for testing. You can use the train_test_split helper function from Scikit-learn.
2. Train the model on the training data using 50 epochs.
3. Evaluate the model on the test data and compute the mean squared error between the predicted concrete strength and the actual concrete strength. You can use the mean_squared_error function from Scikit-learn.
4. Repeat steps 1 - 3, 50 times, i.e., create a list of 50 mean squared errors.
5. Report the mean and the standard deviation of the mean squared errors.

Submit your Jupyter Notebook with your code and comments.

**PART B**
B. Normalize the data.

Repeat Part A but use a normalized version of the data. Recall that one way to normalize the data is by subtracting the mean from the individual predictors and dividing by the standard deviation.

*How does the mean of the mean squared errors compare to that from Step A?*

**PART C**
C. Increate the number of epochs

Repeat Part B but use 100 epochs this time for training.

*How does the mean of the mean squared errors compare to that from Step B?*

**PART D**
D. Increase the number of hidden layers

Repeat part B but use a neural network with the following instead:
- Three hidden layers, each of 10 nodes and ReLU activation function.

*How does the mean of the mean squared errors compare to that from Step B?*
