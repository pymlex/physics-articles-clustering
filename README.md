# Clustering Physics Research Articles

<div style="text-align: center;">
    <img alt="image" src="https://github.com/user-attachments/assets/dcac315a-86c9-4d21-96bd-6a5e8bbe7a20" />
</div>

This project performs clustering of modern physics research articles from [Kaggle](https://www.kaggle.com/datasets/victornuez/latest-research-articles) using SciBERT embeddings and K-Means.  
The goal is to analyse the structure of scientific texts, identify natural groups of articles, and study whether semantic embeddings correlate with article importance metrics such as citations, accesses, and online attention.

## Overview

- Source: latest research articles dataset from Kaggle.  
- Task: cluster physics articles using SciBERT text embeddings.  
- Input: title and abstract combined into a single text field.  
- Embeddings: SciBERT (110M parameters, uncased scientific vocabulary).  
- Clustering: K-Means, number of clusters selected via silhouette score.  
- Additional analysis includes PCA, t-SNE projections, and cluster statistics.

## Findings

Clustering separates articles semantically, but the resulting **groups do not correlate** with citation-based or attention-based importance metrics.  
This illustrates the limitation of BERT-type models: embeddings capture semantic similarity effectively but do not encode deeper structural or contextual value such as scientific influence.
