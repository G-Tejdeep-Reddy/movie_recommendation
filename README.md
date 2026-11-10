# Movie Recommendation System

Discover what to watch next with a genre-based recommendation engine built using **Python, scikit-learn, and Flask**. Enter a title to receive five recommendations ranked by cosine similarity.

## Overview

This content-based recommendation system compares titles using their genres. It converts genre labels into numerical vectors and calculates cosine similarity to identify similar titles from a dataset of **3,256 titles**.

The recommendation engine connects to a Flask web application, allowing users to enter a title and view recommendations through a web interface.

## Features

- **Genre-Based Recommendations:** Finds similar titles using genre information.
- **Cosine Similarity:** Ranks titles by similarity between their genre vectors.
- **Title Search:** Matches titles regardless of letter case or surrounding input spaces.
- **Flask Integration:** Connects the recommendation logic to input and results pages.

## How It Works

1. Load the dataset and handle missing genre values.
2. Encode comma-separated genres using `CountVectorizer`.
3. Compute pairwise cosine similarity between titles.
4. Match the user's input to a title in the dataset.
5. Select five recommendations from the similarity ranking and display the results.

## Technology Stack

- **Language:** Python
- **Data Processing:** pandas
- **Recommendation Engine:** scikit-learn
- **Web Framework:** Flask
- **Frontend:** HTML and CSS

## Project Structure

```text
movie-recommendation-system/
├── demo.py                 # Flask application and web routes
├── netflix.py              # Genre-based cosine similarity recommendation engine
├── netflix_full.csv        # Dataset containing 3,256 titles and their metadata
├── templates/              # HTML templates required by the Flask application
│   ├── index.html          # Title input page
│   └── sub.html            # Recommendation results page
└── README.md               # Project documentation
```
