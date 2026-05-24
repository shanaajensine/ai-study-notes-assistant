# AI Study Notes Assistant

A beginner-friendly question-answering assistant that helps students ask questions from their own study notes.

## Project Overview

This project uses TF-IDF and cosine similarity to retrieve the most relevant answer from user-provided study notes.

The assistant allows users to paste notes, ask a question, and receive the most relevant answer along with a similarity score.

## Features

- Paste custom study notes
- Ask questions from the notes
- Retrieve the most relevant answer
- Show similarity score
- Avoid weak answers using a confidence threshold
- Simple Gradio interface

## Technologies Used

- Python
- scikit-learn
- TF-IDF Vectorizer
- Cosine Similarity
- Gradio
- Google Colab

## How It Works

1. The user enters study notes.
2. The notes are split into smaller chunks.
3. The chunks are converted into numerical vectors using TF-IDF.
4. The user asks a question.
5. The question is converted into a vector.
6. Cosine similarity compares the question with all note chunks.
7. The assistant returns the most relevant chunk as the answer.
8. If the similarity score is too low, the assistant says it could not find a good answer.

## Key Learnings

- Text must be converted into numbers before comparison.
- TF-IDF gives importance to meaningful words.
- Cosine similarity helps find relevant text.
- Chunking affects answer quality.
- A confidence threshold helps reduce weak or incorrect answers.
- Gradio can turn Python code into a simple app interface.

## Limitations

- This assistant does not truly understand language like a large language model.
- It uses similarity matching, so it may fail for complex questions.
- The assistant can only answer from the provided notes.
- It does not generate new explanations beyond the retrieved note chunk.

## Future Improvements

- Add PDF upload support
- Use embeddings for better semantic search
- Add LLM-generated answers
- Build a Streamlit or full web app version
- Store previous notes and questions
