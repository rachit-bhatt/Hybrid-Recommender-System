# Comparing Collaborative Filtering-Based Recommender and Hybrid (Collaborative Plus Content) Recommender System

## Project Description
In this project, we compare collaborative filtering-based recommender systems and hybrid recommender systems. The collaborative filtering-based recommender is built using the Matrix Factorization technique, while the hybrid recommender system combines collaborative filtering with content-based filtering using a Neural Embedding layer from the PyTorch package.

## Dataset Description
The dataset used in this project is from the MovieLens dataset collected by the GroupLens Research Project at the University of Minnesota. It consists of:

- 100,000 ratings (1-5) from 943 users on 1682 movies.

- Each user has rated at least 20 movies.

## Files in the Dataset
**u.data:** The full dataset containing 100,000 ratings by 943 users on 1682 items. This is a tab-separated list of `user id | item id | rating | timestamp`.

**u.item:** Information about the items (movies); this is a tab-separated list of `movie id | movie title | release date | video release date | IMDb URL | genres`.

**u.genre:** A list of the genres.

## Project Structure
**data/:** Contains the dataset files.

- u.data

- u.item

- u.genre

**src/:** Contains the source code for the project.

- `collaborative_filtering.py`: Code for building the collaborative filtering-based recommender system.

- `hybrid_recommender.py`: Code for building the hybrid recommender system.

- `sentiment_analysis.py`: Code for fetching tweets and calculating sentiment scores.

**reports/:** Contains the project report and presentation slides.

- `project_report.docx`

- `presentation_slides.pdf`

## Installation
To run this project, you need to have Python installed along with the following libraries:

- pandas

- numpy

- torch

- vaderSentiment

- tweepy

You can install the required libraries using the following command:

```bash
pip install -r requirements.txt
```

## Usage
1. **Load the Dataset:**

- Place the dataset files (u.data, u.item, u.genre) in the data/ directory.

- Run the collaborative_filtering.py script to build the collaborative filtering-based recommender system.

- Run the hybrid_recommender.py script to build the hybrid recommender system.

2. **Sentiment Analysis:**

- Run the sentiment_analysis.py script to fetch tweets and calculate sentiment scores for each movie.

3. **Evaluation:**

- Evaluate the performance of both recommender systems using metrics such as RMSE, MAE, Precision, Recall, and F1-Score.

## Results
The results of the experiments, including the comparison of RMSE, MAE, Precision, Recall, and F1-Score for the two recommendation models, are documented in the project_report.docx file.

## References
He, X., Liao, L., Zhang, H., Nie, L., Hu, X., & Chua, T. S. (2017, April). Neural collaborative filtering. In Proceedings of the 26th international conference on the world wide web (pp. 173-182).