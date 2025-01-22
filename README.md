# Sentiment Analysis On Movie Reviews

## Table of Contents
- [Description](#description)
- [Models Used](#models-used)
- [Key Features](#key-features)
- [Setup and Installation](#setup-and-installation)
- [Usage Guide](#usage-guide)
- [Results](#results)

## Description
This project uses the IMDB dataset to train and evaluate deep learning models for binary sentiment classification. Text preprocessing includes tokenization, padding sequences, and incorporating pre-trained GloVe embeddings to represent words as dense vectors.

The final **ensemble model** combines predictions from three architectures using weighted averaging, ensuring that models with higher accuracy contribute more to the final predictions.

## Models Used
1. **MLP (Multilayer Perceptron)**:
   - Uses pre-trained GloVe embeddings for word representations.
   - Fully connected layers with dropout regularization to prevent overfitting.

2. **LSTM (Long Short-Term Memory)**:
   - Captures sequential dependencies in the text using an LSTM layer.
   - Randomly initialized embeddings are learned during training.

3. **GRU (Gated Recurrent Unit)**:
   - Similar to LSTM but uses GRU layers for efficiency while maintaining performance.

## Key Features
- **Weighted Ensemble**: Combines predictions from all models using weighted averaging.
- **IMDB Dataset**: A standard dataset for binary sentiment classification.
- **Pre-trained Embeddings**: GloVe embeddings enhance the textual data representation.
- **Evaluation**: Ensemble model achieves **93.8% accuracy** on the test set.

## Setup and Installation
Install the required dependencies:

- pip install datasets
- pip install tensorflow
- pip install scikit-learn
- pip install numpy
- pip install scipy

Download **glove.6B.300d.txt** file at: https://www.kaggle.com/datasets/thanakomsn/glove6b300dtxt?resource=download

## Results
The final ensemble model has achieved an accuracy of 93.8% in classifying sentiments as positive or negative using the IMDB dataset.
