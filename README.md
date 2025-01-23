# HR-Resume

# AI-Powered Resume Screening with BERT

This project provides an AI-powered resume screening tool using BERT (Bidirectional Encoder Representations from Transformers) to evaluate and rank resumes based on their similarity to a job description. The app leverages BERT's ability to generate contextualized embeddings of text and uses cosine similarity to match resumes with the job description.

## Features
- Upload multiple resumes in `.txt`, `.pdf`, `.docx` format.
- Input a job description and evaluate resumes against it.
- Rank resumes based on their similarity to the job description.
- Display results in a table and highlight the best candidates.

## How It Works
1. **BERT Model**: The app uses a pre-trained BERT model (`bert-large-uncased`) from the Hugging Face `transformers` library to compute embeddings for both job descriptions and resumes.
2. **Cosine Similarity**: The similarity between the job description and each resume is computed using cosine similarity between their embeddings.
3. **Ranking**: Resumes are ranked by similarity score, and the best candidate(s) are highlighted at the top.

## Installation

1. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

2. Run the app:
    ```bash
    streamlit run main.py
    ```

3. Open your browser and go to `http://localhost:8501` to use the app.
