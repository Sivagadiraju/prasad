NAME: SIVA SATHYA VARA PRASAD RAJU GADIRAJU ID.NO: 700756448


# MNIST GAN - Handwritten Digit Generation with PyTorch

This project implements a **Generative Adversarial Network (GAN)** using PyTorch to generate realistic handwritten digits based on the MNIST dataset.

## 📌 Features
- Generator and Discriminator neural network models
- Training loop with alternating updates between Generator and Discriminator
- Visualization of loss curves
- Sample images saved at epochs 0, 50, and 100

## 🧠 Model Architecture

### Generator
- Input: Random noise vector (latent_dim = 100)
- Fully connected layers with ReLU activations
- Output: 28x28 image (reshaped from 784 output with Tanh)

### Discriminator
- Input: Flattened 28x28 image
- Fully connected layers with LeakyReLU
- Output: Probability score (Sigmoid)

## 🔁 Training Process
1. Train the **Discriminator** to distinguish real MNIST images from fake ones.
2. Train the **Generator** to produce images that fool the Discriminator.
3. Alternate updates over 100 epochs.

## 📊 Output

### Loss Curves
- Generator loss vs. epoch
- Discriminator loss vs. epoch

### Sample Outputs
Generated digit images are displayed at:
- **Epoch 0**: Random noise-like images
- **Epoch 50**: Rough digit-like shapes
- **Epoch 100**: Clear handwritten digits

## 📦 Requirements

Install dependencies with:

```bash
pip install torch torchvision matplotlib
