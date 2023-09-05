# Movie Recommender System

This is a content based movie recommender system that makes suggestions based on the similarity between movie plots, genres, cast etc.

## Overview

The project follows the below steps:

1. Load and pre-process the TMDB movie metadata dataset
2. Combine important features into a tags column
3. Vectorize tags into TF-IDF vectors
4. Calculate cosine similarity between movie vectors
5. Make recommendations by finding most similar movies

The core components are:

- `data_preprocessing.ipynb`: Data cleaning and feature engineering 
- `model_building.ipynb`: TF-IDF vectorization and similarity calculation
- `app.py`: Streamlit app for movie selection and recommendations
- `utils.py`: Contains helper functions

## Usage

To run the movie recommender app:

```
streamlit run app.py
```

This will launch the webapp where you can pick a movie title and get recommendations.

The movie similarity matrices are saved as pickle files to avoid recalculation.

## Future Improvements

Some ways to improve the project in future:

- Use better similarity metrics like Jaccard or fuzzy matching
- Incorporate ratings, watched status for personalization
- Add additional metadata like actors, directors etc.
- Use image based similarity to find visually similar movies
- Deploy the app on a cloud platform for increased availability
