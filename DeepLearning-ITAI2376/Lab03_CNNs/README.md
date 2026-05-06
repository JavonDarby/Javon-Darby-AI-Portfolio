# CNNs for Image Classification: Puppy or Bagel?

## Problem Statement
Computer Vision has revolutionized how machines interact with the world, but models often struggle with visually similar textures and shapes. This project tackles a classic, humorous computer vision challenge inspired by a viral meme: distinguishing between curled-up puppies and bagels. The goal is to build, train, and optimize Convolutional Neural Network (CNN) architectures capable of accurately classifying these highly similar images.

## Approach and Methodology
The project progressed from fundamental CNN architecture design to advanced transfer learning techniques:
1. **Custom CNN Architecture:** Built a CNN from scratch using TensorFlow and Keras, implementing convolutional layers, max-pooling layers, flatten layers, and dense fully-connected layers to extract hierarchical features from the images.
2. **Data Augmentation:** Implemented `ImageDataGenerator` to dynamically augment the dataset (rotations, shifts, flips, and zooms), effectively expanding the training data and improving the model's ability to generalize to unseen images.
3. **Transfer Learning:** Leveraged state-of-the-art pre-trained models, specifically ResNet50 and MobileNetV2, utilizing their pre-learned feature extraction capabilities on the ImageNet dataset.
4. **Fine-Tuning:** Unfroze the top layers of the pre-trained models and fine-tuned the weights specifically for the "Puppy vs. Bagel" binary classification task.

## Results and Evaluation
- The custom CNN established a strong baseline performance on the validation set.
- The application of Transfer Learning via MobileNetV2/ResNet50 significantly accelerated convergence and achieved superior accuracy, demonstrating the power of leveraging pre-trained weights for specialized tasks.
- Evaluated models using comprehensive metrics including Confusion Matrices and Classification Reports (Precision, Recall, F1-Score).

## Learning Outcomes
- Developed expertise in Convolutional Neural Networks for Computer Vision tasks.
- Mastered the application of Transfer Learning and Fine-Tuning to achieve high performance on limited datasets.
- Gained practical experience in handling, organizing, and augmenting custom image datasets using Python and TensorFlow.

## Dependencies and Data
- **Languages & Frameworks:** Python, TensorFlow, Keras, Matplotlib, Scikit-Learn.
- **Dataset:** "Puppy or Bagel" Dataset (Binary Classification).
