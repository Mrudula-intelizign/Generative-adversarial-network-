# Generative Adversarial Network (GAN)

A **Generative Adversarial Network (GAN)** is a type of deep learning model used to **generate realistic data** by learning the underlying distribution of a dataset.

## Dataset
- **MNIST**: Handwritten digits dataset with 70,000 grayscale images of size 28x28.  
- Used for training the GAN to generate new digit images similar to the MNIST dataset.

## How GANs Work

A GAN consists of **two neural networks** that compete with each other:

### 1. Generator
- Takes **random noise** as input.
- Generates **fake samples** resembling the real data.
- Trained to **fool the discriminator**.

### 2. Discriminator
- Takes input samples (real or fake).
- Outputs the probability that a sample is **real**.
- Trained to **distinguish real from fake**.

### 3. Training Process
1. Generator produces fake data from random noise.
2. Discriminator evaluates both real and fake data.
3. Generator improves by trying to **fool the discriminator**.
4. Discriminator improves by trying to **correctly identify real and fake samples**.


## Applications
- Image generation (e.g., digits, faces, fashion, art)  
- Image-to-image translation (e.g., sketch → photo)  
- Data augmentation  
- Video generation and super-resolution
