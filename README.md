# Movie Recommender System

A content-based movie recommendation prototype built from TMDB metadata. It combines movie overviews, genres, cast, crew, and keywords into a textual "tags" vector, computes similarity via cosine distance, and recommends similar movies for a given title.

## 🚀 Features

- Loads and merges TMDB movie and credits datasets.  
- Extracts and normalizes director, top cast, genres, keywords, and overview.  
- Constructs a combined "tags" field per movie.  
- Vectorizes tags using `CountVectorizer` (with English stop words removed).  
- Computes cosine similarity across movies.  
- Provides a `recommend(movie_title)` function to print top-N similar movies.  
- Persists precomputed artifacts (`movie_list.pkl`, `similarity.pkl`) for fast inference.

## 🛠️ Quickstart

### Prerequisites

- Python 3.8+  
- `pip`  
- TMDB datasets:
  - `tmdb_5000_movies.csv`
  - `tmdb_5000_credits.csv`  
