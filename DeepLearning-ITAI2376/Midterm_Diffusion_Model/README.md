# Generative AI: Probabilistic Diffusion Model from Scratch

## Problem Statement
Generative Artificial Intelligence has transformed the technological landscape, with Diffusion Models driving state-of-the-art systems like Midjourney, DALL-E, and Sora. This midterm project aimed to demystify these complex systems by building and training a probabilistic diffusion model entirely from scratch. The objective was to generate high-fidelity, recognizable images of handwritten digits (MNIST) starting from pure Gaussian noise.

## Approach and Methodology
The project required implementing the complete mathematical and architectural lifecycle of a Denoising Diffusion Probabilistic Model (DDPM):
1. **Forward Diffusion Process:** Implemented the mathematical formulation to systematically inject Gaussian noise into clean images over a series of predefined timesteps, effectively destroying the data distribution.
2. **U-Net Architecture:** Engineered a deep Convolutional U-Net architecture from the ground up using PyTorch. This network was designed to predict and subtract the injected noise at any given timestep.
3. **Sinusoidal Positional Embeddings:** Integrated time embeddings into the U-Net so the model could condition its denoising predictions based on the specific timestep of the diffusion process.
4. **Reverse Diffusion (Generation):** Developed the sampling algorithm to iteratively denoise pure random noise, step-by-step, until a coherent image emerged from the latent space.

## Results and Evaluation
- Successfully trained the DDPM on the MNIST dataset using PyTorch and GPU acceleration.
- The model demonstrated a profound understanding of the data distribution, consistently generating clear, recognizable digits from complete static.
- Visualized the generative process through sequential image grids, showcasing the model's ability to iteratively construct structure from noise.

## Learning Outcomes
- Demonstrated advanced capabilities in PyTorch, including designing complex architectures (U-Net) and managing tensor operations.
- Gained a deep, mathematical understanding of Generative AI, Markov chains, and probabilistic models.
- Showcased the ability to implement cutting-edge AI research papers into functional, readable, and highly performant code.

## Dependencies and Data
- **Languages & Frameworks:** Python, PyTorch, Torchvision, Einops, Matplotlib, tqdm.
- **Dataset:** MNIST (Handwritten Digits).
