# CIFAR-10-image-classification
Deep Neural Network (DNN) and Convolutional Neural Network (CNN) trained to classify image data into 10 categories from the CIFAR-10 dataset.

## Abstract
This paper explores the performance of Deep Nerual Netorks (DNNs) and Convolutional Neural
Networks (CNNs) at object identification in images. Several regularization techniques are
implemented to understand their effects on model development. This research uses the
CIFAR-10 dataset containing 60,000 32x32 color images across 10 categories. TensorFlow and
Keras are used to build the models. The best performing model of this research has 2
convolutional (128, 256 nodes) / max pooling layers and a dense layer (384 nodes). It ran for
1m59s and has a testing accuracy of 75% and loss of 0.74. The loss curves show an appropriate
fitting model and confusion matrix shows an accurate classification of images to their lbeled
classes.

## Methods
This research is conducted using the CIFAR-10 dataset, which is split into 45,000 images for
training, 5,000 for validation, and 10,000 for testing. The main libraries are Tensorflow (v
2.18.0), Keras (v 3.8.0), matplotlib, and scikit-learn libraries. In each experiment, one
hyperparameter is tweaked to find a model with the best accuracy and loss score, and correct
classification of the images with the labelled class. All models are run for 50 epochs in batch size
of 64 with the ReLu activation function. Adam is used as the optimizer and Sparse Categorical
Cross Entropy is used for loss. All Conv2D layers have a kernel size of (3,3), strides of 1and
MaxPooling2D layers have a pool size of (2,2), strides of 2.

The images in this dataset are rescaled to between 0 - 1 by dividing them by 255. The accuracy
and loss for training, validation, and testing, confusion matrix are calculated and visualized with
matplotlib. The filter output from the max pooling layers in Experiment 3 is also visualized with
matplotlib to see which features of the image are being picked up by the filters. The
classification report is constructed using scikit-learn.

13 models trained and compared
