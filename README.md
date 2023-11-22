# The Film Industry: Analysis of movies in the Box Office.
![Image](./Data/cinema2.jpeg)
## Report Overview.
1. Business Understanding
1. Data Assembly.
2. Data verification.
3. Data cleaning.
4. Data Analysis.
5. Data VIsualization.
6. Conclusion.
7. Recommendations.
## Business Understanding.
### Client:
Microsoft Corporation.
### Target : 
The Head of Microsoft's New Movie studio.
### Report  Compiled by:
Bonventure Osoro Willis
### Introduction.
The film industry or motion picture industry comprises the technological and commercial institutions of filmmaking. It dates back to France in 1895 when the first cinematograph was projected. Movie studios earn revenue through:
1. Movie theatre ticket sales(The box office).
2. Merchandise sales like action figures or branded clothing.
3. Television Rights.
4. Streaming.
5. VOD(video on demand).

In 2019, the global box office was worth `$`42.2 billion. When including box office and home entertainment revenue, the global film industry was worth `$`136 billion.
The profitability of a film studio is crucially dependent on picking the right film projects and involving the right management and creative teams, but it also depends heavily on choosing the right scale and approach to film promotion, and control over receipts through technologies. In the extreme, for a major media franchise centered on film, the film might itself be only one large component of many large contributions to total franchise revenue.
The film industry is a brutally competitive winner-take-all market and is "extremely volatile" and it is impossible to predict in advance who will become the market winner at any given moment "or how long their domination will last".
### Problem Statement.
Due to the increase in profitability of the motion picture industry, many companies have ventured into the market by trying to produce movies and television shows for the target audience.
Microsoft Corporation is also looking to diversify into the Film Industry. As a starting point, Microsoft wants to launch a movie studio that can compete with the already established studios that have a market share
### Objective.
1. To analyze movies that have been at the box office.
2. To explore what types of films are currently doing the best at the box office.
3. To translate those findings into actionable insights.
4. To suggest to the client what type of films to create.
## Data Assembly.
The datasets provided were outdated hence the datasets used in this report were outsourced from [Kaggle](https://www.kaggle.com/).
They are :

1. [oscars dataset](https://www.kaggle.com/datasets/pushpakhinglaspure/oscar-dataset)

contains Oscar Academy Award-winning films from 1927-2022 and has 1360 rows and 5 columns:

|Ind|column|Info|
|---|---|---|
|0|Index|indices|
|1|Film|Movie name|
|2|Year|Year of release|
|3|Award|Awards won|
|4|Nomination|Number of awards nominated for|

2. [top 1000 grossing movies](https://www.kaggle.com/datasets/crisleyoliveira/top1000moviesgross)

contains the top 1000 grossing movies at the box office.
it has 1000 rows and 7 columns
the columns are:

|Ind|column|Info|
|---|---|---|
|0|Title|movie name|
|1|Year|Year of release|
|2|Runtime|length of the movie|
|4|Gross|Total revenue earned|
|5|ImdbRating|The movie's rating on IMDB|
|6|imdbRatingVotes|total rating votes on IMDB|
|7|metascoreRating|The movie's rating on Metascore|
|8|rottenRating|The movie's rating on Rotten Tomatoes|
|9|metacriticRating|The movie's rating on Metacritic|

3. Imdb_movies.csv

contains 10178 movies and has the following columns:

|Ind|column|Info|
|---|---|---|
|0|names|Movie name|
|1|date_x|Year of release|
|2|score|rating|
|3|genre|type of movie|
|4|overview|short description|
|5|crew|cast|
|6|orig_title|Movie name|
|7|status|released or not released|
|8|orig_lang|language spoken|
|9|budget_x|Number of awards nominated for|
|10|revenue|total revenue|
|11|country|country of origin|

4. [IMDB_Most_Popular_Movies](https://www.kaggle.com/datasets/ifeoluwafaromika/23000-imdb-most-popular-movies)

contains 23096 movies with the following columns

|Ind|column|Info|
|---|---|---|
|0|movie|movie name|
|1|year|year of release|
|2|category|target audience|
|3|duration|runtime|
|4|genres|movie type|
|5|rating|movie rating|
|6|tagline|catchphrase|
|7|director|movie director|
|8|stars|cast|
|9|votes|number of votes used to rate|
## Data cleaning.
For each of the datasets, I am going to:
1. Remove the irrelevant columns 
2. Remove any of the entries that contain NaN values.
3. Rename columns to achieve naming consistency in all subsets.
### Cleaned Data
From our datasets, I have cleaned and obtained the following subsets:
1. oscar_movies... (oscar winning movies)
2. imdb_movies... (random movies on IMDb)
3. Top_1000_movies... (top 1000 grossing movies)
4. most_popular_movies... (most popular movies on IMDb)

I am not merging the subsets into one because I want them to retain their unique features. Instead, during analysis I will be pulling only the required features from each subset and merging them where necessary.
## Data Analysis.
In this section, I will analyze the subsets created. I am going to focus on four categories:

1. BUDGET.
    1. Budget vs revenue: I will determine if the amount of budget allocated affects the revenue

    2. Budget vs rating: I will determine if the amount of budget allocated affects the rating received

2. GENRE

    1. Genre vs Oscars: I will determine what genres won more Oscars

    2. Genre vs revenue. I will determine if some genres return more revenue than others

3. MOVIE GUIDELINE CATEGORY

I will determine if the movie guideline given eg PG13 affects revenue

4. LANGUAGE

I will determine if the spoken language inthe movie affects revenue.
## Data Analysis Results:
### Budget:
1. The average movie budget is `$`64,882,378
2. The most common movie budget is `$`20,000,000
3. The median movie budget is `$`50,000,000
4. The correlation between movie budget and revenue is 0.674.
### Genre:
The most popular genres are:
    1. Drama.
    2. Action.
    3. Comedy.
    4. Adventure.
    5. Animation.
    6. Horror.
    7. Biography.
### Movie Guideline Category:
The top movie ratings are:
    1. R.
    2. PG-13.
    3. PG.
    4. TV-MA.
    5. TV-14.
    6. G.
### Language:
The most spoken languages in Box Office movies are:
    1. English.
    2. Japanese.
    3. Spanish.
    4. korean.
    5. French.
## SUMMARY.
In this report, we have focused on four main areas in order to meet our objectives:
1. Budget.
2. Genre.
3. Movie Guideline Category.
4. Spoken Language.

We have to acknowldge that there are other factors that may affect the success of a movie studio and the success of the movies they produce. This may include:

1. The movie directors : some directors are better than others.

2. The cast in the movies : some actors have a large fanbase that is always on the lookout for their movies.

3. The promotion strategy of the studio : how well do they promote their movies.

In the film industry there are also some notable mentions:
1. Hollywood is the world's oldest national film industry, and largest in terms of box office gross revenue.
2. Indian cinema is the largest national film industry in terms of the number of films produced, with 2,446 feature films produced annually as of 2019.
3. As of 2021, Chinese cinema has the highest annual ticket sales with 1,156 million tickets sold.
## RECOMMENDATIONS.

From our analysis, we have come up with the following recommendation :

1. I found that the average movie budget has a strong correlation to it's revenue. For the popular and top earning movies, average movie budget was `$`64,882,378 and most common movie budget was`$`20,000,000. Hence I recommend that the movies produced by the new Microsoft studio should have a minimun budget that ranges from `$`20,000,000 - `$`60,000,000. 

2. Some genres peformed better than others in the Box Office. I recommed that the movies produced by the Micorsoft studio, should fall under the following genres:

    1. Drama.
    2. Action.
    3. Comedy.
    4. Adventure.
    5. Animation.
    6. Horror.
    7. Biography.

3. During the analysis of the Box Office, I found out that some movie categories were more popular than others hence earned more revenue. It is recommended that the movies produced by Microsoft movie studio, should fall under the following ratings:
    1. R.
    2. PG-13.
    3. PG.
    4. TV-MA.
    5. TV-14.
    6. G.
 
4. From the report, we can see that movies that used some languages were more common than others. I recommend that movies produced by Microsoft movie studio should use the following spoken languages:
    1. English.
    2. Japanese.
    3. Spanish.
    4. korean.
    5. French.
 
5. I also recommend that the Movie studio should choose the right movie director and a well known cast to tap into their fanbase.

6. I recommend that the movie studio should be established in Hollywood, if possible. This is because Hollywood has the largest box office revenue.

7. It is recommended that the Movie Studio should first release the movies in the Chinese cinema because they have the highest ticket sales in the industry. 



