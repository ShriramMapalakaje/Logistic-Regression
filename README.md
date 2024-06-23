
# Logistic Regression for Stock Price Movement Prediction

This project utilizes logistic regression to predict whether the stock price will increase or decrease in the next 30 days based on historical stock data.

## Key Features

- **Data Preparation**: Processes historical stock price data from a CSV file, creating a target variable indicating upward or downward movement.
  
- **Model Training**: Splits the data, trains a logistic regression model, and evaluates its performance using accuracy, confusion matrix, and classification report.

- **Predictions**: Generates predictions for the next 30 days and visualizes the results comparing actual closing prices with predicted movements.

## Requirements

- Python 3.7 or higher
- Libraries: pandas, numpy, matplotlib, scikit-learn

## Installation

1. Clone the repository or download the script file.

2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib scikit-learn
   ```

## Usage

1. Prepare your CSV file (`your_stock_data.csv`) with columns `Date` and `Close`.

2. Update `csv_file` variable in the script:
   ```python
   csv_file = "your_stock_data.csv"
   ```

3. Run the script:
   ```bash
   python logistic_regression_stock_prediction.py
   ```

4. Outputs:
   - Model accuracy, confusion matrix, and classification report.
   - Predicted stock movements (1: Up, 0: Down) for the next 30 days.
   - Plot comparing actual closing prices with predicted movements.

## Example Data Format

```csv
Date,Close
2023-01-01,350.45
2023-01-02,355.20
2023-01-03,358.90
...
```

## Code Snippet Explanation

- **Load Data**: Reads CSV file and processes date and closing price columns.
- **Prepare Data**: Creates target variable based on future stock price movement.
- **Train and Evaluate Model**: Splits data, trains logistic regression, and evaluates performance.
- **Make Predictions**: Predicts future stock movements.
- **Plot Results**: Visualizes actual vs. predicted stock movements.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

