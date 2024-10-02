# Amharic Named Entity Recognition (NER) Project

This project focuses on developing a Named Entity Recognition (NER) model to extract key entities such as products, prices, and locations from Amharic text in Telegram messages. The project is divided into five main tasks, each designed to build upon the previous one.

## Table of Contents

- [Task 1: Data Preparation](#task-1-data-preparation)
- [Task 2: Labeling Data in CoNLL Format](#task-2-labeling-data-in-conll-format)
- [Task 3: Fine-Tuning NER Model](#task-3-fine-tuning-ner-model)
- [Task 4: Model Comparison & Selection](#task-4-model-comparison--selection)
- [Task 5: Model Interpretability](#task-5-model-interpretability)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Task 1: Data Preparation

In this task, we preprocess the dataset containing Amharic Telegram messages. The preprocessing steps include:

- Cleaning the text data.
- Tokenizing the messages for further processing.

## Task 2: Labeling Data in CoNLL Format

In this task, a portion of the dataset is labeled in the CoNLL format, commonly used for NER tasks. The goals include:

- Identifying and labeling entities such as products, prices, and locations.
- Saving the labeled data in a plain text file in CoNLL format.

### CoNLL Format

- Each token is labeled on its own line, followed by its entity label (e.g., `B-Product`, `I-LOC`, `O`).
- Blank lines separate individual sentences/messages.

## Task 3: Fine-Tuning NER Model

This task involves fine-tuning a pre-trained NER model to extract key entities from Amharic text. The steps include:

- Setting up an environment (e.g., Google Colab) with GPU support.
- Installing necessary libraries.
- Loading the labeled dataset in CoNLL format.
- Tokenizing the data and aligning labels with tokens.
- Setting up training arguments and fine-tuning the model using Hugging Face's Trainer API.
- Evaluating the fine-tuned model on a validation set.

## Task 4: Model Comparison & Selection

In this task, multiple NER models are compared to select the best-performing one. The steps include:

- Fine-tuning various models (e.g., XLM-Roberta, DistilBERT, mBERT).
- Evaluating each model's performance on the validation set.
- Comparing models based on accuracy, speed, and robustness.
- Selecting the best-performing model for production.

## Task 5: Model Interpretability

The final task focuses on explaining how the NER model identifies entities to ensure transparency and trust in the system. This includes:

- Implementing SHAP and LIME for model interpretation.
- Analyzing how the model makes decisions and identifying areas for improvement.
- Generating reports to document the model's decision-making process.

## Installation

To set up the project, clone the repository and install the required dependencies:

```bash
git clone <repository-url>
cd <repository-directory>
pip install -r requirements.txt
