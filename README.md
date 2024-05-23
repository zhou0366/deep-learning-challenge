# Nonprofit Deep Learning Challenge

## Preprocessing

In this step, we remove application types under 500 and classification types under 100 counts in the data. The "IS_SUCCESSFUL" column is dropped as this is the y-axis we will be evaluating when we split the data.

## Compile, Train, and Evaluate

We will initially create a model with two layers of relu activation to an output layer with sigmoid activation. We will try with the first layer at 10 neurons and the second at 20. We will compile using binary cross entropy loss and Adam optimizer. 
### Results of first attempt:

![image](https://github.com/zhou0366/deep-learning-challenge/assets/22827830/065f3d0f-092b-48a7-8291-f4481de6cf4c)

## Second Attempt

For the second attempt at creating a model, the following steps were applied:

  - Add an additional layer
  
  - Increase number of neurons on new layer to 30
  
  - Add validation split of 0.1
  
### Results of second attempt:

![image](https://github.com/zhou0366/deep-learning-challenge/assets/22827830/735b175b-943d-4951-9b66-7c62ba69e3af)

The result is a very small increase in accuracy. It is possible that there could be additional improvements in the preprocessing step such as allowing additional data points to be used.
