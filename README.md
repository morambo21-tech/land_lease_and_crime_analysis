# Toxic Comment Classification
Multi-Label Text Classification Project for Detecting Online Toxicity

Binary Classification ｜ Text Feature Engineering ｜ Multi-Label Imbalanced Data ｜ SHAP Interpretability ｜ NLP Pipeline

## Project Overview
This project is based on the **Jigsaw Toxic Comment Classification** dataset from Kaggle.

The goal is to predict the probability that a given online comment belongs to one or more toxicity categories:  
`toxic`, `severe_toxic`, `obscene`, `threat`, `insult`, `identity_hate`.  

The model outputs a probability score for each category, enabling platforms to flag or moderate harmful comments proactively, while retaining safe speech.

## Technical Workflow
- **Data preprocessing:** text cleaning, punctuation removal, tokenization, lemmatization, stopword filtering  
- **Feature engineering:** TF-IDF vectorization (uni-grams), n-gram representation  
- **Model training:** One-vs-Rest Logistic Regression on multi-label targets  
- **Model evaluation:** ROC-AUC, F1-score, recall per label  
- **Model interpretability:** SHAP-based feature analysis for text insights

## Key Results
- The final model (One-vs-Rest Logistic Regression) achieves strong per-label ROC-AUC on validation data  
- SHAP analysis shows which words contribute most to different types of toxicity  
- Probabilistic outputs allow flexible thresholds for moderation policies

## Dataset
Kaggle Competition:  
[Toxic Comment Classification Challenge](https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge)

**Disclaimer:** The dataset contains offensive language, including profanity and identity-based attacks.

## Example Usage
```python
from pipeline import build_pipeline

pipeline = build_pipeline()
pipeline.fit(X_train, y_train)
y_pred = pipeline.predict_proba(X_test)

Tableau Dashboard (Optional)

Interactive dashboards can translate prediction outputs into moderation insights:
🔗 Live Dashboard (Tableau Public)
https://public.tableau.com/
