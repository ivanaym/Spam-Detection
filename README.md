# Spam Detection in Text Messages
Overview
This repository contains the implementation of various neural network-based methods for detecting spam messages in SMS text. The methods applied include:

Long Short-Term Memory (LSTM)
Bidirectional Long Short-Term Memory (Bi-LSTM)
Gated Recurrent Unit (GRU)
Bidirectional Gated Recurrent Unit (Bi-GRU)
The project aims to build an efficient model to classify SMS messages into two categories: Spam or Ham (not spam). The dataset used for this project was obtained from Kaggle and includes 1143 messages in total, evenly distributed between the two categories.

Models Implemented
1. LSTM
LSTM is a popular recurrent neural network (RNN) architecture designed to model sequence data by capturing long-term dependencies. This model uses two LSTM layers followed by dropout layers to reduce overfitting. A final dense layer with a sigmoid activation function is used to classify SMS messages.

2. Bi-LSTM
Bi-LSTM processes the input data in both forward and backward directions to better capture the context of the words in an SMS message. It includes bidirectional LSTM layers, dropout layers, and a dense layer for binary classification.

3. GRU
GRU is a simplified version of LSTM that includes fewer gates, making it computationally less expensive while still retaining performance. This model also includes two GRU layers with dropout to prevent overfitting.

4. Bi-GRU
Bi-GRU is the bidirectional version of GRU, processing data in both forward and backward directions to capture context. Similar to the other models, it consists of bidirectional GRU layers, dropout layers, and a dense classification layer.

Data
The dataset used for this project consists of 1143 SMS messages:

Spam messages: 574
Ham messages: 569
The data has been preprocessed through several steps:

Case folding: Converting all text to lowercase.
URL and punctuation removal: Removing unnecessary elements like URLs and punctuation.
Stemming: Reducing words to their root forms.
Tokenization: Breaking down the text into individual tokens.
Stopword removal: Eliminating common but unimportant words like "and," "the," etc.

Conclusion
This project demonstrates the use of various neural network architectures to classify SMS messages as either spam or ham. Among the models tested, Bi-LSTM achieved the best results, providing accurate predictions for spam detection. Further improvements can be made by experimenting with different architectures, tuning hyperparameters, or expanding the dataset.
