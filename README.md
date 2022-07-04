# Movie Recommendation System

![Python](https://img.shields.io/badge/Python-3.8-blueviolet)

This program built using two methods that are Weighted Average Rating and Content-based Filtering. It provides the recommended movie's title, genre, release date, runtime, rating, and votes. 

## Weighted Average Rating

The ideas behind this recommendation system:
1. Movies that are more popular will have a greater chance of being liked by the average user as well
2. This model does not provide personalized recommendations for each type of user
3. The implementation of this model is also quite easy, all we need to do is sort the films by rating and popularity and show the top films from the list of films.

**Formula of IMDB with Weighted Rating (WR):** <br>
<img src='img/wr-formula.png' width=600px> <br>
**Description:** <br>
v: the number of votes for the movie <br>
m: the minimum number of votes needed to enter the chart <br>
R: average rating of the movie <br>
C: the average number of votes from the entire movie universe <br>

## Content-based Filtering

Content-based filtering uses movie features to recommend other movies similar to what movie does user recently watch or searched, so this technique doesn't require other users' data during recommendations to one user. This technique uses a similarity metric, for its case using Cosine Similarity, to determine how similar is a vector to a given vector. Then, the top few are recommended.

**Formula of Cosine Similarity** <br>
<img src='img/cosim.png'>
