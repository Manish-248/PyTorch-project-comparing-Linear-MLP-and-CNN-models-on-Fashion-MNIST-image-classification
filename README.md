# PyTorch-project-comparing-Linear-MLP-and-CNN-models-on-Fashion-MNIST-image-classification
PyTorch project comparing Linear, MLP, and CNN models on Fashion-MNIST image classification.
# Fashion-MNIST Neural Network Image Classification Project

## Project Overview

This project builds, trains, and compares three different neural network architectures for image classification using the public **Fashion-MNIST** dataset.

Fashion-MNIST is a computer vision dataset containing grayscale images of clothing items such as shirts, shoes, bags, coats, and trousers. Each image is 28x28 pixels and belongs to one of 10 classes.

The goal of this project is to understand how different neural network architectures perform on the same image classification task.

---

## Project Objectives

The main objectives of this project are:

- Load and explore a public image dataset
- Visualize sample images from the dataset
- Build neural networks using PyTorch
- Train three different model architectures
- Compare model performance using accuracy and loss
- Understand why CNNs are usually better for image recognition
- Save the best model
- Prepare the project for GitHub documentation

---

## Dataset

The project uses the **Fashion-MNIST** dataset from `torchvision.datasets`.

Fashion-MNIST contains:

- 60,000 training images
- 10,000 testing images
- 10 image classes
- Image size: 28 x 28 pixels
- Grayscale images

### Classes

The dataset includes the following categories:

1. T-shirt/top
2. Trouser
3. Pullover
4. Dress
5. Coat
6. Sandal
7. Shirt
8. Sneaker
9. Bag
10. Ankle boot

---

## Models Compared

This project compares three neural network architectures.

### 1. Linear Baseline Model

The first model is a simple linear classifier.

It flattens each 28x28 image into a vector of 784 pixel values and sends it directly to a linear output layer.

This model is useful as a baseline because it helps us understand the minimum performance level.

### 2. Multi-Layer Perceptron

The second model is a fully connected neural network with hidden layers and ReLU activation functions.

This model can learn more complex patterns than the linear baseline, but it still treats the image as a flat vector and does not understand spatial relationships between pixels.

### 3. Convolutional Neural Network

The third model is a convolutional neural network.

CNNs are designed for image data. They use convolutional layers to learn local patterns such as edges, shapes, and textures.

This model is expected to perform better than the first two models because it preserves and learns from the spatial structure of images.

---

## Technologies Used

- Python
- PyTorch
- Torchvision
- Matplotlib
- Pandas
- Jupyter Notebook / Google Colab

---

## Project Structure

```text
fashion-mnist-neural-network-project/
│
├── fashion_mnist_three_architectures.ipynb
├── README.md
├── requirements.txt
└── models/
    └── fashion_mnist_cnn_model.pth
