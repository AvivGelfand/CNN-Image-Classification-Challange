# Convolutional Neural Networks (CNN) - CIFAR-10 Classifier

Welcome to the Convolutional Neural Networks (CNN) CIFAR-10 Classifier project. This README file will guide you through the essentials of this project, its purpose, and the code provided.
1. [The Essence of CNNs](#the-essence-of-cnns)
2. [Data Set - CIFAR-10](#data-set---cifar-10)
3. [Getting Started](#getting-started)
   - [Setting up the Environment](#setting-up-the-environment)
4. [Regular Neural Network (NN)](#regular-neural-network-nn)
5. [Convolutional Neural Network (CNN)](#convolutional-neural-network-cnn)
6. [Model Comparison](#model-comparison)
7. [Visualizing Predictions](#visualizing-predictions)
8. [Conclusion](#conclusion)

![Gelfandar CNN](https://github.com/AvivGelfand/Image-Processing/assets/63909805/c1313b51-07c1-4659-887d-6ffbb345fb7b)

<img width="670" alt="Screenshot 2023-10-14 185103" src="https://github.com/AvivGelfand/Image-Processing/assets/63909805/69696ed4-a7e1-4d76-8049-1ec2a5d19435">

## The Essence of CNNs

Convolutional Neural Networks are a class of deep learning models specifically designed for processing and classifying visual data, such as images. They are highly effective at capturing local and global patterns within images. Here's a brief overview of the key components:

1. **Convolutional Layers:** These layers scan the input image using small filters or kernels, capturing local features and patterns. This operation is crucial for identifying complex image structures.

2. **Pooling Layers:** Pooling layers reduce the spatial dimensions of the data, making the network more robust to variations in position and scale. Max-pooling, for instance, selects the maximum value in a local region, helping to down-sample the data.

3. **Fully Connected Layers:** These layers perform the actual classification or regression tasks, similar to classical neural networks.

The hierarchical structure of CNNs enables them to understand complex image structures, making them ideal for image classification tasks.

## Data Set - CIFAR-10

The CIFAR-10 dataset consists of 60,000 32x32 color images across ten distinct classes, including airplanes, cars, birds, cats, deer, dogs, frogs, horses, ships, and trucks. Each class has 6,000 images. CIFAR-10 is a labeled subset of the larger 80 million tiny images dataset and was collected by Alex Krizhevsky, Vinod Nair, and Geoffrey Hinton.

Source: [CIFAR-10 on Wikipedia](https://en.wikipedia.org/wiki/CIFAR-10)

## Getting Started

The provided code includes two different models: a regular Neural Network (NN) and a Convolutional Neural Network (CNN). The primary objective is to classify images from the CIFAR-10 dataset using these models.

### Setting up the Environment

To get started, make sure you have the necessary libraries and dependencies installed. The code uses TensorFlow, which can be installed using `pip`:

```bash
pip install tensorflow
```

### Regular Neural Network (NN)

The regular Neural Network (NN) model is implemented as follows:

- It uses dense layers with ReLU activation functions.
- Dropout layers are added to prevent overfitting.
- The model is compiled with the Adam optimizer and sparse categorical cross-entropy loss.
- Training is performed for 10 epochs with a batch size of 60.

### Convolutional Neural Network (CNN)

The Convolutional Neural Network (CNN) model is designed to provide better performance:

- Convolutional and max-pooling layers are used to capture local features and down-sample the data.
- Dropout layers are added to prevent overfitting.
- The model is compiled with the Adam optimizer and sparse categorical cross-entropy loss.
- Training is performed for 10 epochs with a batch size of 50.

### Model Comparison

After training both models, the code provides classification reports for both the training and test datasets. These reports include metrics such as precision, recall, and F1-score for each class. The CNN model is expected to outperform the NN model, as it is better suited for image classification tasks.

### Visualizing Predictions

The code also includes a section for visualizing predictions made by the CNN model on the test dataset. It displays a selection of images along with their predicted and true labels. Correctly classified images are labeled in green, while incorrectly classified images are labeled in red.

## Conclusion

In this project, you have explored the use of Convolutional Neural Networks (CNNs) for image classification on the CIFAR-10 dataset. The CNN model demonstrated superior performance to the regular Neural Network, underlining the importance of CNNs in image-related tasks.

Feel free to explore and experiment with the code to gain a deeper understanding of CNNs and their applications in image classification.

