# Sequence Modeling: RNNs vs. Transformers vs. Vision Transformers

## Problem Statement
The landscape of deep learning has shifted dramatically with the introduction of the Transformer architecture, which has largely superseded Recurrent Neural Networks (RNNs) for sequence modeling tasks. This project provides a rigorous, empirical comparison between classical RNNs (LSTMs and GRUs) and modern Transformer models (DistilBERT and Vision Transformers) across both Natural Language Processing (NLP) and Computer Vision domains.

## Approach and Methodology
The comparative analysis was structured into three major components:
1. **Classical Sequence Modeling (RNNs):** Built Bidirectional Long Short-Term Memory (LSTM) and Gated Recurrent Unit (GRU) networks from scratch using PyTorch. Developed a complete NLP preprocessing pipeline, including custom tokenization, vocabulary building, and sequence padding.
2. **Modern NLP (Transformers):** Implemented Hugging Face's `transformers` library to fine-tune a pre-trained DistilBERT model on the exact same text classification task, providing an apples-to-apples comparison against the LSTM/GRU models.
3. **Computer Vision (Vision Transformers):** Extended the Transformer architecture to the vision domain by implementing a Vision Transformer (ViT) on the CIFAR-10 image dataset, comparing its self-attention mechanism to the spatial convolutions of traditional CNNs.

## Results and Evaluation
- **Text Classification (AG News):** The bidirectional LSTM and GRU models successfully learned to categorize news topics, but the fine-tuned DistilBERT model demonstrated vastly superior accuracy and contextual understanding, highlighting the power of self-attention mechanisms.
- **Image Classification (CIFAR-10):** The Vision Transformer (ViT) successfully treated image patches as sequences, proving that Transformer architectures can achieve state-of-the-art results without relying on convolutions.

## Learning Outcomes
- Demonstrated proficiency in PyTorch for building complex sequential models (Bi-LSTM, GRU).
- Mastered the Hugging Face ecosystem (`transformers`, `datasets`) for rapid deployment and fine-tuning of Large Language Models (LLMs) and Vision Transformers.
- Gained a deep architectural understanding of Attention Mechanisms versus Recurrence.

## Dependencies and Data
- **Languages & Frameworks:** Python, PyTorch, Hugging Face Transformers, Hugging Face Datasets.
- **Datasets:** AG News (Text Topic Classification), CIFAR-10 (Image Classification).
