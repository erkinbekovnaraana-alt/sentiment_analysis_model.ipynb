# Sentiment Analysis Model — Text Classification using Machine Learning

## Overview

This project implements a basic sentiment analysis model that classifies text as **positive** or **negative** using machine learning techniques.

The goal is to demonstrate how natural language can be transformed into numerical features and used to train a predictive model.

---

## Problem Statement

Understanding sentiment in text is a key task in natural language processing (NLP), widely used in:

* customer feedback analysis
* social media monitoring
* product reviews

This project aims to answer:

* Can we automatically classify text sentiment?
* How can text data be converted into features for machine learning?

---

## Data

A small labeled dataset was created manually:

* Positive examples:

  * "I love this product"
  * "This is amazing"
  * "I am very happy"

* Negative examples:

  * "I hate this"
  * "This is bad"
  * "Very плохой продукт"

Each text is labeled as:

* `1` → Positive
* `0` → Negative

---

## Methodology

### 1. Text Vectorization

Text data was converted into numerical form using:

* Bag-of-Words approach via `CountVectorizer`

This transforms each sentence into a vector representing word frequencies.

---

### 2. Model Training

A Logistic Regression model was used to:

* learn patterns between words and sentiment
* classify unseen text

---

### 3. Prediction

The trained model was tested on new examples:

* "I love it" → Positive
* "This is bad" → Negative

---

## Results

The model successfully classified test sentences:

```id="1a9x2k"
Predictions: [1 0]
```

This shows that even a simple model can capture basic sentiment patterns.

---

## Key Insights

* Text can be effectively converted into numerical features using vectorization
* Logistic Regression performs well on simple classification tasks
* Even small datasets can demonstrate core NLP concepts

---

## Tech Stack

* Python
* Pandas
* Scikit-learn (`CountVectorizer`, `LogisticRegression`)

---

## Limitations

* Very small dataset (not suitable for real-world use)
* Limited vocabulary understanding
* Does not capture context or sarcasm

---

## Future Improvements

* Use larger, real-world datasets
* Apply advanced models (e.g., Hugging Face Transformers)
* Implement preprocessing (stemming, stopwords removal)
* Evaluate model using accuracy, precision, recall
* Deploy as a web app using Streamlit

---

## Repository Structure

```id="k2l9mn"
sentiment-analysis/
│
├── sentiment_analysis_model.ipynb
├── README.md
```

---

## 👤 Author

Independent project demonstrating foundational skills in natural language processing and machine learning.
