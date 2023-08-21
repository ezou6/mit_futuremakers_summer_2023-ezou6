# Classification Loss Functions

## Topics covered in today's module
* Kullback Leibler Divergence Loss
* Binary Cross-Entropy
* Categorical Cross-Entropy
* Sparse Categorical Cross-Entropy

## Main takeaways from doing today's assignment
- KDL measures how a distribution varies from a reference distribution (relative entropy)
    - a KDL loss of 0 means identical prob. distributions
- Cross Entropy - calculate the diff. b/w two prob. distributions by using entropy
    - calculate total entropy b/w distributions
    - Related to log loss - interchangeable in classification models
    - Binaru cross entropy - binary classification w/ two choices (0 and 1) or multi-label classification (binary image segmentation)
        -Used in one-hot encoding 
    - Categorical cross entropy - multi-class classification
        - Also uses one-hot encoding [0.2, .75, .05] vs. [0,1,0]
    - Sparse Categorical Cross Entropy - but y-true are integers instead of one-hot encoding
    - y-pred is always a value between 0 and 1 

## Challenging, interesting, or exciting aspects of today's assignment
I have no idea what entropy is since I'm not familiar with information theory so I had a hard time digesting the difference between KDL and cross entropy. In addition, it was difficult to figure out what the cross entropy loss functions would return by just looking at the formulas and trying to plug in y-hat and y-true.

## Additional resources used 
- Cross Entropy: https://www.youtube.com/watch?v=6ArSys5qHAU&ab_channel=StatQuestwithJoshStarmer (StatQuest)
- Binary Cross Entropy Formula Explained and Math: https://medium.com/analytics-vidhya/binary-crossentropy-in-its-core-35bcecf27a8a
