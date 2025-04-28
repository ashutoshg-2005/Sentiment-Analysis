

# Sentiment Analysis on IMDb Dataset using LSTM

## Overview
This project builds a Sentiment Analysis model to classify movie reviews as positive or negative using Recurrent Neural Networks (RNN), specifically an LSTM architecture. The model is trained on the IMDb Movie Reviews dataset.

## Dataset
**IMDb Dataset**:  
The dataset consists of movie reviews along with their sentiment labels (positive or negative). It is a widely used dataset for binary sentiment classification.

The dataset is preprocessed to:
- Tokenize the reviews.
- Pad sequences to ensure uniform length.
- Convert words to word embeddings using GloVe pre-trained embeddings.

## Model Architecture
The model is built using a Long Short-Term Memory (LSTM) network to classify the sentiment of movie reviews.

- **Embedding Layer**: Initialized with pre-trained GloVe embeddings (dimension: 100), non-trainable.
- **LSTM Layer**: The LSTM layer processes the sequence of word embeddings.
- **Dense Layer**: A fully connected layer with a sigmoid activation for binary classification (positive/negative).

## Results
The following graph shows the model loss over the training epochs for both the training and validation sets:

**Final Accuracy:**
- Training accuracy: 85.4%
- Validation accuracy: 85.2%

**Loss:**
- Training loss decreased significantly after a few epochs.
- Validation loss closely follows training loss, indicating good generalization.

**Evaluation Metrics:**
- Accuracy: 85.2%
- Precision: 85.6%
- Recall: 84.8%
- F1-score: 85.3%

## Conclusion
The LSTM model is able to classify movie reviews into positive and negative classes with a reasonable level of accuracy, as indicated by the training and validation metrics. The loss graph shows that the model is well-optimized without significant overfitting.

## Future Improvements
1. Experiment with trainable embeddings instead of frozen GloVe embeddings.
2. Use bidirectional LSTMs or attention mechanisms to further improve the accuracy.
3. Incorporate early stopping to prevent overfitting.

## Run on Google Colab
You can run and explore this project here:  
[Open in Google Colab](https://colab.research.google.com/drive/1I-VPRy_3OwPYZMRd5lEMAsQ6V8oKAjMl?usp=sharing)

## License
This project is licensed under the MIT License.

