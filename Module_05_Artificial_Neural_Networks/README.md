# Artificial Neural Networks

## Topics covered in today's module
* Introduction to Neural Networks
* Hyperparameters
* Forward Pass
* Backpropagation
* Computing accuracy

## Main takeaways from doing today's assignment
- to_categorical() is tensorflow's function for one-hot encoding
- Hidden layers learn the latent variables and dimensions
- Output layers may parallel the number of output classes and does not have to be 1; sometimes there's even more output neurons that input features
- Weights can be represented as matrices
- We assign random weights that are within scale via the Guassian distribution to a NN first
- The transformation process goes: initialize weights, dot product weight by previous layer (in that order), sum up the weights, apply activation function
- randmom.randn(x,y) generates a matrix of size x * y with the Guassian distribution values
- Activation functions are injective and map distinct inputs to distinct outputs
    - We prefer activation functions that are smooth
- Some optimizers include RMSprop() which reach higher momentum before it changes direcction (RNNs) and Adam which has slower momentum (noise and image estimation)
- Backpropagation consists of a forward pass (get predictions and output based on current weights) and a backward pass (update gradients of weights based on loss)
- Backprop and SGD are different algorithims

## Challenging, interesting, or exciting aspects of today's assignment
I'm still kind of confused about the differences in SGD and backprop. I also don't understand the notation behind weights, and SGD and why we multiply the weight first and the the previous layer.

## Additional resources used 
- Multiplication by square root of 1/dimensionn of layer: https://pouannes.github.io/blog/initialization/ 
- Backprop and SGD: https://machinelearningmastery.com/difference-between-backpropagation-and-stochastic-gradient-descent/
- Weight Matrix: https://jmyao17.github.io/Machine_Learning/Neural_Network/NN_From_Scratch_1.html
- Sigmoid vs Softmax: https://web.stanford.edu/~nanbhas/blog/sigmoid-softmax/

