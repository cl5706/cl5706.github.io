# Convolutional neural Network     
Convolutional Neural Network, known as CNN, is an important field in machine learning. Here is an introduction to it.       
## Why do we need neural network?
Before neural network, we have already learned linear and logistic regression model. But there are some situtations where these two models can't work well in.         
For example, when we meet the XOR function, we will get very low accuracy if we fit in a linear model.      
Thus, we need other models beyond these two to solve such complicated problems, and here comes neural Network.
## What is neural network?
### Classification: 
$$P(y=1|x)= \frac{1}{1+e^{\overrightarrow {w}^{T}x}}$$       
On one hand, we can view this classification model as a linear model followed by a sigmoid function. On the other hand, however, we can view it as a network.Think of the input x1,x2...,xn as n nodes of a tree in layer 1, and we are passing from n nodes in layer 1 to one node in layer 2 thoughout the process. This is an example of a simple network, wehre the nodes being the neurons. 
### Regression：
$$\hat y = \overrightarrow {w}^{T}x$$      
Similarly, we can also view the linear regression model as a network. We take each of the dimensions of the input as a scalar value for a neuron, and we can get a network that maps from multiple neurons to one neuron, which is the output.   
### Multi-values Regression: 
$$\hat y = Wx$$  
Both classification and regression map from n dimension to 1 dimension, what if we want to map from n dimension to n dimension? Instead of having only one output, we can have multiple outputs. let each element in vector x be an input node and each element in vector y be an output node.


Hi
Nov.3rd
