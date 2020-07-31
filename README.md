# **TitanicPrediction**

Machine Learning model that can predict if a certain person were more likely to survive famous titanic shipwreck or not ?

From this you can clearly see this is Yes or No situation which means this is Binary Classification Problem

**Dataset from Kaggle Competition: https://www.kaggle.com/c/titanic/data**

After submiting to Kaggle.com this model scored 73.6% (0.736) accuracy score on final test dataset, which means this model could be surely improved but it achived my goal of 70% (0.7)

## Feature Importance 

**What is this?**

> Feature importance refers to techniques that assign a score to input features based on how useful they are at predicting a target variable

Here is an plot showing Feature Importance of this model

![Feature Importance](/markdown_imgs/feature_importance.png)

From this you can see that sex was the most important thing and this plot just proves it

![Sex Survived](/markdown_imgs/sex_survived.png)

This plot shows how many males vs females survived (from a training dataset), from this you can clearly see that being a female would give you higher chance to survive

## **Confusion Matrix**

Here is an Confusion Matrix describing performence on validation dataset

![Confusion Matrix](/markdown_imgs/confusion_matrix.png)

**What is an Confusion Matrix ?**

> Confusion matrix is a table that is often used to describe the performance of a classification model (or “classifier”) on a set of test data for which the true values are known. It allows the visualization of the performance of an algorithm.

Or in other words it allows us to see where is our model getting confused

## Models used to train this one

With this i tried 5 different models:

* RandomForestClassifier
* LinearSVC
* SVC
* KNeighbors
* Logistic Regression

From these 5 models, RandomForestClassifier showed up to be best for this task, here is an plot that proves it

![Best clf](/markdown_imgs/best_clf.png)

## Evaluation

Here is an evaluation plot with RandomForestClassifier that was used on a validation dataset, showing Accuracy, Precision, Recall and F1

![Evaluation plot](/markdown_imgs/evaluation.png)
