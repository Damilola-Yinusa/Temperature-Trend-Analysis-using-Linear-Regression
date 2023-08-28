# trend-analysis

# Temperature Trend Analysis using Linear Regression

This project demonstrates a simple temperature trend analysis using a Linear Regression model. It involves loading weather data into a Pandas DataFrame, normalizing numerical variables, calculating rolling statistics, identifying anomalies, and using Linear Regression to predict temperature trends.

## Getting Started

Follow these instructions to set up and run the project on your local machine.

### Prerequisites

- Python (>=3.6)
- Pandas
- NumPy
- Matplotlib
- Scikit-learn

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/Damilola-Yinusa/temperature-trend-analysis.git
   cd temperature-trend-analysis
   ```

2. Install the required packages:

   ```bash
   pip install pandas numpy matplotlib scikit-learn
   ```

### Usage

1. Place your weather dataset (e.g., 'seattle-weather.csv') in the project directory.

2. Open the Jupyter Notebook or Python script where you want to perform temperature trend analysis.

3. Copy and paste the code provided in the `temperature_trend_analysis.py` file into your Jupyter Notebook or script.

4. Modify the dataset path as needed:

   ```python
   df = pd.read_csv('seattle-weather.csv')  # Replace with the path to your dataset
   ```

5. Run the code to perform the temperature trend analysis.

## Explanation

This code performs the following steps:

1. Load the weather dataset into a Pandas DataFrame.
2. Normalize the numerical variables using Min-Max scaling.
3. Calculate the rolling mean of temperature over a 30-day window.
4. Calculate the standard deviation of the rolling mean.
5. Identify anomalies based on temperature deviations from the rolling mean.
6. Convert the date to numerical format for regression using the index.
7. Prepare the features (date) and target variable (temperature).
8. Initialize a Linear Regression model.
9. Fit the model to the data after handling missing values.
10. Make temperature predictions using the Linear Regression model.
11. Plot the original temperature data and the predicted trend line.

## Contributing

Contributions are welcome! If you have any improvements or suggestions, feel free to open an issue or a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
