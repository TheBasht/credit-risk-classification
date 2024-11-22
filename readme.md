# README

## About this Codebase

This codebase is for analyzing loans to see if they are healthy (`0`) or high-risk (`1`). It uses machine learning to make predictions based on financial data like loan size, interest rate, income, and more. 

## What It Does

1. Loads loan data from a CSV file.
2. Splits the data into training and testing groups.
3. Trains a Logistic Regression model to predict loan status.
4. Checks how good the model is with accuracy, precision, recall, and a confusion matrix.
5. Shows if the model is useful for the company.

## Files

- `lending_data.csv`: The data with all loan information.
- Main script: Code for training the model and checking its results.

## How to Use

1. Make sure you have Python and required libraries installed (`pandas`, `numpy`, `sklearn`).
2. Run the script to load the data, train the model, and see the results.
3. Check the confusion matrix and classification report to understand the predictions.

## Results

- The model predicts healthy loans (`0`) very well.
- It is not as good at finding high-risk loans (`1`), but it still helps.
- You can improve the model or use it as it is, dependin
