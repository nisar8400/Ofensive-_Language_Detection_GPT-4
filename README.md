# Ofensive-_Language_Detection_GPT-4
This project explores the detection of offensive language in Roman Urdu using GPT-4 embeddings as a feature extraction method. We implemented an end-to-end pipeline that involves preprocessing raw text, extracting embeddings from GPT-4, and utilizing both machine learning (ML) and deep learning (DL) models for classification. 
Introduction
Offensive language detection is critical for maintaining a safe online environment, especially in low-resource languages such as Roman Urdu. The task involves challenges due to linguistic variability and limited annotated datasets. This project leverages GPT-4 embeddings to improve feature representation for ML and DL models.

Objectives
1.	Preprocess Roman Urdu text to prepare it for embedding generation.
2.	Generate embeddings using GPT-4 through OpenAI’s API.
3.	Train traditional ML models (Logistic Regression, SVM, and Random Forest) and a Bi-LSTM DL model.
4.	Evaluate the models based on precision, recall, F1-score, and accuracy.
Dataset
The dataset consists of Roman Urdu text classified as either "Offensive" or "Not Offensive". It contains two columns:
Methodology
Step 1: Data Preprocessing
1.	Text Cleaning: Removed special characters, numbers, and extra spaces.
2.	Label Mapping: Converted "Offensive" to 1 and "Not Offensive" to 0.
3.	Train-Test Split: Divided the data into 80% training and 20% testing sets, maintaining class distribution.
Step 2: Generating GPT-4 Embeddings
1.	Used OpenAI’s text-embedding-ada-002 model to extract 1536-dimensional embeddings for each comment.
2.	Embedded both training and testing sets to represent textual data numerically.
Step 3: Model Training
•	Machine Learning Models:
o	Logistic Regression
o	Support Vector Machine (SVM)
o	Random Forest
•	Deep Learning Model:
o	Bidirectional LSTM (Bi-LSTM) with dense layers and dropout for regularization.
Step 4: Evaluation
•	Metrics used:
o	Accuracy
o	Precision
o	Recall
o	F1-Score
