# Genre-Recommender
Repository recommending genre based on the ratings you give to the movies

## Introduction

PCS(Pearson Correlation Similarity) Measure to solve for the closest in likings users to estimate ratings given to movies by a user which is a Collabrative Filtering Methodology.This engine then uses K-Means clustering to cluster movies of similar genre into groups for boosting the performance and curacy of predictions. Also made a basic terminal app which asks the user to rate certain movies and the recommends genre based on ratings as well as show to closest users thus predicting age,sex etc.

## Pre-Reqs

You should have Scikit-Learn Preinstalled. You can install it by

      pip install -U scikit-learn
The Pre-Reqs to install scikit-learn are :
Python (>= 2.7 or >= 3.3),
NumPy (>= 1.8.2),
SciPy (>= 0.13.3).


## Results

The datatset used for the training and testing of the engine is the MovieLens100K dataset . The schema of the dataset can be read about here or in the /data repo . In brief the dataset has 100,000 user ratings (valued between 1-5) for 943 users across 1682 movies . Along with that essential features of users like age,sex,occupation and zipcode as well as essential features of movies like genre,year etc are provied.
The Engine accuracy will be measured using Mean squared error evaluation between predicted rating and ground truth rating which can be checked [here](http://files.grouplens.org/datasets/movielens/ml-100k-README.txt) which of around 1.256.Besides this PCS generated a utility matrix heatmap 

as well as a user vs ratings heatmap 

![Graph](https://i.imgur.com/Rtnfouk.png)

![Graph2](https://i.imgur.com/rBYwtJC.png)

## Compiling the code

The Engine can be used by running the file Main.py by which all the graphs will be stored in the selected directory

    $ python Main.pyn 
    
Now input the ratings from 1 to 5 of the displayed movies and the output will be the type of people with whom your movie tastes matches and you'll get your genre recomendations

    $ python gui.py

![code-suippet](https://i.imgur.com/IwGn0Ie.png)






