# Cats and Dogs: OpenCV and CNN

Cats and Dogs dataset has images of different sizes. All images are not of same size, so it requires resizing so that it would be easy to train similar sized images in CNN.

OpenCV is used in this notebook for cropping, changing RGB colors of the image and grayscale image to see the performance of image.

Implemented two models:
1. Output layer with softmax activation function and 2 output units
2. Output layer with sigmoid activation function and 1 output unit

Softmax function is used for multi class classification, while sigmoid function is used for binary classification. Here the problem have binary classification, so we can check that which model is performing best. There are also some problems of overfitting was seen.

Techniques to prevent Overfitting:

1. Early Stopping: In this method, we track the loss on the validation set during the training phase and use it to determine when to stop training such that the model is accurate but not overfitting.

2. Image Augmentation: Artificially boosting the number of images in our training set by applying random image transformations to the existing images in the training set.

3. Dropout: Removing a random selection of a fixed number of neurons in a neural network during training.
