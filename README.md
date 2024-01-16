# Traditional Chinese Medicine Training using Support Vector Machine Model
2023 Fall Machine Learning Team 13 Final Project.
This is the model built using SVM.

## About This Repository
This repository serve for demonstrating training a support vector machine model for traditional chinese medicine prescription prediction.

## Setup instructions
There are 3 packages imported in this project: **pandas, numpy, and sklearn**.
So please make sure that you've already installed them.

You can install them by using pip:
```
pip install pandas numpy sklearn
```
## Data Source
The data used to train the model is process_data.csv

## Code execution instructions
The model is in tcm_svm.ipynb. You can follow the steps in the notebook.<br>
There is detailed information above every code block to indicate their use.<br>
The last 2 code blocks are about hyperparameter tuning, so you don't need to run them.

## Model performance details
The f1-score of the testing data is around 0.4 ~ 0.6, mainly affected by the balance of the data.<br>
In other words, if the data of a medicine contains the 1s as many as the 0s, it tends to have a higher f1-score.

## Model output examples
There are 2 variables in the naming of the directories: **Model kind and threshold**.<br>
The naming convention of the directories is **{Model kind}_{threshold}**.<br>
Model kind stands for the different ways to build the SVM models.<br>
Model kind 2 does not exist since it has the same output as mode kind 1.<br>
Threshold stands for how many times the medicines are used at least.<br>
For example, if the threshold is 100, it means all the medicines in it are used at least 100 times.

There are 2 .csv files under a directory, which stands for the result of training data and testing data.<br>
The naming convention of the files is **{file kind}{Model kind}_{threshold}.csv**, while file kind is either "train" or "test".<br>
For example, "test3_250.csv" is the testing data's result of the SVM model with model kind 3 and threshold 250.<br>
