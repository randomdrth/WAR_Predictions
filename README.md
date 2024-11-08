# Project Overview

This project attempts to predict a baseball player's Wins Above Replacement (WAR) for the upcoming season using historical data. WAR is a comprehensive statistic used to summarize a player's overall contribution to their team. By leveraging historical performance metrics and machine learning, this project aims to forecast the WAR a player will generate next season, which can be useful for teams looking to make data-driven roster decisions.

## Project steps

* Download the baseball season data using pybaseball from 2002 to 2022
* Clean the data (remove or replace null values, delete rows)
* Run feature selection, identify most promising features, and generate any relevant features
* Create a ridge regression model and estimate accuracy
* Measure error, improve the model, and boost accuracy

## Code

You can find all of the code necessary for the project [here](https://github.com/randomdrth/WAR_Predictions/blob/main/war_predictions.ipynb)

Files:

* 'war_predictions.ipynb' - the Jupyter notebook that contains all of the code

# Local Setup

## Installation

The following need to be installed locally in order to explore the project:

* Python
* JupyterLab
* Python packages
    * pybaseball
    * pandas
    * numpy
    * scikit learn

All of the data used in the project will be downloaded using the 'pybaseball' package

## Results

* The initial model showed a reasonable accuracy but struggled with players having limited historical data or coming off injuries
* Some key predictors included Intentional Base on Balls (IBB) and Hard-Hit Percentage (Hard%+)
* The current model can be further optimized with feature selection and hyperparameter tuning

## Next Steps

* Experiment with ensemble models like Random Forest and Gradient Boosting Machines (GBM)
* Use the optimized model to predict next season’s WAR for current players using their latest stats.
    * This could help teams make more informed decisions before the season starts
* Incorporate minor league stats to improve predictions for rookies

_More detailed takeaways and next steps can be found at the end of the Jupyter Notebook_

