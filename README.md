# Admission Prediction Model

This is a Python script that implements a machine learning model for predicting admission chances based on certain features. It includes both regression and classification approaches.

## Dependencies

The script requires the following dependencies:

- pandas
- scikit-learn
- seaborn
- numpy
- joblib

You can install these dependencies using pip:

```shell
pip install pandas scikit-learn seaborn numpy joblib
```shell

## Usage

Ensure that the dataset file 'Admission_Predict.csv' is present in the same directory as the script.

Run the script using a Python interpreter.

```shell
python admission_prediction_model.py
```

The script performs the following steps:

##Regression
- Loads the dataset using pandas.
- Displays the top 5 and bottom 5 rows of the dataset.
- Prints the shape of the dataset.
- Provides information about the dataset.
- Checks for null values in the dataset.
- Displays overall statistics about the dataset.
- Removes the 'Serial No.' column as it is irrelevant.
- Splits the dataset into training and testing sets.
- Performs feature scaling on the training and testing sets.
- Imports the required regression models (Linear Regression, SVR, Random Forest Regressor, Gradient Boosting Regressor).
- Trains each model on the training data.
- Makes predictions on the testing data using each trained model.
- Evaluates the accuracy of each model using the R2 score.

###Displays a bar plot showing the R2 scores of each model.

## Screenshots of Project
![Screenshot (864)](https://github.com/shreyansh28801/AddmisionPredictionModel/assets/81692600/2846ffee-afb5-4b50-8f9e-477ff2847fc3)

##Classification

- Converts the target variable into a categorical value for classification.
- Imports the required classification models (Logistic Regression, SVM, K-Nearest Neighbors, Random Forest Classifier, Gradient Boosting Classifier).
- Trains each model on the training data.
- Makes predictions on the testing data using each trained model.
- Evaluates the accuracy of each model.

###Displays a bar plot showing the accuracy scores of each model.

## Screenshots of Project
![Screenshot (863)](https://github.com/shreyansh28801/AddmisionPredictionModel/assets/81692600/54a2a0c8-e765-4203-821e-7f35369a4b9e)

##Model Saving
- Saves the trained Gradient Boosting Classifier model using joblib.
- Loads the saved model.
- Makes a prediction using the loaded model on a sample input.
