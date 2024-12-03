# Movie Recommender System

## Overview
This project is a Movie Recommender System built using content-based filtering. The system recommends movies to users based on the features of the movies (such as genre, director, cast, etc.) and compares them with the movies the user has previously liked or watched. The data used for the recommendations is sourced from Kaggle, specifically the MovieLens dataset. This project utilizes Python and various libraries like pandas, scikit-learn, and numpy for the data processing and model building.

## Features
* **Content-Based Filtering:** Recommends movies based on similarity with a given movie using features such as genre, director, and cast.
* **User-Item Similarity:** Uses cosine similarity to measure the similarity between movies and suggest the most similar movies.
* **Data Handling:** The dataset is cleaned and processed to extract the relevant features for making recommendations.Features

## Technologies Used
* Python 
* Pandas: For data manipulation and cleaning.
* Numpy: For numerical operations.
* Scikit-learn: For building the recommendation algorithm using cosine similarity.
* Matplotlib & Seaborn: For data visualization.
* Jupyter Notebook: For project documentation and step-by-step analysis.

## Data
The dataset used for this recommender system is sourced from Kaggle. The data contains movie metadata including the following features:
* Movie Title
* Genre
* Director
* Cast
* Rating
* Release Date
* Plot

The dataset has been cleaned and processed to ensure relevant information for content-based filtering.

## Data Processing
* **Handling Missing Values:** Missing values are either imputed or removed based on the context of the data.
* **Feature Engineering:** Features like 'genre', 'director', and 'cast' are combined into a single column for similarity calculation.
* **Bag of Words Representation:** The text data (such as movie descriptions, genres, and cast) is converted into a Bag of Words model using the CountVectorizer from scikit-learn.
* **Cosine Similarity:** The cosine similarity between movies is calculated based on the Bag of Words features to find the most similar movies.


## Model - Content-Based Filtering
The movie recommender system uses content-based filtering, which compares a movie's features with those of other movies. The steps for building the model are as follows:

* **Preprocess the Data:** Clean and combine features like genre, director, and cast into a single text column.
* **Bag of Words Representation:** Convert the combined text features into a Bag of Words representation.
* **Cosine Similarity:** Calculate the cosine similarity between the Bag of Words vectors of movies.
* **Recommendation Generation:** Based on the input movie, suggest movies with the highest similarity scores.
  
## Example of Recommendations
Given a movie like "The Matrix", the system will recommend other movies that are similar in terms of genre, director, and other features, using the Bag of Words similarity.

## Future Improvements
* Hybrid Recommender System:** Combining content-based filtering with collaborative filtering for better recommendations.
* Personalized Recommendations:** Implementing user profiling to generate personalized recommendations.
* Real-Time Data Integration:** Allowing real-time data fetching from APIs like TheMovieDB or IMDb for up-to-date movie information.

## Streamlit Application
https://movie-recommender-system-sahilkarale.streamlit.app/

## Sample Visual
![Screenshot 2024-12-03 233742](https://github.com/user-attachments/assets/f8141f5b-290b-454a-abe7-1d7da95a6e72)

