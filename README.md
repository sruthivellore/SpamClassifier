# Spam Classifier

A simple and practical machine learning project for detecting spam emails.

This notebook walks through building a spam detection system for emails. The goal is to classify emails as either "spam" or "not spam" (ham).

---

## How It Works

- **Data Loading:**  
  The system starts by loading a dataset of emails labeled as spam or not spam.

- **Text Preprocessing:**  
  - Removes special characters and converts text to lowercase.
  - Splits emails into words, removes common stopwords (like "the", "and"), and applies stemming to reduce words to their root form.

- **Feature Extraction:**  
  - Uses the Bag of Words model to turn emails into a matrix of word counts, making them suitable for machine learning.

- **Model Training:**  
  - Several algorithms are tested:
    - Multinomial Naive Bayes
    - Gaussian Naive Bayes
    - Bernoulli Naive Bayes
    - Linear Support Vector Classifier (SVC)
  - Each model is trained on a portion of the data and tested on the rest.

- **Evaluation:**  
  - For each model, the notebook prints out the confusion matrix, accuracy, and a classification report.
  - ROC curves are plotted to visually compare performance.
  - AUC scores are calculated for each model.

---

## Results

- **Accuracy:**  
  The models achieve high accuracy, with Multinomial Naive Bayes and Linear SVC performing best (both above 98% accuracy).
- **AUC Scores:**  
  - MultinomialNB: 96.9%
  - LinearSVC: 95.9%
  - BernoulliNB: 94.9%
  - GaussianNB: 88.1%

---

## Tech Stack

- **Python (Jupyter Notebook)**
- **Libraries:**  
  - pandas, numpy, scikit-learn, nltk, matplotlib

---

## Quick Start

1. Load your email dataset (make sure it’s in the right format).
2. Run the notebook cells step by step.
3. Try out different models and see which works best for your data.

