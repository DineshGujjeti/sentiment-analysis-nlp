# Sentiment Analysis using Natural Language Processing

This project performs **Sentiment Analysis** on text data to classify whether a review or tweet expresses **Positive** or **Negative** sentiment using Natural Language Processing (NLP) techniques and Machine Learning.

---

## Project Overview

Sentiment analysis is widely used to analyze customer feedback, product reviews, and social media posts.  
This project processes raw text data, applies NLP preprocessing techniques, and trains a machine learning model to predict sentiment.

The model converts text into numerical features using **TF-IDF vectorization** and trains a **Logistic Regression classifier** to perform sentiment classification.

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

The model is trained using a **Twitter sentiment dataset** containing tweets labeled with sentiment.

Sentiment labels:

| Label | Meaning |
|------|------|
| 0 | Positive |
| 1 | Negative |

The dataset is imbalanced, with significantly more positive samples than negative ones.

---

## Handling Class Imbalance

Since the dataset contains more samples from one class, the model was trained using:

```python
LogisticRegression(class_weight='balanced')
```

---

### Machine Learning Pipeline

-Data Loading
-Data Cleaning and Preprocessing
-Text Normalization (lowercase, remove special characters)
-Stopword Removal using NLTK
-Feature Extraction using TF-IDF Vectorization
-Train-Test Split
-Model Training using Logistic Regression
-Model Evaluation using classification metrics
-Custom sentiment prediction

---

## Model Performance

The trained Logistic Regression model achieved the following evaluation results:

| Metric | Score |
|------|------|
| Accuracy | ~92% |
| Macro F1 Score | 0.77 |
| Weighted F1 Score | 0.93 |

### Classification Report

| Class | Precision | Recall | F1 Score | Support |
|------|------|------|------|------|
| Negative | 0.46 | 0.81 | 0.58 | 456 |
| Positive | 0.98 | 0.93 | 0.95 | 5937 |

The model performs strongly in detecting **positive sentiment** while maintaining reasonable detection of **negative sentiment**, despite the dataset being imbalanced.

---

## Example Predictions

Input: I love this product  
Prediction: Positive

Input: I am very happy today  
Prediction: Positive

Input: This is terrible and I hate it  
Prediction: Negative

---

## Applications

- Customer feedback analysis  
- Product review sentiment detection  
- Social media sentiment monitoring  
- Brand reputation analysis  

---

## Future Improvements

- Train additional models such as SVM or Random Forest  
- Implement deep learning models like LSTM or BERT  
- Deploy the model using Streamlit or Flask  

---
