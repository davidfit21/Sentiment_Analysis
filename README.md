# Sentiment Analysis Using Deep Learning Methods

**Description**
----------------------
The project uses the IMDB dataset to train and evaluate deep learning models. Text preprocessing includes tokenization, padding sequences, and incorporating pre-trained GloVe embeddings to represent words as dense vectors. The processed text data is fed into three distinct deep learning models, each designed with unique architectures to capture different aspects of the data.

The final ensemble model combines the predictions of each architecture using weighted averaging, where weights are assigned based on individual model performance. This ensures that models with higher accuracy contribute more to the final predictions. The ensemble output is then converted into binary labels to evaluate overall performance.

**Models Used**
-------------------
1. MLP Model:
Uses pre-trained GloVe embeddings for word representations.
Employs fully connected layers with dropout regularization to prevent overfitting.

2. LSTM Model:
Incorporates an LSTM layer to capture sequential dependencies in the text.
Randomly initialized embeddings are learned during training.

3. GRU Model:
Similar to the LSTM model but uses GRU layers for sequence modeling.
Provides computational efficiency while maintaining performance.

**Key Features**
-----------------------------------

Weighted Ensemble: Combines predictions from all models using weighted averaging. Models with higher performance influence the ensemble predictions more significantly.

IMDB Dataset: A standard dataset for binary sentiment classification.

Pre-trained Embeddings: GloVe embeddings are used to enhance the representation of textual data.

Evaluation: The ensemble model's performance is evaluated using accuracy on the test set.
