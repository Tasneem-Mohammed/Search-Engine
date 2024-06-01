# **Document Search Engine using CISI Dataset**

## Overview
This project implements a document search engine using the CISI dataset, leveraging various information retrieval and natural language processing techniques. The project involves data preprocessing, indexing, query processing, and query expansion using TF-IDF, BM25, and word embeddings.

## Tools and Technologies
- **Languages:** Python
- **Libraries:** PyTerrier, Pandas, NLTK, Gensim, Gradio
- **Data Source:** CISI dataset
- **Frameworks:** PyTerrier

## Project Steps

### 1. Data Collection
- **Load CISI Dataset:** The dataset is extracted from a zip file and includes documents, queries, and relevance judgments.
- **Read Documents:** Extract text from the CISI.ALL file.
- **Read Queries:** Extract query text from the CISI.QRY file.
- **Read Qrels:** Extract relevance judgments from the CISI.REL file.

### 2. Data Preprocessing
- **Tokenization:** Split text into tokens.
- **Stopword Removal:** Remove common stopwords.
- **Stemming:** Reduce words to their root forms.
- **Cleaning:** Remove special characters, tabs, and extra white spaces.

### 3. Indexing
- **Index Documents:** Use PyTerrier’s DFIndexer to create an index of the preprocessed documents.

### 4. Query Processing
- **TF-IDF Model:** Implement TF-IDF retrieval model to process and rank documents based on the query.

### 5. Query Expansion
- **Word2Vec Model:** Train a Continuous Bag of Words (CBOW) model to create word embeddings.
- **BM25 Model:** Implement BM25 retrieval model for initial ranking.
- **RM3 Query Expansion:** Expand the query using RM3 method based on the initial BM25 results.

### 6. User Interface
- **Gradio Interface:** Create a web-based interface for users to enter queries and retrieve documents.
  ![image](https://github.com/Tasneem-Mohammed/Search-Engine/assets/120495578/72b10859-0cb8-46cc-93b8-fbceef930c4c)


### 7. Evaluation
- **Evaluate Retrieval Accuracy:** Test with various queries and assess retrieval accuracy and speed using metrics like precision and recall.

## Results Summary
- **TF-IDF Retrieval:** Provided baseline search results.
- **BM25 with Query Expansion:** Improved search accuracy with query expansion.
- **Word2Vec Embeddings:** Enhanced understanding of word similarities and query expansion.

## Conclusion
This project demonstrates the implementation of a document search engine using the CISI dataset with various retrieval models and query expansion techniques. The integration of TF-IDF, BM25, and Word2Vec embeddings, along with the user-friendly Gradio interface, showcases the effectiveness of combining traditional and advanced NLP techniques for information retrieval.

- **Date:** 11/5/2024
