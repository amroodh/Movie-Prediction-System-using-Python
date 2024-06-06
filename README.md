# Movie Recommendation System

This project is a Movie Recommendation System built using Machine Learning techniques in Python. The system recommends movies based on various features such as genres, keywords, taglines, cast, and directors.

## Project Structure

- `movie_recommendation_system_using_machine_learning_with_python.py`: This script contains the implementation of the movie recommendation system.
- `movies.csv`: This CSV file contains the dataset of movies used for recommendations.

## Installation

To run this project, you need to have Python installed on your system along with the necessary libraries. You can install the required libraries using the following command:

```bash
pip install numpy pandas scikit-learn
```
## Usage
1.Clone this repository to your local machine.
2.Ensure that movies.csv is in the same directory as the script.
3.Run the script using the following command:
```
python movie_recommendation_system_using_machine_learning_with_python.py
```
4.Enter your favorite movie name when prompted. The system will then output a list of recommended movies based on your input.

## How It Works
1.**Data Collection and Pre-Processing:**
The script reads the movie data from movies.csv.
It selects relevant features for recommendations such as genres, keywords, taglines, cast, and directors.
Null values in these features are replaced with empty strings.
All selected features are combined into a single feature.

2.**Feature Vectorization:**
The combined text features are converted into feature vectors using TfidfVectorizer from the scikit-learn library.

3.**Cosine Similarity Calculation:**
The similarity between movies is calculated using cosine similarity on the feature vectors.

4.**Recommendation Generation:**
The script prompts the user to input their favorite movie name.
It finds the closest match to the input movie name in the dataset.
It retrieves the similarity scores for the matched movie and sorts them to get the top similar movies.
The top similar movies are then printed as recommendations.

## Example
```
 Enter your favourite movie name : Inception
Movies suggested for you :

1. Inception
2. The Dark Knight
3. Interstellar
...
```
