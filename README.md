# Resume Classification using RoBERTa and GPT-2
This project focuses on the classification of resumes into predefined categories using state-of-the-art transformer-based models, specifically RoBERTa and GPT-2. The project involves training, fine-tuning, and evaluating these models to achieve high accuracy in categorizing resumes based on their content.

# Introduction
In the modern recruitment process, resumes are a primary source of information for evaluating candidates. This project automates the classification of resumes into categories such as job roles, industries, or levels of experience using advanced natural language processing (NLP) models.
# Dataset

Dataset Used: Resume.csv (attached with code)

Labels: The Designation field is used as the target variable for classification.

Preprocessing: The dataset was preprocessed to combine all relevant fields into a single text field for input into the models.
# Models Used

RoBERTa (Robustly Optimized BERT):

Pre-trained model fine-tuned for sequence classification.
Tokenized input with a maximum length of 128.

GPT-2:

Adapted for classification by adding a classification head.
Used a custom tokenizer with the EOS token as padding.

# Methodology

1-Pre-reprocessing:

Combine relevant fields (e.g., Skills, Experience, Education) into a single text string.

Encode labels using categorical encoding.

2-Dataset Splitting:

Split the dataset into 80% training and 20% testing sets.

3-Model Training:

Fine-tuned RoBERTa and GPT-2 models for one epoch using training data.

4-Evaluation:

Evaluated models on test data using accuracy as the primary metric.

5-Fine-Tuning:

Fine-tuned both models for additional epochs to further improve performance.

# How to Run

Prerequisites

Python 3.8+

PyTorch

Transformers (Hugging Face)

Pandas, NumPy, Scikit-learn

# Steps

1- Clone this repository:

    git clone 
    cd 

2- Run the training script:

    python train.py

3- Evaluate the models:

    python evaluate.py
