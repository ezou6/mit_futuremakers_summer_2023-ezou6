# Optimization Functions

## Topics covered in today's module
* Gradient Descent
* Mini-batch
* Hyperparamaters
* Cost Function

## Main takeaways from doing today's assignment
- Optimization is the process of comparing items and selecting the best one based on a metric - min. vs. max.
  - Minimize loss, maximize accuracy - update weights and biases
  - Computational complexity prevents us from finding an analytical solution in a reasonable amt. of time to optimizing loss
- Graident descent - forms basis of other optimizers momentum, RMSprop and Adam
-   to update parameters, scale gradient by learning rate for each parameter and subtract it from corresponding parameter
    - Batch size of n: using all of the training examples for each epoch is known as BGD -> most accurate estimate of gradient but takes too long  and not compatible w/ online learning (get new examples during training)
    - SGD uses batch size of n = 1 -? noisy estimate, not garaunteed for global minima but can prevent overfitting and much less computing memory
    - Batch size of 1<n<all is Mini-batch GD - almost always use in DL and in multiples of 2, 4 or 8
- Learning rate - high can overshoot but low will never reach minima
- Cost-function - aka loss function (tell us how good the model is at predicting and update parameters accordingly)
- Keras provides reasonable default values for hyper-params
- Adam appears to be the best optimizer algorihtim for minimizing loss consistently 
  - Adagrad and adadelta are pretty fast to converge too
- Momentum accelerates convergence by taking exponentially weighted averages of past gradients
  
## Challenging, interesting, or exciting aspects of today's assignment
There are so many optimizers to choose from that it's hard to decide which one suits a DL task the best. I thought every algorithim only used simple gradient descent, but was pleasantly surprised. I would still like to better understand Adam and what 'moving averages' are, as well as momentum and their limitations.

## Additional resources used 
Adam optimization: https://machinelearningmastery.com/adam-optimization-algorithm-for-deep-learning/
Momentum: https://medium.com/@vinodhb95/momentum-optimizer-6023aa445e18
Differentiating b/w Batch optimizers: https://towardsdatascience.com/batch-mini-batch-stochastic-gradient-descent-7a62ecba642a

