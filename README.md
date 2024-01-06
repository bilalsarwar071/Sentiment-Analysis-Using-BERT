# Sentiment-Analysis-Using-BERT

This code repository demonstrates sentiment analysis using BERT (Bidirectional Encoder Representations from Transformers). The model is trained on the IMDb dataset for binary sentiment classification (positive or negative).

## Setup

Make sure you have the necessary libraries installed:

```bash
pip install tensorflow torch transformers pandas beautifulsoup4 matplotlib plotly wordcloud scikit-learn
```
In case, you are using Google Colab notebook.

```bash
!pip install tensorflow torch transformers pandas beautifulsoup4 matplotlib plotly wordcloud scikit-learn
```

## Dataset

The IMDb dataset is downloaded and extracted using TensorFlow's utility functions. The dataset contains movie reviews labeled as positive or negative sentiments.

## Data Exploration

Explore the dataset by checking the contents of the train directory and displaying sample reviews with their sentiments.

## Data Cleaning

A cleaning function removes HTML tags, square brackets, and non-alphanumeric characters from the text.

## Visualization

* **Sentiments Counts Bar Chart**: Visualizes the distribution of positive and negative sentiments in the training dataset using Plotly.

* **Word Clouds**: Generates word clouds for positive and negative reviews to visualize frequently occurring words.

## Tokenization and Encoding

The BERT tokenizer is used to tokenize and encode the reviews. The data is split into training, validation, and test sets.

## BERT Model

A BERT-based sequence classification model is initialized and compiled for training. The model is trained on the GPU.

## Model Evaluation

The trained model is evaluated on the test dataset, and test loss and accuracy are reported.

## Model Saving and Loading

The trained model and tokenizer are saved to a specified path for future use.

## Inference

A function (```Get_sentiment```) is provided for predicting sentiments of custom reviews using the trained model.

## Example Usage

A sample positive review of the movie is provided (You can also write yours, and the Get_sentiment function predicts its sentiment.

*Feel free to adapt and use the code for your sentiment analysis tasks!*
