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


