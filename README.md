# MNIST - Neural Networks

## Introduction

Attempt to recognize MNIST handwritten numbers with Keras using tensorflow-gpu backend.

## Multi Layer Perceptron

* Train set : 50000 images
* Validation set : 10000 images
* Test set : 10000 images
* Batch size : 64
* Epochs : 12
* Input shape : 784
* Hidden layers : 2 layers of 512 neurons each and 'relu' activation function
* Output layer : 10 (0 to 9) with 'softmax' activation
* Optimizer : Stochastic Gradient Descent
* Loss measure : Categorical Cross Enthropy

```
Test loss: 0.060839374903682616
Test accuracy: 0.9801
```

![](https://i.imgur.com/CTlO9I6.png)
![](https://i.imgur.com/RClYr75.png)

## Convolutional Neural Network

* Train set : 50000 images
* Validation set : 10000 images
* Test set : 10000 images
* Batch size : 64
* Epochs : 12
* Input shape : (28, 28, 1)
* Hidden layers : 
    * Conv2D 32 activation 'relu'
    * Conv2D 64 activation 'relu'
    * MaxPooling2D
    * Dense 128 activation 'relu'
* Output layer : 10 (0 to 9) with 'softmax' activation
* Optimizer : Stochastic Gradient Descent
* Loss measure : Categorical Cross Enthropy

```
Test loss: 0.03202990765200775
Test accuracy: 0.9906
```
![](https://i.imgur.com/g5qky4K.png)
![](https://i.imgur.com/hprdWwM.png)

## Conclusions

We see that the convolutional neural network is more precise on image recognition than a common multi layer perceptron and generalizes better on the test set.
