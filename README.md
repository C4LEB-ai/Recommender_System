# Movies Recommender_System
Movie Recommendation system
## Data Set
The data set used for this notebook is the 1M ratings data set from MovieLens. This contains 1M ratings of movies from 7120 movies and 14,025 Users. This data set includes:

- movieId
- userId
- rating
In addition a data set of the movies includes the movie name and genres.
- 

- movieId
- title
- genres
The dataset can be found here : https://github.com/Gurupradeep/Movie-Recommendation-System/tree/master/Dataset
- 

Approaches Used :
Non Personalised Recommendations
This type of recommendations are simple but very useful. Because they solve the cold start problem for users. That is without knowing anything about the user, we can do some recommendations to the user. After getting some reviews from the user or getting some additional information about the user, we can switch some of the more advanced model which are described below.

In the notebook, formula given by IMDB was used to calculate the best movies according to various genres and they can be recommended to any new user.

Most Commonly wathced movie by people who watched X were
This recommender takes the approach of looking at at all users who have watched a particular movie and then counts the returns the most popular movie returned by that group.

Finding similar movies
Without taking content into account (Just based on ratings)
Here just based on the ratings of the users for different movies, we use K nearest neighbours algorithm to find the movies which are similar.

With taking Content into account
Here we just information about the movies, in this case the information of genres to predict the most similar movies.

Matrix Factorisation(Collabarative Filtering)
Two approaches were tried to do matrix factorisation, the low rank method is very slow, so used scipy's SVD for sparse matrix.

Required Tools
- 
- Keras
- Scipy
- Numpy
- Pandas
- python 3
