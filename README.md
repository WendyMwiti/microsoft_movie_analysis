# microsoft_movie_analysis
An analysis of movies 
Microsoft wants to create original video content and have decided to create a new movie studio. Therefore my task is to  help them succeed in this niche is to explore, understand prepare and analyse various movie datasets and find insights that will help in deciding what films to create.
#Business Understanding
The movie industry is competitive and to be a big performer a company has to approach in the right way, in this case using insights from existing data.There are many popular databases like IMDB and TMDB with movie datasets that we can analyse. For this project 6 datasets were provided and I chose to use 3 which I felt would answer the business questions I posed.
#Goals
My objective is to answer the following questions
a)What are the best rated genres
b)Which is the most profitable month to release a movie
c)What is the relationship between production budget and profit made
d)Which month has the highest movie releases
#Platforms Used
Git/GitHub
#Tools Used
pandas for data analysis
numpy for scientific computation
matplotlib for basic plotting
seaborn for advanced plotting
sqlite3 for running SQL queries on our datasets
#Data Understanding
The first step was to load my data into my jupyter notebook then explore surface properties of the datasets to like the data attributes and its bulkiness
This enabled me to choose the datasets that were best to answer my business questions. Queying the data to find the shape of the data, where relationships lie, the datatypes involved, how many missing values exist and how the aggregations of numerical values appears
#Data Preparation
Having Understood the data, I selected the following datasets: IMDB('im.db'), The Numbers('tn.movie_budgets.csv.gz'), TMDB('tmdb.movies.csv.gz'). This is because their attributes like genres, ratings, production budget, worldwide gross would best inform on my business questions. Here I started data cleaning and in most instances for missing values I dropped them since the datasets were fairly large.  any duplicates of data were dropped. In certain instances, i had to convert certain datatypes  like dates to datetime objects to easily access the values I required. SQL enabled to select only the columns I required for my data analysis. There was a relationship of innterest in the movie_basics table and movie_ratings from the IMDB data so i merged them.
###Visualization
Best Rated Genre
Used a bar graph to show the distribution of the various movie-genres in terms of ratings
![image](https://user-images.githubusercontent.com/109112517/187027381-d7e0f057-0464-440b-a109-835b553ce213.png)
