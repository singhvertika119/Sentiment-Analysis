# Twitter Sentiment Analysis with TensorFlow

This project demonstrates Sentiment Analysis on Twitter posts using the Sentiment140 dataset and a Recurrent Neural Network (RNN/LSTM) built with TensorFlow/Keras.

We classify tweets into three categories:

- 😀 Positive

- 😐 Neutral

- 😡 Negative

## Dataset

We use the Sentiment140 dataset, which contains 1.6 million tweets labeled for sentiment.

Columns in the dataset:
- sentiment → (0 = negative, 2 = neutral, 4 = positive)

- tweet → raw tweet text

For this project, we map labels to:

- 0 → Negative

- 1 → Neutral

- 2 → Positive

## Model Workflow

- Load Dataset
- Load Sentiment140 CSV and extract sentiment + tweet text.
- Preprocessing
- Clean tweets (remove mentions, hashtags, URLs, emojis).
- Tokenize text and pad sequences.
- Model (RNN with LSTM/GRU)
- Embedding Layer
- LSTM/GRU Layers
- Dense + Softmax Output
- Training
- Train the model on 1M+ tweets with categorical cross-entropy loss.
- Evaluation
- Prediction