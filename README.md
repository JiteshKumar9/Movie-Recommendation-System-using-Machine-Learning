# Movie-Recommendation-System


This project is a content-based Movie Recommendation System that suggests similar movies based on a given movie title. It uses a combination of movie genres and overviews to generate recommendations using Natural Language Processing techniques.

## Features

- **Content-Based Filtering**: Recommends movies based on their similarity to the selected movie.
- **Text Vectorization**: Uses `CountVectorizer` to convert text data into numerical vectors.
- **Cosine Similarity**: Calculates the similarity between movies based on their vectorized tags.
- **Interactive Recommendations**: Users can input a movie title to get top similar movies.

## Dataset

The system uses a dataset containing the following columns:
- `id`: Unique identifier for each movie.
- `title`: Movie title.
- `genre`: Genres associated with the movie.
- `overview`: Brief description of the movie.
- `popularity`, `release_date`, `vote_average`, `vote_count`: Additional metadata (not used in recommendations).

### Example of Dataset Format

| id   | title                   | genre          | overview                                   |
|------|-------------------------|----------------|-------------------------------------------|
| 278  | The Shawshank Redemption | Drama,Crime    | Framed in the 1940s for the double murder... |

## How It Works

1. **Data Preparation**:
   - Combines `genre` and `overview` columns into a new column `tags`.
   - Filters the dataset to include only `id`, `title`, and `tags`.

2. **Text Vectorization**:
   - Converts the `tags` column into numerical vectors using `CountVectorizer` with a vocabulary size of 10,000 and English stop words removed.

3. **Similarity Calculation**:
   - Computes pairwise cosine similarity between all movie vectors.

4. **Recommendations**:
   - Retrieves the top 5 movies similar to the given movie title based on cosine similarity scores.

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/movie-recommendation-system.git


![image](https://github.com/user-attachments/assets/3ee061b7-ba1f-454a-bf36-e43b62ec6033)

![image](https://github.com/user-attachments/assets/d7363a97-415a-44ed-bf5f-a77dbef275c5)

