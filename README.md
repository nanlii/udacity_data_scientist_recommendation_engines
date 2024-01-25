# udacity-data-scientist
[**Udacity Data Scientist NanoDegree Program**](https://www.udacity.com/course/data-scientist-nanodegree--nd025)

`Project 3- Recommendation Engines`
## Table of Contents

1. [Introduction](#introduction)
2. [Installation](#installation)
3. [Project Motivation](#motivation)
4. [File Descriptions](#files)
5. [Results](#results)
6. [Licensing, Authors, and Acknowledgements](#licensing)

## Introduction <a name="introduction"></a>
This is the third project of the [**Udacity Data Scientist NanoDegree Program**](https://www.udacity.com/course/data-scientist-nanodegree--nd025).

For this project, I will analyze the interactions that users have with articles on the `IBM Watson Studio platform`, and make recommendations to them about new articles.

The recommendation system and method used in the project:
1. Rank Based Recommendations
2. Collaborative Filtering Based Recomendations
3. Similarities
4. Matrix Factorization


## Installation <a name="installation"></a>

1. Mac or Windows System
2. [Anaconda Distribution](https://docs.anaconda.com/free/anaconda/index.html)
3. Libraries: Numpy, Pandas, Matplotlib
4. Packages in the workspace: project_tests, pickle

## Project Motivation <a name="motivation"></a>

In the IBM Watson Studio, there is a large collaborative community ecosystem of articles, datasets, notebooks, and other A.I. and ML. assets. Users of the system interact with all of this. 
In this project, I created several recommendation systems in order to determine the potential improvements of different reocmendation methods. 

## File Descriptions <a name="files"></a>
.
├── Recommendations_with_IBM.html #html version notebook
├── Recommendations_with_IBM.ipynb #jupyter notebook with all the analysis
├── __pycache__
│   └── project_tests.cpython-39.pyc
├── data
│   ├── articles_community.csv
│   └── user-item-interactions.csv
├── project_tests.py
├── read_me_template
├── top_10.p
├── top_20.p
├── top_5.p
└── user_item_matrix.p

## Results<a name="results"></a>
There are several approaches to further determine if the recommendation systems are an improvement:

1. Take the system online for A/B Testing - The most intuitive way to determine the model performance is to take the matrix factorization recommendation system online for a set of users as experimental group, use rank based recommendation for control group, and then compare the article view rates between control and experimental groups.

2. While taking the model online for a small set of users, keep collecting user viewing data. One of the reasons it is hard to make the determination is lake of data, therefore it is important increase the number of users for testing.

3. In real world practice, we also combine A/B testing and questionnaires together to understand performances. It is also a good approach to ask uses feedback once we take the recommendation systems online.

## Licensing, Authors, Acknowledgements<a name="licensing"></a>
This project is part of the Udacity Data Scientist Nano Degree Program, and I'm using the data provided by [IBM](https://dataplatform.cloud.ibm.com/)

Thank you :love_you_gesture: