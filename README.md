# Video Game Engagement Analysis

## Overview

![gaming banner](https://github.com/user-attachments/assets/f200cc23-f195-4468-98e0-2df27b7b39c8)


The purpose of this project is to provide stakeholders with valuable insights into predictors of high engagement in video game players (gamers).  This project can be used to predict high engagement in video games to make recommendations for video game design and marketing strategies.

## Business Understanding

The stakeholder for this project is a video game producer or marketer.  This project can be used for predictive modeling of video game player engagement patterns which can be used for optimization of game design and marketing strategies.  This can be used to help the business design games to be more engaging.  It can also help the business with targeting marketing towards individuals who are highly engaged in video games. 

## Data and Methodology

Data regarding high engagement behavior in video game plaers was given in one csv file: [Rabie El Kharoua. (2024). 🎮 Predict Online Gaming Behavior Dataset](https://www.kaggle.com/datasets/rabieelkharoua/predict-online-gaming-behavior-dataset)

I created a `TARGET` column based on whether or not an entry was a high engagement gamer and dividied it into two categories.  10k entries for high engagement gamers and 10k entries for low engagement gamers. 

For this business question recall is the most important metric because it emphasizes limiting the amount of false negatives in the model. 

## Models
I am attempting to produce the model with the highest recall and the lowest number of false negatives.  Then I tuned that model to produce the best performance. 

<img width="359" alt="updated evaluation metrics" src="https://github.com/user-attachments/assets/cb1bd291-d254-4dd0-a481-f829d859aa33">


## Final Model

<img width="326" alt="final model" src="https://github.com/user-attachments/assets/e460fef8-f0e7-4e50-9bc0-71943229c3e1">

<img width="653" alt="final model" src="https://github.com/user-attachments/assets/3a64f072-d041-43bf-8c41-d127733645d9">

When finding a model to predict high engagement in video game players I saw that the logistic regression model with a intercept was performing best by producing the smallest number of false negatives.  

## Conclusions
- __Conclusion 1:__  When finding a model to predict high engagement gaming activity I found that the logistic regression model with an intercept was performing best at reducing the number of false negatives.


- __Conslusion 2:__  The most important features to my model for predicting high engagement gaming behavior are how many sessions per week they play and how long those sessions are. There is a steep increase in the proportion of high engagement gamers in people who play 9 or more sessions per week of at least 90 minutes. 

![predictors](https://github.com/user-attachments/assets/112bd56f-88ff-4523-9e0f-ac50a6fba252)

![sessionsperweek](https://github.com/user-attachments/assets/5eaefdbc-c878-4731-9049-93b416481884)

![session duration](https://github.com/user-attachments/assets/729ccc94-d6d6-4adf-b013-c5eda097dc83)

- __Conclusion 3:__   Age, gender, game difficulty, location, and game genre are not significant or important features in predicting high engagement gamers. 

## Next Steps
- __Next Step 1:__  This model can be useful for predicting which people are more likely to be engaged in the video games you design or who to advertise to in order to have a higher chance of getting them to purchase your game.


- __Next Step 2:__  Learn how to identify people based on how many sessions they play per week and how many minutes they spend playing in each session. 


- __Next Step 3:__  Limitation: I tried to change the C parameter to 100 and ran it for an hour and fifteen minutes before it fit the model and it didn't change the results. Therefore, I'm going to remove this from the program so that if someone wants to run it it won't take that long.  I also ran C=10 and it took quite some time too and didn't make a difference with the metrics so I'm going to keep it at default. 

## For More Information
See the full analysis in the [Jupyter Notebook](https://github.com/josh-g-grimes/Gaming-Behavior/blob/main/notebook.ipynb) or review [this presentation](https://docs.google.com/presentation/d/16DpmhlED85T7bBYjyElxSJ-8xrJmT_Df4Wvs0EHA63Y/edit?usp=sharing). 

For additional info, contact Josh Grimes at josh.g.grimes@gmail.com


## Project Structure
|-- git ignore
|-- README.md
|-- gb_final_notebook
|-- online_gaming_behavior_data
|-- video game engagement presentation
