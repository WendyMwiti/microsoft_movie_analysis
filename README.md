# Analysis of movie datasets
## Overview
Microsoft wants to create original video content and have decided to create a new movie studio. Therefore my task is to  help them succeed in this niche is to explore, understand prepare and analyse various movie datasets and find insights that will help in deciding what films to create.
## Business Understanding
The movie industry is competitive and to be a big performer a company has to approach in the right way, in this case using insights from existing data.There are many popular databases like IMDB and TMDB with movie datasets that we can analyse. For this project 6 datasets were provided and I chose to use 3 which I felt would answer the business questions I posed.
### Goals
My objective is to answer the following questions
1.What are the best rated genres
2.Which is the most profitable month to release a movie
3.What is the relationship between production budget and profit made
4.Which month has the highest movie releases
### Platforms Used
1.Git/GitHub
### Tools Used
1.pandas for data analysis
2.numpy for scientific computation
3.matplotlib for basic plotting
4.seaborn for advanced plotting
5.sqlite3 for running SQL queries on our datasets
## Data Understanding
The first step was to load my data into my jupyter notebook then explore surface properties of the datasets to like the data attributes.This enabled me to choose the datasets that were best to answer my business questions. Queying the data to find the shape of the data, where relationships lie, the datatypes involved, how many missing values exist and how the aggregations of numerical values appears Having Understood the data, I selected the following datasets: IMDB('im.db'), The Numbers('tn.movie_budgets.csv.gz'), TMDB('tmdb.movies.csv.gz'). This is because their attributes like genres, ratings, production budget, worldwide gross would best inform on my business questions
## Data Preparation
Here I started data cleaning and in most instances for missing values I dropped them since the datasets were fairly large and any duplicates of data were dropped. In certain instances, I had to convert certain datatypes  like dates to datetime objects to easily access the values I required. SQL enabled to select only the columns I required for my data analysis. There was a relationship of innterest in the movie_basics table and movie_ratings from the IMDB data so i merged them.
## Visualization
Question 1: What are the Best Rated Genres
Used a bar graph to show the various movie-genres in terms of ratings
![image](https://user-images.githubusercontent.com/109112517/187027381-d7e0f057-0464-440b-a109-835b553ce213.png)
### Findings
Documentaries are the best rated genre followed by comedies with an aspect of drama and adventure respectively. Historical Documentaries are also highly regarded by the audience
Question 2: Which is the most profitable month to release a movie
![image](https://user-images.githubusercontent.com/109112517/187030086-a3eb9b97-d646-4c9c-a8cf-0a71bbc5277d.png)
Due to the provision of worldwidegross and production budget in the The Numbers dataset I was able to calculate the profit various movies brought and later the most profitable month.
### Findings
December produces the highest profits followed by April and finally June.
January has the lowest profits
There is also a relative decline in profits between the months of August and November
Question 3:What is the relationship between production budget and profit made?
![image](https://user-images.githubusercontent.com/109112517/187030458-de22698f-3401-44da-acfd-138082b635ba.png)
### Findings
For the 5 movies in 4 of them, the profit made is relatively higher than the production budget. 1 movie Dark Phoenix, however, made a loss and further attributes would have to be analysed to properly explain this outcome. The margin for the production budget used for the 4 movies that made profits is not so different yet the profits highly vary. Other attributes of the movies like runtime, genre would have to be investigated to paint a clear picture on this situation
Question 4: Which month has the highest Number of movie releases in all the years
![image](https://user-images.githubusercontent.com/109112517/187030818-bc43a405-ff15-4ab9-9b78-6820f3b6d57e.png)
### Findings
January and October are the two months with the highest number of released movies. These two would be referred as dump months. This means the two periods of the year, when new movie releases are either poor-quality, cheaply made, cannot be easily marketed, performed poorly at screen testings or intended for niche audiences. in these two  periods there are lowered commercial and critical expectations for most rekeases from filmmakers and distributors
## Conclusion and Recommendations
1. Microsoft should look into producing more documentary movies as they are highly regarded by audiences with the best ratings as compared with other genres
2. For a higher likelihood of profits Microsoft should consider release  movies during the months of December and April
3. Where movies produced have performed poorly at screen testings, are poorly or cheaply made, meant for niche audiences, Microsoft should release during either the month of January or October, the two dump months




