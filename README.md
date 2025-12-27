# Emotional Classification & Analysis – NLP Project

📌 Project Objective

This project aims to analyze text data and classify the emotions expressed (e.g., joy, sadness, anger, fear, surprise, neutrality) using Natural Language Processing and Machine Learning techniques. The focus is on building a complete pipeline, including preprocessing, modeling, evaluation, and result interpretation.

# 📊 Dataset

Dataset name: Hello-SimpleAI/HC3
Source: Hugging Face
Link: https://huggingface.co/datasets/Hello-SimpleAI/HC3
Model: BERT  nlptown/bert-base-multilingual-uncased-sentiment
Task: rating classification (5 stars)


Format: text + emotion label
Number of samples: more than 20,000 sentences

Split:
Train: 16,000
Validation: 2,000
Test: 2,000

Labels: sadness, joy, love, anger, fear, surprise ect..
License: BSD License

Description

The dataset consists of short sentences annotated with one of six primary emotions.
It is widely used for emotion classification tasks and NLP model benchmarking.
The diversity of the sentences and the balanced label distribution make it suitable for experimentation with both classical machine learning models and transformer-based approaches.

# How it was used in the project

The model was employed to:

- Generate a sentiment score (1–5) for each text

- Convert the score into emotion categories

- Analyze the distribution of emotions in the dataset

# 🔧 Project Pipeline

The implemented NLP pipeline includes the following steps:
1. Text Preprocessing(Lowercasing, Punctuation removal, Stopword removal, Tokenization, Lemmatization)

2. Text Representation
BERT embeddings using the model nlptown/bert-base-multilingual-uncased-sentiment

3. Modeling
- Sentiment inference using the BERT model
- Conversion of the score into emotion categories
- Training a traditional classifier for comparison

4. Evaluation
Metrics used:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion matrix to compare predictions with the original labels

5. Error Analysis
- Identification of the most difficult emotions to classify
- Analysis of ambiguous cases
- Verification of class distribution

6. Results Visualization
- Emotion distribution plot
- Confusion matrix heatmap
- Comparison between actual and predicted labels

