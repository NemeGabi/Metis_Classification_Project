Classification module

The project goal is to predict if the rate of a boardgame which is added to BoardGameGeek will get a good rating or not.

https://boardgamegeek.com

The website shows details of the boardgames and users can rate the games. The dataset downloaded from Kaggle and after dropping the lines with 0 geek_rating the project will calculate with over 25.000 boardgame's data.

What do the game ratings mean?

There are three rating systems you will see on the site:

User Rating (aka Your Rating): The rating you gave to the game. When viewing the ratings section of a game page you can see the individual ratings each user gave that particular game. You will see this rating listed in advanced searches and your game collection.
Average Rating: The average of all the ratings from registered BGG users, calculated by adding up the individual ratings and dividing by the number of ratings. You will see this rating listed in advanced searches and near the top of game pages.

BGG Rating (aka Geek Rating): BoardGameGeek's ranking charts are ordered using the BGG Rating, which is based on the Average Rating, but with some alterations. To prevent games with relatively few votes climbing to the top of the BGG Ranks, artificial "dummy" votes are added to the User Ratings. These votes are currently thought to be 100 votes equal to the mid range of the voting scale: 5.5, but the actual algorithm is kept secret to avoid manipulation. The effect of adding these dummy votes is to pull BGG Ratings toward the mid range. Games with a large number of votes will see their BGG Rating alter very little from their Average Rating, but games with relatively few user ratings will see their BGG Rating move considerably toward 5.5. This is known as "Bayesian averaging" and a quick search of both BGG and/or the Web will reveal much discussion on the topic. You will see this rating listed in advanced searches, your game collection, and near the top, most right corner of game pages.


The target of the project is the Geek_rating data. Other features are min_players, max_players, avg_time, min_time, max_time, year, avg_rating, num_votes, rank, age, owned, weight,expands, reimplements. The Geek_rate mean is 5.7 on the training data.


The next steps are to pick a few - possibly important - features and check what results we would get with a logistic regression model on the selected features. The results will direct us what model and possible feature engineering would increase our model's score. 
