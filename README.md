# Projet SY09 - Data Science

## Intro
This repository contains my work developed in the course SY09 - Data Science at the Technological University of Compiègne. The project was developed by 3 students, but here it contains only my part of the work and all the code written by me. The data was provided by the teacher and is available at https://archive.ics.uci.edu/ml/datasets/Crowdsourced+Mapping

The aim of the study was to apply all concepts and techniques seen in class to create a complete analysis of data science and define the best classification model for a series of satellite images. Our data set was composed of several landscape satellite images labeled with the landscape class. The entire process used to reach our conclusions is described in the report available in the repository.

## Personnal contribuition to project
### Exploratory Analysis
In this part, I tried to provide the team with insights into the data and then try to explain our further decisions in the project. The analysis also helped to better understand the problem and see which points are interesting to study. An interesting point that we noticed is that max_ndvi can be used to separate classes. The distribution of each class is in accordance with the definition of NDVI, where regions with greener have higher values of NDVI as shown below.

<img src="https://github.com/gabrielsouzaesilva/sy09-imgsat/blob/master/imgs/max_ndvi_dist.png">

This phase of our project was the basis for understanding the data and the problem and was crucial for our final analysis. All details [here]{https://github.com/gabrielsouzaesilva/sy09-imgsat/blob/master/analyseExploratoire.ipynb}

### Model Selection
In this part I made a pipeline to evaluate some models seen in class. The models chosen were: LDA, QDA, Naive Bayes and KNN. The purpose of this part is to apply the methods to our dataset, evaluate them and justify the choice of the best algorithm. The pipeline consists of the cross-validation with 5 different subsets of sizes from 10% to 100% of the training data. Each cross-validation works with 10 splits and a test size used is equal to 20% of the data set. This gives us the test and train scores of a model, and also a good view of the work of the model and how it changes with variation of the data. The image below simplyfies the model selection pipeline.

<img src="https://github.com/gabrielsouzaesilva/sy09-imgsat/blob/master/imgs/modelEval.png">

All details [here]https://github.com/gabrielsouzaesilva/sy09-imgsat/blob/master/modelPipe.ipynb
