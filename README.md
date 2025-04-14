# Lab-2
MGT 665 - Lab 2

# Student Success Classifier
## Abstract
The goal of this project was to train and fit a data set for various classification models. The models used in this study were Logistical Regression, k-Nearest Neighbor and a Decision Tree. 

## Introduction
Given the demographics of 316 students, I wanted to create a model to help identify individuals who are struggling with school. 

## Related Work
Serhat ran a study using a different data set and using KNN to determine student success. He was able to achieve a 95% accuracy score. The data he used was much more linear and showed a stronger correlation, than the data used in my study. 

## Methodology
The first big step in understanding the key indicators for a struggling student was to create a correlation matrix. This helped me identify which variables heavily correlated with student success. Once these variables were picked, it was time to train the models. In order for the classifiers to work, all text had to be converted to binary. I did this by classifying any student with more than 0 class fails, to be "failed". Then, I converted "failed" to 0 and 1's by using the get_dummies function in pandas. 

## Results
Of the three models tested, the best model was the logistic regression. The accuracy came out to 62% which is not the worst, but is not great. 

## Discussion
Looking back at the results, the data used to predict whether a student would fail a class or not  was terrible. Most of the correlation matrix was below 10% correlation, meaning the AI models were almost just randomly guessing whether the student would fail or not. The other models, scored higher; however, the AI never predicted any student to fail. Given the data split for a student failing a class was 61/316.

## References
Çoban, S. (2023, June 26). Knn example. Kaggle. https://www.kaggle.com/code/fizikciserhat/knn-example 
