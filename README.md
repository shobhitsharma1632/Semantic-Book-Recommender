# Semantic Book Recommender

A semantic, emotion-aware book recommendation system powered by NLP and machine learning.

## Overview

This project provides a book recommendation dashboard that leverages semantic search and emotion analysis to suggest books based on user queries, preferred categories, and emotional tone. It uses state-of-the-art language models and embeddings to understand book descriptions and user intent, delivering personalized recommendations.

## Features

- **Semantic Search:** Finds books similar to a user's description using vector embeddings.
- **Emotion-Aware Filtering:** Recommends books by matching the desired emotional tone (e.g., happy, sad, suspenseful).
- **Category Selection:** Filter recommendations by simplified book categories (e.g., Fiction, Nonfiction, Children's Fiction).
- **Interactive Dashboard:** User-friendly Gradio interface for entering queries and viewing recommendations with book covers and summaries.

## Data

- Book metadata and descriptions are processed and cleaned from public datasets.
- Categories are mapped to simplified groups for easier filtering.
- Emotion scores for each book are computed using a transformer-based emotion classifier.

## Main Components

- [`gradio_dashboard.py`](gradio_dashboard.py): Main app with the Gradio UI and recommendation logic.
- [`books_with_emotions.csv`](books_with_emotions.csv): Final dataset with book metadata, simplified categories, and emotion scores.
- [`text_classification.ipynb`](text_classification.ipynb): Notebook for category mapping and classification.
- [`sentiment_analysis.ipynb`](sentiment_analysis.ipynb): Notebook for emotion analysis and scoring.
- [`data_exploration.ipynb`](data_exploration.ipynb): Data cleaning and exploration.

## Getting Started

1. **Install dependencies:**
   ```sh
   pip install -r requirements.txt
   ```

2. **Run the dashboard:**
   ```sh
   python gradio_dashboard.py
   ```

3. **Open the provided link in your browser to use the recommender.**

## Requirements

- Python 3.8+
- See [`requirements.txt`](requirements.txt) for all dependencies.

## Project Structure

- `gradio_dashboard.py` — Main application
- `books_with_emotions.csv` — Enriched book data
- `text_classification.ipynb` — Category processing
- `sentiment_analysis.ipynb` — Emotion scoring
- `data_exploration.ipynb` — Data cleaning
- `README.md`, `requirements.txt`, etc.

## Acknowledgements

- [LangChain](https://github.com/langchain-ai/langchain)
- [HuggingFace Transformers](https://github.com/huggingface/transformers)
- [Gradio](https://github.com/gradio-app/gradio)
- Public book datasets from Kaggle
