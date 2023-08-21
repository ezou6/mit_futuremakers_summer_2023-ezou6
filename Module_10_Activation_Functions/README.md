# Activation Functions

## Topics covered in today's module
* Introduction to Sigmoid, Tanh, ReLU
* Visualizing how ReLU affects the feature maps
* Vanishing and exploding gradients
* Dying ReLU problem
* Advanced activation functions: Swish, GeLU, SeLU

## Main takeaways from doing today's assignment
- Activation functions determine firing of neurons
-   Should be nonlinear and differentiable - allows us to backpropagate the model's error to optimize weights
  - Sigmoid - squashing function to range of 0 to 1 from domain of all real numbers
  - Tanh - same s-shape as sigmoid but has range of -1 to 1 and domain of all real numbers
  - ReLU - replace sigmoid and tanh in DL hidden layers
    - computation saving - derivate is just constant 1
    - Solves vanishing gradient - really larger or small values in tanh or sigmoid reach asympmtotes and have a gradient close to 0, preventing updates
        - exacerbated by small learning rates and partial derivatives (chain rule) during backpropagation
    - Exploding gradients - if derivatives are too large, gradient increases exp. from output to input
  - Dying ReLU - negative inputs are outputed to 0 and don't activate neuron (not permanently dead if new training data added)
      -Solution 1: Leaky ReLU (multiply negative by an "a" gradient
          - Problem: still doesn't take into account really really negative inputs
      - Solution 2: Exponential Linear Unit (ELU) where a > 0 (gradient)
      - Swish (depth larger than 40 layers), GeLU and SeLU are other variants of ReLU
    

## Challenging, interesting, or exciting aspects of today's assignment
I've heard of ReLU being used in hidden layers instead of Tanh or sigmoid before, but never knew that there were so many variants of ReLU such as Leaky ReLU or ELU or Swish. I still have no idea how these activation functions pick up on the most "salient" features so I'd like to deep dive into the math. The graph of activation functions at the beginning of the Colab notebook is also fascinating to me since half of these functions weren't mentioned such as bipolar ReLU and softplus.

## Additional resources used 
Swish: https://towardsdatascience.com/swish-booting-relu-from-the-activation-function-throne-78f87e5ab6eb
Tanh: https://towardsdatascience.com/activation-functions-neural-networks-1cbd9f8d91d6
zip function: https://www.w3schools.com/python/ref_func_zip.asp
