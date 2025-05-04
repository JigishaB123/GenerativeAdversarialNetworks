# Generative Adversarial Network (GAN) on MNIST using PyTorch

This project implements a simple Generative Adversarial Network (GAN) using PyTorch to generate handwritten digits similar to those found in the MNIST dataset. It includes code for training the generator and discriminator networks, visualizing generated samples, and saving model checkpoints.

## 📌 Overview

A GAN consists of two neural networks:

- **Generator**: Tries to generate realistic data from random noise.
- **Discriminator**: Tries to distinguish between real and fake data.

These two models are trained in a zero-sum game where the generator tries to fool the discriminator, and the discriminator improves at detecting fakes.

## 🧠 Model Architecture

- **Generator**: A feedforward neural network that maps a 100-dimensional latent vector to a 784-dimensional image (28x28).
- **Discriminator**: A neural network that takes a 784-dimensional image and outputs a probability score representing real/fake.

## 🗂️ Project Structure

```bash
gan.ipynb              # Main Jupyter Notebook implementing and training the GAN
README.md              # Project documentation
```

## 🛠️ Requirements

To run this project, you will need the following Python packages:

- Python 3.x

- PyTorch

- torchvision

- matplotlib

- numpy

## 🏃 How to Run
1. Clone the repository or download the notebook.

2. Open `gan.ipynb` using Jupyter Notebook or Google Colab.

3. Run all cells to train the GAN. Generated samples are visualized after each epoch.

## 📊 Training Details
- Dataset: MNIST 
- Optimizer: Adam
- Loss Function: Binary Cross-Entropy
- Batch Size: 100
- Latent Vector Size: 100
- Training Epochs: Configurable (default: 50)