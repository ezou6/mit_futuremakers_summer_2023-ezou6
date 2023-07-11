# Machine Learning

## Topics covered in today's module

* Introduction to Machine Learning
* Machine learning with Scikit-learn
* Decision Trees
* Linear Regression
* Random Forests

## Main takeaways from doing today's assignment
- Reinforcement learning is based on an agent exploring its environment and receiving feedback in the form of a reward
- Sci-Kit is built off of pandas and numpy libraries
- The Iris data set is a famous ML dataset
- Decision Trees can both be used for classification and regression
    - Consist of nodes and leaf nodes that split into true or false
    - Gini Index is a measure of purity and measures how much more work is        needed to be done in splitting nodes
    - A gini index of .5 means randomly classifying into classes
    - The process for most classifier models seems to be the same: clf =          modelClassifier(), clf = clf.fit(train_data, train_target),                 clf_prediction = clf.predict(test_data), and then I compared                clf_prediction with test_target and all of the datapoints matched up.
- You can render models via graphviz, which converts images into pdfs
- Random Forest is a collection of decison trees that have randomized         features and take a final vote for the most statistically probable class - "averaging" rather than boosting
- Small datasets may come with higher accuracies

## Challenging, interesting, or exciting aspects of today's assignment
I was surprised that all three of my classifier models for the bonus question yielded an accuracy of 100% but the code was reviewed by the head mentors and checked out. I think it's just the small dataset that made predicting so much easier. Also, I struggled with printing the entire ensemble of decision trees for the random forest classifier but apparently we didn't need to. I still tried to enumerate through the random forest but I only received one decision tree. I was surprised that the process for building classifier models only took 3-4 lines of code. 

## Additional resources used 
Differences between random forest and decision trees: https://www.educba.com/random-forest-vs-decision-tree/
RandomForest and Decision Tree Classifiers: https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html
Plot randomforest ensemble: https://stackoverflow.com/questions/70253091/export-plot-random-forest-decision-tree-randomforestclassifier-object-has

