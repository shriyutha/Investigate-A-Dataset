# Investigate-A-Dataset

Table of Contents

* Introduction

* Data Wrangling

* Exploratory Data Analysis

* Conclusions


INTRODUCTION:

I choose TMDb Movie Data Set to for Data Analysis. 
This Data Set contains more than 1000 records and 21 columns. And it includes information about budget, revenue, runtime, casting, director, genres, release_year, popularity of the movies, viewer's rating, production company and others. 
This Data Set can help us to understand various factors like trends on genres over years, profitabiliy, top movies over years, average runtime over years, top directors and casts and many more.
Following are the points which colud be analysed using Numpy, Pandas(Series and DataFrame) and Matplotlib.

QUESTIONS:

1. Which genre has the highest movies releases?

2. With respect to vote counts
    2.a. Which are the Top 5 Movies ?
    2.b. Who are the Top 5 actors ?
    2.c. Who are the Top 5 directors ?

3. Which movie(s) 
   3.a. Have earned the highest and least profits?
   3.b. Have the highest and least popularity scores?
   3.c. Has the highest and least revenue?
   3.d. Have the highest and least budget?

4. 4.a. Which year has the highest number of movie releases?
   4.b. which year has the highest annual profit?
   4.c. Which year has the highest annual popularity count?

5. 5.a What is Average runtime of all the movies in the data set?
   5.b How does the yearly average movie run time vary over the years in the [1859-2015] ?

6. 6.a. Which acter acted in highest number of films?
   6.b. Which director directed highest number of films?

7. 7.a. Is there a relationship between movie popularity v/s vote_count? 
   7.b. Is there a relationship between movie profit v/s revenue?


DATA WRANGLING:

Here we are going to import CSV file and will perform following operations:

a. Checking head and tail of the data.

b. Checking size, number of rows, columns.

c. Checking null values, description and info.


OBSERVATIONS:

a. There are  major missing values in 'homepage', 'keywords', 'production_companies', 'taglines'.

b. 'id', 'imdb_id', 'homepage', 'tagline', 'overview' are not relevent for this analysis, so we can drop this columns.

c. 'cast', 'genres', 'director' has multivariables. Need to split this columns.

d. Since there are missing values, needs to fill/drop.

e. 'release_date' is not in proper format. Need to change to datetime format (YYYY/MM/DD).


DATA CLEANING:

STEPS:

      a. Dropping not relevent columns.
      
      b. Dropping rows which have missing values.
      
      c. Repalcing '0' values with their mean values.
      
      d. Checking duplicate rows and droping it.
      
      e. Changing the 'release_date' format to datetime format.


CONCLUSION:

Limitations:

The above observations may not be accurate. As I am not using statistical methods and machine learning, further analysis is required for accurate information.

Some rows are deleted from data set, due to NAh or missing values. This may effect the analysis.

Some columns also deleted from data set, thought not relevent for my analysis. This may effect the analysis too.

In this project, I have analysied general trends in movies.

And these observations are tentative, not verified by principles of statistics and machine learning.


ACCORDING TO MY ANALYSIS:

1. Drama has the highest number of movies release followed by Comedy and Thriller.

2. Inception is the most voted movie, Leonardo DiCaprio is the most voted actor and Christopher Nolan is the most voted director.

3. AVATAR is highest profit earned movie and THE WARRIOR'S WAY is the lowest profit earned movie.

4. Highest number of movies released in 2014, highest popularity in 2015 and highest profit earned in 2015 followed by 2012.

5. The average mean runtime is: 103.89758781937479 by the time of analysis.

6. ROBERT DE NIRO is the actor who acted highest number of movies and WOODY ALLEN is the director who directed highest number of movies.

7. There is a relation between revenue and profit. As revenue increases, profit also increases.
