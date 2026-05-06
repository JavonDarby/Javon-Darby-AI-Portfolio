# Neural Network Foundations: From Scratch to Frameworks

## Problem Statement
Understanding the fundamental mathematics and mechanics of neural networks is critical for debugging, optimizing, and deploying deep learning models. This project aims to bridge the gap between theoretical understanding and practical application by implementing a neural network entirely from scratch using raw NumPy, followed by reconstructing the same architecture using modern industry-standard frameworks: PyTorch and TensorFlow/Keras.

## Approach and Methodology
The project was divided into two distinct phases to provide a comprehensive learning experience:
1. **Mathematical Implementation (From Scratch):** Implemented the forward pass, backward pass (backpropagation), activation functions (ReLU, Sigmoid, Softmax), and gradient descent optimization entirely from scratch using Python and NumPy. This phase solidified the understanding of matrix multiplications and the chain rule of calculus in deep learning.
2. **Framework Implementation (PyTorch & TensorFlow):** Rebuilt the network using PyTorch and TensorFlow/Keras to solve the Fashion-MNIST image classification problem. This phase highlighted the efficiency, automatic differentiation, and GPU-acceleration capabilities of modern frameworks.

## Results and Evaluation
- Successfully trained a Multi-Layer Perceptron (MLP) on the Fashion-MNIST dataset.
- Evaluated performance using both PyTorch and TensorFlow/Keras, achieving competitive accuracy scores on the validation and test sets.
- Conducted hyperparameter tuning experiments, systematically analyzing the impact of learning rate, batch size, and epoch count on model convergence and generalization.

## Learning Outcomes
- Demonstrated deep technical knowledge of neural network architecture, extending beyond high-level APIs.
- Gained proficiency in both PyTorch (dynamic computational graphs, research-focused) and TensorFlow/Keras (static/eager execution, production-focused).
- Mastered the ability to diagnose and mitigate overfitting through hyperparameter optimization and regularization techniques.

## Dependencies and Data
- **Languages & Frameworks:** Python, NumPy, PyTorch, TensorFlow, Keras.
- **Dataset:** Fashion-MNIST (70,000 grayscale images of 10 clothing categories).
