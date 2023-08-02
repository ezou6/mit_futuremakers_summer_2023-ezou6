# Convolution Neural Network

## Topics covered in today's module
* Convolution neural network components
* Visualizing kernels
* Visualizing feature maps
* Pooling
* Dropout
* Batch norm

## Main takeaways from doing today's assignment
- CNNs have local receptive fields and spatially invariant
- Each Convolutional layer has two sets of weights: filter (matrix) and bias
- depth of filter has to match # of channels in input
- Pooling layers reduce spatial dimensions and can prevent overfitting
  - Max pooling = keep max value
- Padding -> fit kernal size with 0s
- Dropout reduces overfiting by reducing reliance on any single feature and forcing the model to generalize
- BN also reduces overiffting by centering mean at 0 and std deviation at 1, 'whitening' data

## Challenging, interesting, or exciting aspects of today's assignment
I'm still confused on batch normalization and how the distribution of outputs within layers woulde xperience internal covariate shift. I'd also like to understand how feature maps are generated and what features they focus on based on the operations done in the convolution and pooling layers. I'd also like to know how the input shape is preserved with many pooling layers. 
## Additional resources used 
Batch Normalization: https://machinelearningmastery.com/batch-normalization-for-training-of-deep-neural-networks/
Padding: https://www.geeksforgeeks.org/cnn-introduction-to-padding/
filter vs. kernel: https://stats.stackexchange.com/questions/154798/difference-between-kernel-and-filter-in-cnn
CNN architecture visualization: https://towardsdatascience.com/convolutional-neural-networks-explained-9cc5188c4939
