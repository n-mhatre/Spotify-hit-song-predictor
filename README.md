# Spotify-Hit/Miss-song-predictor

This project aims to predict whether songs will be hits or misses using a Spotify dataset spanning from the 1960s to the 2010s. Employing Logistic Regression, Support Vector Machines (SVM), Random Forest, and Ensemble methods, the project entails thorough data preprocessing, hyperparameter optimization, model evaluation, and comprehensive result analysis.

## Table of Contents
- [Introduction](#introduction)
- [Data](#data)
- [Preprocessing](#preprocessing)
- [Logistic Regression](#logistic-regression)
- [Support Vector Machines](#support-vector-machines)
- [Random Forest](#random-forest)
- [Ensemble Techniques](#ensemble-techniques)
- [Model Evaluation](#model-evaluation)
- [Conclusion](#conclusion)
- [Future Improvements](#future-improvements)

## Introduction

Predicting song success is pivotal in the music industry. This project leverages machine learning to classify songs as hits or misses based on diverse Spotify dataset features.

## Data

Spanning from the 1960s to the 2010s, the dataset encompasses songs with attributes such as danceability, energy, and tempo. The binary target variable distinguishes hit songs (1) from misses (0).

## Preprocessing

Key steps in preprocessing include:
- Eliminating irrelevant categorical variables: 'track', 'artist', 'uri'.
- Stratifying data into training, validation, and test sets.
- Standardizing feature scales to ensure consistency.
- Managing data integrity without missing values.

## Logistic Regression

Exploring various solver strategies and regularization settings, Logistic Regression models hint at the dataset's potential linear separability, impacting model performance minimally.

## Support Vector Machines

Employing kernels (linear, polynomial, sigmoid, RBF), SVM models reveal RBF's superior capability in handling complex data patterns. Tuning hyperparameters (C and gamma) optimizes model efficacy.

## Random Forest

Through varying hyperparameters (n_estimators, max_depth), Random Forest models uncover feature importance, shedding light on attributes influencing predictions.

## Ensemble Techniques

Utilizing Voting and Stacking, models like Logistic Regression, SVM, and Random Forest combine predictions. Hard and soft Voting methods are explored, with Stacking incorporating AdaBoost and GradientBoosting as final estimators.

## Model Evaluation

The standout model, Stacking with GradientBoosting as the final estimator, achieves compelling metrics on the test dataset: accuracy (0.8069), recall (0.8457), and precision (0.7881).

## Conclusion

This project showcases machine learning's efficacy in predicting song success based on audio attributes. Stacking with GradientBoosting emerges as a robust choice, delivering competitive accuracy and precision in classifying songs.

## Future Improvements

Enhancing model generalization via expanded dataset size, exploring additional features or transformations, and conducting further hyperparameter fine-tuning promise to advance predictive performance. Exploring advanced ensemble techniques and architectures holds potential for further gains.