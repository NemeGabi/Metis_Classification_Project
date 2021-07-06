Classification Project work - MVP

Board Game rating - good or bad?


The goal of the project is to build a model which predicts if a board game will get good or bad rating on BoardGameGeeks (BGG). 

After data cleaning an some EDA work, the median of the Geek ratings ( ~ 5.7) was identify as the threshold of the target. Under that value the board game rating were convert to 0 and above that to 1.

The model selection happened with cross validation on 4 learnt models: K_NearestNeighbor, Logistic Regression, Decision Tree and Random Forest. The models were scored with accuracy and F1 score.

For main classification metric accuracy was chosen, as there is no significant importancy difference between the positive or negative event in the model. Furthermore, during the cross validation of the different models the accuracy over-performed the F1 score in each cases. The best performing model the Random Forest was, so that is the model that we wish to use and improve in the rest of the project.

Please see below the ROC curve and the confusion matrix which confirms it further that with the Random Forest model we can get a balanced, good performing model.



![ROC_Curve](https://raw.githubusercontent.com/NemeGabi/Metis_Classification_Project/main/ROC_Curve.png)

![Confusion_matrix](https://raw.githubusercontent.com/NemeGabi/Metis_Classification_Project/main/Confusion_Matrix.png)

In the model improvement process the best hyper parameters will be identified with tqdm package and GridSearchCV