# Japanese PDF Semantic Classifier Using LaBSE and Cosine Similarity

This project extracts Japanese text from PDF files, processes it into clean sentences, and classifies each sentence into predefined environmental and social topics using semantic similarity with multilingual embeddings from the LaBSE model.

## Overview

The goal of this project is to automate the classification of textual content in Japanese PDF documents into meaningful categories. It leverages the LaBSE (Language-agnostic BERT Sentence Embedding) model to generate high-dimensional embeddings for both the document content and a list of predefined topics. Cosine similarity is used to identify the most semantically relevant topic for each sentence.

## Features

- Extracts text from Japanese PDF documents using `pdfplumber`
- Segments and cleans Japanese sentences using regex-based filtering
- Generates semantic embeddings for sentences and topics using the LaBSE model
- Matches sentences to the most relevant topics using cosine similarity
- Supports batch processing of multiple files
- Saves classification results in a structured format

## Dependencies

- Python 3.8+
- pdfplumber  
- sentence-transformers  
- pandas  
- numpy  
- scikit-learn  
- re (Python regex module)


## Folder Descriptions

### `cosine_similarity_japanese_pdf_file/`
**Sentence Classification Results**  
Contains CSV files where each row includes a sentence from a PDF, its page number, the matched ESG topic, and the cosine similarity score that reflects classification confidence.

### `JAPANESE_FILES/`
**ESG-Related Japanese PDF Documents**  
This folder contains the source PDF files written in Japanese, focused on ESG (Environmental, Social, and Governance) topics. These files serve as the input data for the classification pipeline.

### `sentence_embedding_files/`
**Sentence Embeddings**  
Includes outputs where each sentence extracted from the PDFs is paired with its corresponding LaBSE-generated embedding. These are used to compute similarity with topic vectors.

