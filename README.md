LLM-Detect AI Generated Text Detection

This repository contains eight notebooks focused on detecting AI-generated text using DistilBERT embeddings and classification techniques.

Notebooks

1. DistilBERT Embeddings Generation (LLM-Detect AI generated Text)
2. DistilBERT Embeddings Generation (Daigt-V4)
3. XLM-RoBERTa Embeddings Generation (LLM-Detect AI generated Text)
4. XLM-RoBERTa Embeddings Generation (Daigt-V4)

These notebooks are responsible for generating embeddings using the DistilBERT and XLM-RoBERTa models from text data.

Steps:

Installation of Dependencies: Installs transformers and torch.

Data Loading: Loads a  dataset (preprocessed_LLM_detect_AI_dataset.csv).

Embedding Generation: Uses DistilBERTTokenizer and DistilBertModel to produce embeddings for each text entry.

Output: Saves embeddings for further processing.

5. XGBoost on DistilBERT Embeddings (LLM-Detect Dataset)
6. XGBoost on DistilBERT Embeddings (Daigt-V4)
7. XGBoost on XLM-RoBERTa Embeddings (LLM-Detect Dataset)
8. XGBoost on XLM-RoBERTa Embeddings (Daigt-V4)

These notebooks focuses on training a classification model using the embeddings generated in the previous notebook.

Steps:

Data Loading: Loads embeddings dataset (dataset2_distilbert_with_embeddings.csv).

Data Preparation: Converts string embeddings into numerical arrays.

Model Training: Uses XGBoost Classifier for training and evaluation.

Performance Evaluation: Provides classification reports and accuracy metrics.
Note:This process is repeated for both datasets and both models.

Requirements

transformers

torch

pandas

numpy

scikit-learn

Usage

Run the DistilBERT Embeddings Generation notebook to produce embeddings from your dataset.

Save the embeddings as a CSV file.

Use the XGBoost on DistilBERT Embeddings notebook to train and evaluate a classifier on the generated embeddings.
