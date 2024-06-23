Logistic Regression for Stock Price Movement Prediction
This project utilizes logistic regression to predict whether the stock price will increase or decrease in the next 30 days based on historical stock data.

Overview
The project involves:

Loading historical stock price data from a CSV file.
Preparing the data for logistic regression modeling.
Training a logistic regression model to predict stock price movements.
Evaluating the model's performance using accuracy, confusion matrix, and classification report.
Making predictions for the next 30 days and visualizing the results.
Features
Loading Data: Reads and preprocesses historical stock price data.
Data Preparation: Creates a target variable indicating whether the stock price will rise (1) or fall (0) in the next 30 days.
Model Training: Splits the data into training and testing sets, trains a logistic regression model.
Model Evaluation: Computes accuracy, confusion matrix, and classification report to evaluate model performance.
Future Predictions: Predicts future stock price movements for the next 30 days.
Visualization: Plots actual closing prices and marks predicted stock movements.
Requirements
Python 3.7 or higher
pandas
numpy
matplotlib
scikit-learn
Installation
Clone the repository or download the script file.

Install the required Python packages:

bash
Copy code
pip install pandas numpy matplotlib scikit-learn
Usage
Prepare your CSV file with at least two columns: Date and Close. The Date column should contain the dates of the stock prices, and the Close column should contain the closing prices of the stock.

Update the csv_file variable in the script with the path to your CSV file:

python
Copy code
csv_file = "your_stock_data.csv"  # Replace with your CSV file path
Run the script:

bash
Copy code
python logistic_regression_stock_prediction.py
The script will output the model's accuracy, confusion matrix, and classification report.

It will also print the predicted stock movements (1: Up, 0: Down) for the next 30 days.

Additionally, it will display a plot comparing the actual closing prices with the predicted stock movements.

Example
Here is an example of what the CSV file should look like:

csv
Copy code
Date,Close
2020-01-01,300.35
2020-01-02,302.56
2020-01-03,298.44
...
Code Explanation
Load Data: The load_data function reads the CSV file and processes the date and closing price columns.

Prepare Data: The prepare_data function creates a target variable (Target) indicating whether the stock price will rise or fall in the next 30 days.

Train and Evaluate Model: The train_and_evaluate_model function splits the data into training and testing sets, trains a logistic regression model, and evaluates its performance using accuracy, confusion matrix, and classification report.

Make Predictions: The make_predictions function predicts the stock movements for the next 30 days based on the trained model.

Plot Results: The plot_results function plots the actual closing prices and marks the predicted stock movements.

License
This project is licensed under the MIT License.
