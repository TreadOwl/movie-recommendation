# Movie Recommendation System

This repository contains a **Movie Recommendation System** implemented in Python (using Pandas and Scikit-Learn) that provides personalized recommendations based on three distinct approaches:

## 1. Simple Recommender
- Uses a mathematically robust formula, inspired by **IMDb's Weighted Rating**, to calculate a metric based on critical ratings and vote counts.
- It provides generalized recommendations useful for building charts of overall top movies.

## 2. Content-Based Recommenders
### Description-Based Recommender
- Leverages the movie's `overview` and `tagline`.
- Uses a **TF-IDF (Term Frequency-Inverse Document Frequency) Vectorizer** to analyze the text.
- Calculates similarity between movies using **Cosine Similarity** (`linear_kernel`) to return 30 closely related titles.

### Metadata-Based Recommender
- Analyzes granular movie details including `director`, `cast` (top 3 actors), `keywords` (stemmed), and `genres`.
- The director's influence is weighted 3x higher to improve recommendation relevance.
- Applies a **CountVectorizer** and utilizes **Cosine Similarity** to match multi-dimensional metadata arrays.

---

**Tech Stack Highlights:** Pandas, NumPy, Scikit-Learn (TF-IDF, CountVectorizer, Cosine Similarity), NLTK (SnowballStemmer).
