# Ethio Mart Telegram NER Project

This project aims to develop a Named Entity Recognition (NER) system for Amharic text by collecting and preprocessing data from Ethiopian-based Telegram e-commerce channels. The application fetches messages, images, and documents, preprocesses the data for entity extraction, and compares different NER models.

## Table of Contents

- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Objectives](#objectives)
  - [Task 1: Data Ingestion and Data Preprocessing](#task-1-data-ingestion-and-data-preprocessing)
- [Configuration](#configuration)
- [Model Development](#model-development)
- [License](#license)

## Features

- Connects to Telegram using an API ID and hash.
- Fetches messages, images, and documents from specified Telegram channels in real-time.
- Cleans and preprocesses Amharic text for NER.
- Supports image and document handling.
- Saves fetched messages into a structured JSON file for further analysis.
- Compares different NER models for performance evaluation.

## Requirements

- Python 3.7 or higher
- `telethon` library
- `sqlite3` (comes with Python)
- Additional libraries for NER and data processing (e.g., `spaCy`, `transformers`, etc.)

You can install the required libraries using pip:

```bash
pip install telethon
pip install spacy transformers
