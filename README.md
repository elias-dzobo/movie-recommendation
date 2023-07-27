# Movie Recommendation Using Unsupervised Learning 

## Objective
Create a function that takes a user ID and an integer n and returns n recommendations for the user 

## Workflow 
1. Data Preprocessing:
- Load the MovieLens data into a pandas DataFrame.
- Handle any missing data: check for missing values and fill them appropriately.
- Conduct exploratory data analysis: understand the dataset, look for patterns, outliers, etc.
2. Data Transformation:
- Transform the data to prepare it for the unsupervised learning model. This can involve
creating a matrix where each row corresponds to a user, each column corresponds to a
different movie, and each entry corresponds to a user's rating for a specific movie.
3. Model Creation:
- Use an unsupervised learning technique such as K-means clustering or hierarchical
clustering to segment users into groups. The idea is that users in the same cluster have similar
movie preferences.
- Experiment with different numbers of clusters. Determine the optimal number of clusters
by using techniques such as the Elbow method.
4. Recommender System:
- Create a function that takes a user ID and the number of recommendations as inputs and
outputs movie recommendations for that user.
- This function can work by finding the cluster that a user belongs to, and then
recommending the highest-rated movies from that cluster that the user hasn't already rated.
5. Evaluation:
- Although this is an unsupervised task, we can still evaluate the performance of our
recommender system. One common way to do this is by splitting the data into a training set
and a test set. We can pretend we don't know some of the ratings in the test set, predict them
using our recommender system, and then compare our predictions to the actual values.
- Calculate metrics such as RMSE (Root Mean Squared Error) and MAE (Mean Absolute
Error) to evaluate the performance of your recommender system.


