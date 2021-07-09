Classification project - Board Game time!

The goal of project is to built a model that predict effectively that a new released board game will get a good or bad rating on BoardGameGeeks. It would help people who would like to participate in crowdfunding of a game that which games would "worth" it.
During the project I will identify the rating which separates the good and bad games, then find and fit the best suiting model on the available data.
After I improved the model in the best possible way I will identify the features that has the most influence on the model's performance.


Design

Board game market has been increasing in the past few years, a bigger jump were identified on the game sales in 2020 due to the more free time what people experienced during the pandemic. A great increase were noticed in the number of new game projects too. Many people are listing new game ideas and searching for financial support from the board game loving public. 
People will support games what they believe that will be successful. Studies show that most people makind decisions based on information from friends and personal preferences. Checking a game review site is the online version of "recommendation of friends" so its an important factor of opinion creation.

Data

The dataset was exported from Kaggle and the data were collected from BoardGameGeeks. The site contents plenty of information of the games and gives opportunity to gamers to give ratings/feedback of the games they have tried. 
Over 116000 board game's data included in the original file and after data cleaning, over 25000 data points were used for the project. The selected features are: number of players (min, max), play time(avg, min, max),the year it was released, minimum recommended age, weight (level of complexity, available expands, num_votes, how many people owns the game, reimplements, publisher, category. Target is geek rating.


Algorithms

The project goal is to identify the best performing model even with the trade off in the interpretability. Our users don't want to know how the model works exactly, so we can focus on the accuracy. For large datasets as what we have, random forest model is the best suiting one. It can handle many different types of data and works well with different features too.
For the metric of the project accuracy was chosen as there is no importance differences in the negative and positive event. 

A strong model was built with hyperparameter tuning when I noticed that I made a mistake. During the feature importance check I realized that the two strongest features were in the model by mistake. the number of votes and the number of people who ownes the game are not predictors that a game how successful will be.

The model was re-run on the reduced features which resulted a large drop in the accuracy (~ 0.45). The model was further improved with feature engineering and that made better the final model's performance ( ~ 0.60)


Tools

The main tool was Python package for the project. Visualization of the results were created in Matplotlib.


Communication

The identified most important features
 -Weight
 -Year
 -Avg time 
 -Max time
 -Expands


![ROC_curves](https://raw.githubusercontent.com/NemeGabi/Metis_Classification_Project/main/Old_fixed_ROC_curve.png)


![Feature_importance_chart](https://raw.githubusercontent.com/NemeGabi/Metis_Classification_Project/main/Feature_importance.png)