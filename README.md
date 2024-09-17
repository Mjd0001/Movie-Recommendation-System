# Movie Recommendation System
This project implements a Movie Recommendation System using a Jupyter Notebook (movie_recommendation_system.ipynb). The system suggests similar movies based on a user's input using cosine similarity and TF-IDF vectorization on features like genres, keywords, tagline, cast, and director.

## Dataset
The dataset used for this project is a CSV file (movies.csv) containing information about various movies, such as:

- Genres
- Keywords
- Tagline
- Cast
- Director
- Title (for user input and recommendations)
- Features

The following features from the dataset are used to build the recommendation system:

- Genres
- Keywords
- Tagline
- Cast
- Director
These features are combined to form a single text which is then vectorized using TF-IDF to help calculate the similarity between movies.

## Installation
Clone this repository:

```
git clone https://github.com/yourusername/movierecommendationsystem.git

cd movierecommendationsystem
```

Install the required dependencies:

```
pip install -r requirements.txt
```
Place the movies.csv dataset in the project directory.

## Usage
Open the Jupyter Notebook:
```
jupyter notebook movie_recommendation_system.ipynb
```
Run all cells in the notebook to execute the recommendation system.

Enter your favorite movie name when prompted:
```
Enter your favourite movie name: Inception
```
The system will recommend the top 30 most similar movies:
```
Movies suggested for you:
1 - Interstellar
2 - The Prestige
3 - Memento
...
```
## How It Works
- Data Loading: The system loads the movie dataset and processes it to clean any missing values in the selected features.
- Feature Engineering: Combines relevant features such as genres, keywords, tagline, cast, and director into a single text for each movie.
- Vectorization: Uses TF-IDF vectorization to convert text data into numerical features for similarity comparison.
- Cosine Similarity: Computes the cosine similarity between the input movie and all other movies in the dataset to rank them based on similarity scores.
- Movie Recommendation: The system suggests the top 30 most similar movies based on the similarity scores.

## Dependencies
To run this project, the following libraries are required:

Python 3.x
NumPy
Pandas
Scikit-learn
Difflib
