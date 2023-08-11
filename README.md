# DS5110 FInal Project
## Introduction
This project aims to predict whether a running play will result in a first down based on player tracking at the time of the hand-off. Using a dataset that was provided as part of the 2020 NFL Big Data Bowl,  we leverage Spark ML to preprocess data, extract relevant features, and employ three machine learning models for prediction.

 

## Dataset
The dataset originates from the 2020 NFL Big Data Bowl. It contains granular player tracking data for over 30,000 NFL rushing plays from 2017 to 2019. The data consisted of 49 variables, spanning from unique identifiers such as  PlayId, to game identifier, GameId, to player attributes like position, speed, acceleration, defensive presence, down, and more.

 

## Preprocessing and Feature Engineering
The dataset underwent thorough preprocessing and feature engineering. We introduced new features like DistanceToTouchdown, which illustrates the distance from the current position to the end zone, and ClosestDefenderDistance, which signifies the proximity of the nearest defender to the ball carrier (rusher). We also established a binary target variable first_down_gained to pinpoint if a play resulted in a first down.
## Modeling
We employed three machine learning models: logistic regression, random forest, and a gradient boosted trees model.

 

The models were evaluated based on the following metrics:
Accuracy: The proportion of true results among the total cases.
Precision: The proportion of true positive predictions among the positive predictions.
Recall: The proportion of true positive predictions among the actual positives.
F1 Score: The harmonic mean of precision and recall, providing a balance between the two.
AUC (Area Under the Curve): Represents the model's ability to distinguish between positive and negative classes.

 

## Results
Although the differences in performance between the models were marginal, the Gradient Boosting model showed slightly higher proficiency in predicting first_down_gained.

 

## Conclusion and Future Work
Our results suggest the effectiveness of Gradient Boosting models in predicting the success of first downs using the features from the NFL Big Data Bowl dataset. For future studies, we aim to include additional features, refine model parameters, and explore deep learning models such as CNNs.
