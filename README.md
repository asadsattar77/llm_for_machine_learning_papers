# Project: Comparing Pretrained and From-Scratch Models for Machine Learning Research Papers

## Overview

This project compares the performance of pretrained models and models trained from scratch on Machine Learning research papers. Specifically, it uses LLaMA 13B-8 as a pretrained model and trains a T5 model from scratch. The workflow includes data preprocessing, model quantization, training, and evaluation.

## Usage
### 1. Data Preprocessing

- Loads raw research papers from (https://drive.google.com/uc?id=1cNCKr0z1Qy0nCQdcxIXxhLeUFSDuldjP).
- Cleans the text by removing references, headers, footers, and irrelevant text.
- Converts the cleaned text into question-answer pairs using the question generation repository(https://github.com/patil-suraj/question_generation).
- Saves the processed data to dataset.csv file.

### 2. Model Training and Evaluation
#### Pretrained Model: LLaMA 13B-8

#### 1.Quantization and Fine-Tuning:

- Quantize the pretrained LLaMA model using LoRA techniques.
- Fine-tune the model on the preprocessed data.
- Evaluate its performance.
#### 2.From-Scratch Model: T5

#### 3.Configuration:

- Configure the T5 model from scratch.
- Train the T5 model on the same preprocessed data.
- Evaluate its performance.

### 3. Jupyter Notebook
The fyp.ipynb notebook consolidates the workflow:

- Loads the processed data.
- Runs experiments with both pretrained and from-scratch models.
- Compares their performance and visualizes results.

## Models
- LLaMA 13B-8: A pretrained language model used for comparison. Quantized using LoRA techniques and fine-tuned on the dataset.
- T5: Configured and trained from scratch on the preprocessed data.

## Results
- Evaluation Reports: Performance metrics and comparison results for both models are included directly in the code outputs at the end of the fyp.ipynb notebook.
- Plots and Visualizations: Key visualizations of model performances are also included directly in the fyp.ipynb notebook.
