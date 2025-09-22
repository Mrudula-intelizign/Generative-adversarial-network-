# Generative Adversarial Network (GAN)

A **Generative Adversarial Network (GAN)** is a type of deep learning model used to **generate realistic data** by learning the underlying distribution of a dataset.

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

This creates a **minimax game**:

\[
\min_G \max_D V(D, G) = \mathbb{E}_{x \sim p_\text{data}(x)}[\log D(x)] + \mathbb{E}_{z \sim p_z(z)}[\log(1 - D(G(z)))]
\]

Where:  
- \(G\) = Generator  
- \(D\) = Discriminator  
- \(x\) = real data  
- \(z\) = random noise

## Applications
- Image generation (e.g., faces, fashion, art)  
- Image-to-image translation (e.g., sketch → photo)  
- Data augmentation  
- Video generation and super-resolution
