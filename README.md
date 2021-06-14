# Predicting-the-English-Premier-League

By Elvis Dang and Jake Haggard
-------------------------------------------------------------------------------------------------
## Intro

This was a school project that was made to showcase the Data-Science Workflow. The purpose of this is to predict the outcome of an English Premier League game. 
The outputs will be the full time result of a mathc; **0** (Home Win), **1** (Away Win), and **2** (Draw).   

-------------------------------------------------------------------------------------------------
## Data

The data for this came from 'https://www.football-data.co.uk/englandm.php', I used the data from 2014-2015 season to the 2020-2021 season. In this data one main thing was that a porition of the data had a *Time* variable. So I created two types of models, models that use the time variable and models that don't use it. The models that use this variable have less data but delivered better results than the ones without the *Time* variable. 

-------------------------------------------------------------------------------------------------
## Data Preparation

To prepare the data for the Machine Learning algorithms the data had to be processed and some variables needed to be encoded. There wasn't too much done here outside of merging
all of the individual datasets together, removed NaN values, and dropped irrelevant columns/features. When it came to encoding the data, the variables that were encoded are *Season*, *Time*, *Home Team*, *Away Team*, *Match Referee*, and *Full Time Results*.

-------------------------------------------------------------------------------------------------
## ML Algorithms

The following Machine Learning Algorithms used are:
  * Logistic Regression
      - Accuracy: 61.842%

  * Random Forest
      - Accuracy: 63.157%
      
  * K-Nearest Neighbors
       - Accuracy: 58.552%
  
  * Neural Network (Multi Layer Perceptron)
      - Accuracy: 63.157%
      
  * Ensemble Method (Made using the fours models above)
      - Accuracy: 62.5%

There is a report in this repo that discusses the models in more details. If interested in the models you can read that or look at the models themselves (which are also in the repo).

-------------------------------------------------------------------------------------------------
## Misc.

* The structure of this project was set up after all of the programming and what not was done, so if you want to run the code I'd recommend putting all of the data and notebooks
into the same directory. The file paths will also have to be changed if you were to run them on your machine. 

* The Random Forest and Neural Network models yielded the same accuracy score however when given an example match the Random Forest was able to accurately predict the outcome where the Neural Network model did not accurately predict the outcome of the match. 

* I have a plan to make this into a Python GUI App using the models created. This would give users the chance to predict a match using various models. 
