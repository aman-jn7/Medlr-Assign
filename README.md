# Medicine Clustering & Retrieval-Augmented Generation (RAG) Analysis

# Project Overview

This project implements clustering and similarity retrieval for a dataset of medicines using machine learning and natural language processing (NLP) techniques. The goal is to categorize medicines based on their active ingredients, packaging forms, and dosages while enabling fast retrieval of similar medicines using FAISS (Facebook AI Similarity Search).

# Features & Methods Used

# 1. Data Preprocessing

Standardized column names and text fields.

Filled missing values for packaging_form and quantity based on medicine names.

Normalized retail_price and discounted_price.

# 2. Clustering

Extracted embeddings using Sentence Transformers (all-MiniLM-L6-v2).

Applied K-Means clustering to categorize medicines into similar groups.

Evaluated clustering performance using the Silhouette Score.

# 3. Retrieval-Augmented Generation (RAG) for Similarity Search

Stored medicine embeddings in FAISS (L2-based vector search).

Implemented a fast similarity search function to retrieve similar medicines based on embeddings.

# 4. PCA & t-SNE Visualization

Applied Principal Component Analysis (PCA) to reduce embeddings to 2D for better visualization.

Used t-SNE for a more nonlinear separation of clusters.
