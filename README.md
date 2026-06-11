# Movie Recommendation System

## Overview

A content-based Movie Recommendation System that suggests movies similar to a user's selected movie based on genres, keywords, cast, crew, and movie overview information.

The system leverages Natural Language Processing (NLP) techniques and cosine similarity to identify movies with similar characteristics and provides recommendations through an interactive Streamlit web application.

---

## Features

* Content-based movie recommendation engine
* Interactive Streamlit web interface
* Real-time movie poster retrieval using TMDB API
* NLP-based feature extraction and text preprocessing
* Cosine similarity-based recommendation generation
* Fast inference using pre-computed similarity matrices

---

## Dataset

The project utilizes the TMDB 5000 Movie Dataset:

* tmdb_5000_movies.csv
* tmdb_5000_credits.csv

The dataset contains:

* Movie titles
* Genres
* Cast information
* Crew information
* Keywords
* Movie overviews
* Popularity metrics

---

## Methodology

### Data Preprocessing

* Merged movie and credits datasets
* Removed irrelevant and missing values
* Extracted genres, keywords, cast, and director information
* Combined relevant features into a unified text representation

### Feature Engineering

Created a consolidated movie profile using:

* Genres
* Keywords
* Top cast members
* Director
* Movie overview

### Text Vectorization

Applied:

* CountVectorizer
* Token normalization
* Stemming

to convert textual information into numerical feature vectors.

### Similarity Computation

Generated a similarity matrix using Cosine Similarity to identify movies with related content characteristics.

---

## Tech Stack

* Python
* Pandas
* NumPy
* Scikit-learn
* NLTK
* Streamlit
* Requests API
* Pickle

---

## Project Structure

```text
Movie-Recommendation-System/
│
├── app.py
├── movie-recomendation.ipynb
├── movie_list.pkl
├── similarity.pkl
├── requirements.txt
│
├── tmdb_5000_movies.csv
├── tmdb_5000_credits.csv
│
└── venv/
```

---

## How It Works

1. User selects a movie from the Streamlit interface.
2. The recommendation engine retrieves the movie index.
3. Similar movies are identified using the cosine similarity matrix.
4. Top recommendations are generated.
5. Movie posters are fetched dynamically from TMDB API.
6. Results are displayed in an interactive dashboard.

---

## Results

* Generates Top-5 personalized movie recommendations.
* Provides visual movie posters for enhanced user experience.
* Delivers recommendations with low inference latency through precomputed similarity scores.

---

## Future Enhancements

* Collaborative Filtering
* Hybrid Recommendation Systems
* Deep Learning-based Recommendations
* User Authentication
* Personalized User Profiles
* Cloud Deployment using AWS

---

## Author

Arnab Ghosh

Machine Learning | Data Science | Artificial Intelligence
