# movie-recommendation-system
Developing a movie recommendation system using The Movie Database (TMDb) and IMDb movie datasets, incorporating content-based, collaborative, and hybrid recommendation methods

# Requirements
Python 3.8+ Jupyter Notebook - Kaggle Notebook is preferrable.

# Dataset
Movie Dataset : https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata and https://www.kaggle.com/datasets/rounakbanik/the-movies-dataset

# How to Run The Notebook.
1. Login to Kaggle.com
2. Visit  https://www.kaggle.com/datasets/liewyousheng/geolocation link
3. Click on "New Notebook" Option Available on the top of the screen.
4. Download the ".ipynb" File attached in the current repository, select the right version
5. Upload On the New Notebook place by clicking on Import Notebook option.
6. Run The Notebook program

# Run the program in virtual envrionment python
1. Create virtual environment
2. Activate virtual environment
3. Install requirements.txt 
4. Run jupyter notebook and Open the .ipynb notebook file on the localhost:8888

# Key Data Insights
1. The Weighted Mean Ratings model introduces flexibility by employing a weighted average of user mean and item mean ratings.The mean rating for all the movies is approx 6 on a scale of 10.The next step is to determine an appropriate value for m, the minimum votes required to be listed in the chart. We will use 90th percentile as our cutoff. In other words, for a movie to feature in the charts, it must have more votes than at least 90% of the movies in the list.This model is simply based on the popularity of movies.
2.The Weighted Mean Rating does not recommend movies based on user preferences, so we implemented a content-based recommender. This system utilizes movie titles, descriptions, cast, genres, and directors. Using these features, the model predicts new movies for users based on the characteristics of the movies they have already watched.
3. In the content recommendation system, we included the weighted mean rating factor to deliver more refined and accurate results to the users.
4. To address the limitations of the content-based recommendation system, we developed a collaborative filtering recommender system using the Surprise library. The objective was to compare the performance of various collaborative filtering algorithms to identify the one with the highest prediction accuracy, measured by the Root Mean Square Error (RMSE).
5The finally we build the Hybrid movie recommendation system. This powerful approach combines the strengths of Content-based Filtering, Collaborative Filtering and Weighted Score to consider additional factors like popularity or the weighted average rating of a movie. The data score that we already get before can be using a mix of weighted average and popularity, which can be incorporated into the hybrid model to make the recommendations more robust
