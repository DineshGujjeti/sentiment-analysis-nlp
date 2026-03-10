# Sentiment Analysis using Natural Language Processing

This project performs **Sentiment Analysis** on text data to classify whether a review or tweet expresses a **Positive** or **Negative** sentiment.  
It uses Natural Language Processing (NLP) techniques and a machine learning model to analyze text and predict sentiment.

---

## Project Overview

Sentiment Analysis is widely used in:

- Customer feedback analysis
- Product review evaluation
- Social media monitoring
- Market research

This project processes text data, cleans it using NLP techniques, and trains a machine learning model to classify sentiments.

---

## Technologies Used

- Python
- Pandas
- NumPy
- NLTK
- Scikit-learn
- TF-IDF Vectorizer
- Logistic Regression

---

## Dataset

The model is trained using a dataset of tweets/reviews labeled with sentiment values.

Sentiment labels:

- **0 → Negative**
- **1 → Positive**

---

## Workflow

The following steps were performed in this project:

1. Data Loading
2. Data Cleaning and Preprocessing
3. Text Normalization (lowercase, remove special characters)
4. Stopword Removal using NLTK
5. Feature Extraction using TF-IDF Vectorizer
6. Train-Test Split
7. Model Training using Logistic Regression
8. Model Evaluation and Prediction

---

## Model Evaluation

The model performance is evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score

---

## Example Prediction

Input Review: This phone is amazing and works perfectly!

Prediction: Positive

Input Review: Worst product I have ever bought.

Prediction: Negative

---

## Applications

- Customer sentiment monitoring
- Brand reputation analysis
- Product review analysis
- Social media sentiment tracking

---

## Future Improvements

- Try advanced models like Support Vector Machines
- Use Deep Learning (LSTM or BERT)
- Deploy as a web application

---
