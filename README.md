# ML_TCM_SVM
2023 Fall Machine Learning Team 13 Final Project.
This is the model built by SVM.

## Step 1. Package import
Import the necessary packages.

## Step 2. Data preparation
1. Read data from the .csv file as a Pandas DataFrame.
2. Change the columns with texts into numeric values using LabelEncoder.
3. Split the data into the status/diagnoses/symptoms and the prescriptions.
4. Delete the CHMs that are not often used enough.
5. Split the data into training data and validation data.

## Step 3. Build the SVM model
For information about sklearn SVC, go to: [sklearn.svm.SVC](https://scikit-learn.org/stable/modules/generated/sklearn.svm.SVC.html)
1. **Build the SVM models.**
    - Type 1: Multiple models: Build models according to every single column.
    - Type 2: MultiOutputClassifier model: Build the model according to all the columns.
    - Type 3: Weighted model: Build the weighted model to handle the imbalanced data.
2. **Use the model to predict the data.**
3. **Evaluate the model's performance**
    - Including the accuracy and the f1-score.

## Step 4. Main code and model training
Use the code implemented above to train the model.
