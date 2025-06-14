# Project - Hybrid Movie Recommendation System
This project builds a hybrid recommender system using the MovieLens 1M Dataset to suggest movies based on both content features (genres, titles) and collaborative filtering (user behavior).

# Overview

This project implements a **Hybrid Recommendation Engine** using the [MovieLens 1M dataset](https://grouplens.org/datasets/movielens/1m/). It combines **Content-Based Filtering** and **Collaborative Filtering** to recommend movies based on both movie metadata (genres, titles) and user behavior (ratings).

---

## Project Highlights

- **Content-Based Filtering** using TF-IDF on movie genres and titles
- **Collaborative Filtering** with SVD matrix factorization + cosine similarity
- **Hybrid Recommender**: Combines both scores using a weighted average
- Visualization of recommendation scores
- Clean, modular pipeline in Jupyter Notebook

---

## Dataset

**Source**: [MovieLens 1M Dataset](https://grouplens.org/datasets/movielens/1m/)

The dataset consists of:
- `movies.dat`: MovieID, Title, Genres
- `ratings.dat`: UserID, MovieID, Rating, Timestamp
- `users.dat`: UserID, Gender, Age, Occupation, Zip-code

> These files are preprocessed and converted to CSV before analysis.

---

## Tech Stack

- Python (Pandas, NumPy)
- Scikit-learn (TF-IDF, SVD, Pipelines)
- Matplotlib / Seaborn for visualization
- Jupyter Notebook

---

## Workflow

1. **Data Preprocessing**  
   Convert `.dat` files to `.csv`, merge dataframes, handle missing values.

2. **Content-Based Filtering**  
   - TF-IDF Vectorization of `Title + Genres`
   - Cosine similarity between movie vectors

3. **Collaborative Filtering**  
   - Create a User-Movie ratings matrix
   - Apply Truncated SVD for dimensionality reduction
   - Calculate similarity between movie latent vectors

4. **Hybrid Recommender**  
   ```python
   hybrid_scores = α * content_score + (1 - α) * collaborative_score

---

# Contact

- Email: [anubhavdogra7@gmail.com](mailto:anubhavdogra7@gmail.com)
- LinkedIn: [linkedin.com/in/anubhav-dogra](https://www.linkedin.com/in/anubhav-dogra/)
- GitHub: [github.com/anubhavdogra1](https://github.com/anubhavdogra1)
- Instagram: [@anubhavdogra1](https://www.instagram.com/anubhavdogra1/)
- Website: [My Portfolio](https://www.notion.so/Anubhav-Dogra-211d6dc537bf8027bfe3ebdf322032ec)
