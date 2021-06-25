# Predicting pass or run plays in the NFL

The objective of this project was to address the question - can we predict whether a team is going to run or pass the based on information available prior to the play?

The answer to this question is important to football teams as they determine how to prepare for a coming play when on defense. If a team can accuractely predict if their opponent will pass or run the ball, they will have a competitive advantage while on defense.

![image](https://user-images.githubusercontent.com/81783731/123434356-628cb300-d59a-11eb-89cd-cbad69f8eb60.png)

The dataset used for this analysis was obtained from the 'Detailed NFL Play-by-Play Data 2009-2018' kaggle page (https://www.kaggle.com/maxhorowitz/nflplaybyplay2009to2016). It contains information from 2,526 games across 10 seasons. There were 449,371 plays in those games). Please note, this dataset was too large to include in this repo, but it can be found at the above link.

Our goal in this project was to build a machine learning model that could accuractely predict if a team would run or pass the ball.

The model with the best performance (in terms of accurately predicting whether a team would run or pass the ball) was an XGBoost model. The optimal hyperparameters for this model were determined using grid search. This model achieved an accuracy of 70.2%. Confusion matrix for best model:

<img width="372" alt="Screen Shot 2021-06-24 at 10 25 51 AM" src="https://user-images.githubusercontent.com/81783731/123435133-3887c080-d59b-11eb-94c2-23b160fca480.png">

The most important features leveraged in this model were:
1. Yard line
2. Score differential
3. Time remaining
4. Yards needed for first down

Files included in this repo:
NFL Notebook.ipynb - Jupyter notebook containing code used for this analysis
NFL Predictions.pdf - Presentation detailing some of the findings from this project
README.md - You are reading this now
