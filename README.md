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

    # Prerequisites

Python 3.8+

PyTorch

Transformers (Hugging Face)

Pandas, NumPy, Scikit-learn

# Steps

1- Clone this repository:

    git clone https://github.com/csaurabh26/Resume_extraction_using_LLM.git
    cd NLP_PROJECT-2

2- Run the training script:

    python train.py

3- Evaluate the models:

    python evaluate.py


# Future Work

1- Enhancing Dataset: Include a larger and more diverse dataset for better generalization.

2- Multilingual Support: Extend the model to handle resumes in multiple languages.

3- Additional Models: Experiment with newer transformer models such as DeBERTa or LLaMA.

4- Explainability: Develop visualization tools to explain model predictions.

# References
1-	Automated Resume Parsing: A Natural Language Processing Approach
Thatavarthi Giri Sougandh; Sai Snehith K; Nithish Sagar Reddy; Meena Belwal
Published in: 2023 7th International Conference on Computation System and Information Technology for Sustainable Solutions (CSITSS)
Date of Conference: 02-04 November 2023
Date Added to IEEE Xplore: 07 December 2023

2-	Information Extraction From Free-Form CV Documents in Multiple Languages
Davor Vukadin; Adrian Satja Kurdija; Goran Delač; Marin Šilić
Published in: IEEE Access ( Volume: 9)
Page(s): 84559 - 84575
Date of Publication: 09 June 2021 
Electronic ISSN: 2169-3536

3-	Empirical Evaluation of Large Language Models in Resume Classification
Prasanna Kumar R; Rithani M; Bharathi Mohan G; Venkatakrishnan R
Published in: 2024 Fourth International Conference on Advances in Electrical, Computing, Communication and Sustainable Technologies (ICAECT)
Date of Conference: 11-12 January 2024
Date Added to IEEE Xplore: 21 March 2024 
Conference Location: Bhilai, India

4-	Revolutionizing Talent Acquisition: A Comparative Study of Large Language Models in Resume Classification
R Venkatakrishnan; M Rithani; G Bharathi Mohan; V Sulochana; R PrasannaKumar
Published in: 2024 5th International Conference on Innovative Trends in Information Technology (ICITIIT)
Date of Conference: 15-16 March 2024
Date Added to IEEE Xplore: 10 July 2024
ISBN Information:
DOI: 10.1109/ICITIIT61487.2024.10580109
Conference Location: Kottayam, India

