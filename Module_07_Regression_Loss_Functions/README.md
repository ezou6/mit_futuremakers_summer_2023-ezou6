# Regression Loss Functions

## Topics covered in today's module
* Mean Squared Error
* Mean Absolute Error
* Mean Squared Logarithm Error

## Main takeaways from doing today's assignment
- Loss functions measure how far an estimated value is from the true value
  - Regression Loss Functions: L1, L2, Huber loss, Quantile Loss
      - MSE - penalize large errors
      - MAE - measures magnitude of error - more robust to outliers
      - MSLE - take log of actual and estimated w/ squaring
        - Measures relative difference or precentual difference (treat small and big differences the same)
        - 5-4 vs 5000-4000
  - Classification Loss Functions: log loss, exp. loss, hinge loss, relative entropy loss
    

## Challenging, interesting, or exciting aspects of today's assignment
I only knew about MSE and MAE beforehand and was surprised that MSLE was a loss function. I think MSLE is a pretty convenient loss function since it penalizes proportionally for big and small errors, but it may be hard to differentiate when fed into the actual model, and thus the preponderance of MSE being used in DL. I also was confused by the terms huber and quantile loss since I never heard of these functions, but apparently the Huber loss combines the MSE and MAE by setting a delta value.

## Additional resources used 
Huber Loss: https://towardsdatascience.com/understanding-the-3-most-common-loss-functions-for-machine-learning-regression-23e0ef3e14d3

