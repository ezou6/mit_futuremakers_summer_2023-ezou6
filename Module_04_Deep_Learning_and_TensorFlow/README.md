# Deep Learning and TensorFlow

## Topics covered in today's module
* Linear models in machine learning
* Introduction to TensorFlow
* Dataloaders
* Building a simple Neural Network

**Main Takeaways**
- The XOR data cannot be classified by a linear single-layer perceptron
    - Returns 0 if inputs are the same (0,0 and 1,1) and 1 if inputs are different (0,1 and 1,0)
- reg.score(x,y) returns r^2, reg.coef_ returns the coefficient for each feature and reg.intercept_ returns the bias
- TensorFlow is a python library that specializes in building, training and deploying NNs
- Tensors are multi-dimensional arrays wth a uniform type
- The models.Squential() function creates NNs layer by layer
- tf.keras.layers.Dense() creates a fully connected layer in which every neuron is connected to every neuron in the previous layer
- Our loss function will be binarycrossentropy() for a binary classification NN
- Sigmoid is the output layer's activation function for a binary classifier or multilabel classification
- Softmax is used for multiclass classification
- MNIST is a famous dataset for the application of computer vision in ML
-   consists of 28x28 pixels and each pixel is scaled on a grayscale from 0 to 255
-   each image is labeled 0 to 9 as a class
-   We normalize values by dividing each  pixel value by the largest value it can take on, 255
-   The flatten() function squishes a 2d tensor into a 1d one

**Interesting, challenging, surprising things I learned**
- I struggled in understanding what was was happening when we made predictions using the model trained on the MNIST Fashion dataset. There were functions I never heard of interspersed throughout the functions we created and it was hard to follow what each variable stored. For example, I still can't figure out why we multiplied the columns and rows in the figsize by 2.

  **Additional resources used**
- Dot products and matrix multiplication: https://mathinsight.org/dot_product_matrix_notation
- Matplotlib documentation: https://mathinsight.org/dot_product_matrix_notation
