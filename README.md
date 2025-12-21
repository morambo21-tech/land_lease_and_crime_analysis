Toxic Comment Classification

Machine Learning Project for Online Toxicity Risk Detection

Multi-Label Classification ｜ NLP ｜ Imbalanced Data ｜ Interpretability-Ready ｜ Text Mining

Project Overview

This project is based on the Kaggle Toxic Comment Classification Challenge.

The objective is to identify and quantify different types of toxic behavior in online comments using text data collected from Wikipedia discussion pages.

The model outputs a probability score for each toxicity category, which can be interpreted as a content risk indicator to support moderation, filtering, and community safety efforts.

Technical Workflow

Text preprocessing: normalization, tokenization, lemmatization

Feature extraction: TF-IDF representation of comment text

Model training: One-vs-Rest Logistic Regression for multi-label classification

Model evaluation: ROC-AUC with cross-validation

Pipeline design: end-to-end scikit-learn pipeline for reproducibility and clean inference

Key Results

The final model achieves stable ROC-AUC performance across multiple toxicity labels

Linear models with TF-IDF features provide strong baseline accuracy and robustness

Probability outputs enable flexible thresholding for different moderation policies

Dataset

Kaggle Competition:
https://www.kaggle.com/competitions/jigsaw-toxic-comment-classification-challenge

Practical Applications

Automated content moderation

Early detection of abusive or harmful discussions

Customizable toxicity filtering based on platform policy
