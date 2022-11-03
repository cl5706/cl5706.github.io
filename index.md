# Convolutional neural Network     
Convolutional Neural Network, known as CNN, is an important field in machine learning. Here is an introduction to it.       
## What is neural network?
### Simple Examples:
#### Classification: 
$$P(y=1|x)= \frac{1}{1+e^{\overrightarrow {w}^{T}x}}$$       
On one hand, we can view this classification model as a linear model followed by a sigmoid function. On the other hand, however, we can view it as a network.Think of the input 1,x1,x2...,xn as n nodes of a tree in layer 1 (1 be the bias when there is no importantce), and we are passing from n nodes in layer 1 to one node in layer 2 thoughout the process. This is an example of a simple network, wehre the nodes being the neurons. 
#### Regression：
$$\hat y = \overrightarrow {w}^{T}x$$      
Similarly, we can also view the linear regression model as a network. We take each of the dimensions of the input as a scalar value for a neuron, and we can get a network that maps from multiple neurons to one neuron, which is the output.   
#### Multi-values Regression: 
$$\hat y = Wx$$  
Both classification and regression map from n dimension to 1 dimension, what if we want to map from n dimension to n dimension? Instead of having only one output, we can have multiple outputs. let each element in vector x be an input node and each element in vector y be an output node.                
## Why do we need neural network?
Before neural network, we have already learned linear and logistic regression model. But there are some situtations where these two models can't work well in.    
### Feature Transformation:
For example, when we have a circle-shaped data, we need to change the space from x,y axis to r, θ space by certain radio function first and then apply linear model to it. Whatsmore, in real problems the transformation may not be clear enough to be written out, which makes the transformation even harder. In this case, neural network can find the feature transform automatically just by adding an "n to n" hidden layer between the input layer and output layer. However, if this hidden layer is linear, we can never get non-linear transformation like the radio function do. All elements in the hidden layer are just linear combiantion of the input elements:     
$$h_j = \sum_{i=1}^{d}w_{ij}x_i$$     
To fulfill this, we need to add a non-linear function after the linear combination:
$$h_j = g(\sum_{i=1}^{d}w_{ij}x_i)$$     
Here, g is a non-linear function applying on the linear value. g can be any function that is continuous and derivative theoretically, but the computer can run faster if the gradient is simple. Some examples can be tanh, sigmoid or relu function.
### XOR Function          
When we meet the XOR function, we will get very low accuracy if we fit in a linear model. Here, we can build a neural network to make the classification using sigmoid function. We will find a number between 0 to 1 after the process, and we can round it to get the final output.         
## Deep Learning:
Deep learning literally just means more hidden layers. As we have more layers, the network gets deeper and can perform more complicated function.








Nov.3rd
