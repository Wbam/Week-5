# Task 2: Label a Subset of Dataset in CoNLL Format

## Overview
This project aims to label a portion of a provided dataset in the CoNLL format, commonly used for Named Entity Recognition (NER) tasks. The goal is to identify and label entities such as products, prices, and locations in Amharic text from a dataset containing various product descriptions.

## Dataset
The dataset consists of a "Message" column that includes text describing various products and entities. Each message contains information that needs to be processed and labeled.

### Entity Types
The following entities are labeled in the CoNLL format:

- **B-Product**: The beginning of a product entity (e.g., "Baby bottle").
- **I-Product**: Inside a product entity (e.g., the word "bottle" in "Baby bottle").
- **B-LOC**: The beginning of a location entity (e.g., "Addis Abeba", "Bole").
- **I-LOC**: Inside a location entity (e.g., the word "Abeba" in “Addis Abeba”).
- **B-PRICE**: The beginning of a price entity (e.g., "ዋጋ 1000 ብር", "በ 100 ብር").
- **I-PRICE**: Inside a price entity (e.g., the word "1000" in “ዋጋ 1000 ብር”).
- **O**: Tokens that are outside any entities.

## Requirements
- Python 3.x
- Libraries: `telethon`, `json`, `re`, `sqlite3`, etc.

## Usage
1. **Setup**: Clone this repository and navigate to the project directory.
2. **Install Dependencies**: Use pip to install the required libraries.
   ```bash
   pip install -r requirements.txt
