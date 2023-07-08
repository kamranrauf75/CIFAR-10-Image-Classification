CIFAR-10 Image Classification using k-Nearest Neighbors (k-NN)

This project focuses on implementing the k-Nearest Neighbors (k-NN) algorithm to classify images from the CIFAR-10 dataset. The project involves loading the dataset, visualizing the images, computing distances between training and test examples, and predicting labels for test samples.

Setup:

Before running the code, make sure to install the required packages and libraries. Additionally, adjust the figure size settings for proper visualization.

Loading the CIFAR-10 Dataset:

The CIFAR-10 dataset contains a set of labeled images for classification tasks. To load the dataset, use the 'coutils.data.cifar10()' function, which returns four Torch tensors:
- 'x_train': Contains all training images (real numbers in the range [0,1])
- 'y_train': Contains all training labels (integers in the range [0,9])
- 'x_test': Contains all test images
- 'y_test': Contains all test labels

Visualizing the Dataset:

To get an idea of the images in the CIFAR-10 dataset, a random selection of examples from the training set is visualized using matplotlib.

Computing Distances: Naive Implementation:

The project involves computing distances between training and test examples. The initial implementation uses explicit loops over the training and test sets.

Computing Distances: Vectorization:

To improve the efficiency of computing distances, the project aims to eliminate explicit loops and vectorize the code using PyTorch functions.

Predicting Labels:

To predict labels for test samples, the project implements a function that uses the distances and training labels to find the k nearest neighbors and make predictions.

