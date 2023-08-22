# Overfitting and Underfitting

## Topics covered in today's module
* Overfitting
* Underfitting
* Data preparation
* Reducing network capacity

## Main takeaways from doing today's assignment
- Overfitting - good fit of model on training but does not generalize well to unseen data (learns noise)
  - too many params - not robust to noise and fluctuations in trained data
  - Solutions:
      - Remove layers or reduce neurons in hidden layers
      - Apply regularization - add penalty to loss functin (L1 or L2)
      - Dropout Layers
- Underfitting - data model is unable to capture relationship b/w input and output, generating high error rate on training set and test set
    - not enough params to capture trends in underlying system 
- Helper functions via regular expressions
  - extract email addresses, phone numbers, dates using stopwords
  - df.duplicated().any() checks for duplicated sample feature values
  - df.isnull().sum() determines how many sample features have empty values
- history: model training history
- Data cleansing
  - good to randomly shuffle samples before splitting so classes are equally distributed
  - Tokenize for NLP tasks and sentiment analysis
  - 

## Challenging, interesting, or exciting aspects of today's assignment
I had no idea what regex was before we started the sentiment analysis task for the tweets so learning about regular expressions was interesting and I'd like to experiment more with their capabilities for searching. I would also like to investigate how to adjust my DL model so that it does not overfit. I was excited when the terms bias and variance from my AP stat class showed up in the google colab notebook and reminded me of sampling bias. 

## Additional resources used 
helper functions for data cleansing: https://medium.com/bitgrit-data-science-publication/data-cleaning-with-python-f6bc3da64e45
Regex: https://www.w3schools.com/python/python_regex.asp
Regularization: https://towardsdatascience.com/regularization-in-machine-learning-76441ddcf99a
