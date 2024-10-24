# Content-Based-Movie-Recommendation-System
This Python-based movie recommendation system uses cosine similarity to suggest movies similar to a user-specified movie. It leverages features like keywords, cast, genres, and director to compare movies and recommend the most similar ones from a dataset.

**Features**

Takes user input to specify a favorite movie.
Uses a CountVectorizer to transform movie features into a matrix of token counts.
Computes cosine similarity between all movies in the dataset.
Outputs a list of 10 movies most similar to the user's choice.
Prerequisites
Before running this project, ensure you have the following installed:
Python 3.x
Pandas
NumPy
Scikit-learn

**Dataset**

The project relies on a CSV file (movie_dataset.csv) containing the following columns:
title (Movie title)
keywords
cast
genres
director
Make sure the movie_dataset.csv file is present in the same directory as the Python script.

**Code Overview**

The core functionality is divided into the following steps:

Reading the CSV file: The dataset is loaded using Pandas.
Combining movie features: The selected features (keywords, cast, genres, director) are combined into a single string for each movie.
Count Matrix: The combined feature column is vectorized into a count matrix.
Cosine Similarity Calculation: Cosine similarity is used to calculate the similarity between the user-specified movie and all other movies in the dataset.
Movie Recommendations: Based on the cosine similarity scores, the system returns the top 10 most similar movies.
