# Stock Price Prediction using LSTM

This project provides a comprehensive solution for predicting stock prices using Long Short-Term Memory (LSTM) neural networks. The project utilizes historical stock data, preprocesses it, trains an LSTM model, and makes future predictions.

## Features

- Fetches historical stock data using `yfinance`.
- Preprocesses data and computes hourly percentage changes.
- Scales data using `MinMaxScaler`.
- Creates a dataset for training and testing the LSTM model.
- Trains an LSTM model with the option to save the model and scaler.
- Makes predictions and evaluates model performance.
- Plots historical data, model predictions, and future predictions using Plotly.

## Requirements

- Python 3.6+
- `numpy`
- `pandas`
- `yfinance`
- `sklearn`
- `tensorflow`
- `plotly`
- `joblib`

## Setup

1. **Clone the Repository:**

    ```sh
    git clone https://github.com/yourusername/stock-price-prediction-lstm.git
    cd stock-price-prediction-lstm
    ```

2. **Install Dependencies:**

    ```sh
    pip install numpy pandas yfinance scikit-learn tensorflow plotly joblib
    ```

## Usage

1. **Run the Script:**

    Execute the script by running:

    ```sh
    python stock_prediction.py
    ```

    You will be prompted to enter a stock symbol. The script will then fetch the historical stock data, preprocess it, train the LSTM model, and make predictions.

2. **Inputs:**

    - `stock_symbol`: Enter the stock symbol for which you want to make predictions.

3. **Outputs:**

    - The trained model and scaler are saved in the specified directory.
    - The script prints the Root Mean Squared Error (RMSE) for the predictions.
    - A Plotly graph is displayed, showing historical data, model predictions, and future predictions.

## Example

1. **Stock Symbol Input:**

    ```sh
    Please enter a stock symbol: AAPL
    ```

2. **Output:**

    - The RMSE of the model's predictions.
    - Plotly graph showing historical data, model predictions, and future predictions.

## Functions

- `create_dataset(data, time_step)`: Prepares the dataset for training and testing.
- `save_model_and_scaler(model, scaler, symbol, directory)`: Saves the trained model and scaler to the specified directory.
- `main()`: Main function to execute the workflow from fetching data to making predictions and plotting results.

## Contributing

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -m 'Add feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a Pull Request.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## Contact

For any questions or support, please contact [your_email@example.com](mailto:your_email@example.com).
