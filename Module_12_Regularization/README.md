# Regularization

## Topics covered in today's module
* L1/L2 Regularization
* Dropout
* Overfitting
* Underfitting

## Main takeaways from doing today's assignment
- The simplest, more 'correct' DL model is one where the distribution of parameter values has less entropy or less parameters
- prevent overfitting by forcing weights to assume small values - weight regularization
  - L1 regularization - absolute value of weights coef is added to cost
    - push towards zero (abs value function has four corners)
  - L2 regularization - square of value of weights coef - weight decay
    - penalize weights without making them sparse
  - Lambda value comes before regularization penalty
  - Dropout layers
  - Data augmentation and batch normalization
- prevent underfitting by increasing paramaters or order of model
    - train for more epochs and ensure loss is gradually decreasing
    - shuffle data after every epoch 
## Challenging, interesting, or exciting aspects of today's assignment
I have to research more on data augmentation and batch normalization but from what I've heard it just means creating modified copies of an existing sample (rotation, cropping, adding noise or blur), and normalizing activation vectors from hidden layers w/ mean and variance respectively. I also had no idea why L1 or L2 was preferred over the other until I saw the visualizations of the penalty term. I still don't understand why L1 looks like a diamond more than an unfinished inverted triangl. 

## Additional resources used 
Batch Normalization: https://towardsdatascience.com/batch-normalization-in-3-levels-of-understanding-14c2da90a338
L1 and L2 visualization: https://towardsdatascience.com/visualizing-regularization-and-the-l1-and-l2-norms-d962aa769932
