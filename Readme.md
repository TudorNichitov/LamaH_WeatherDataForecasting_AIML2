
# Data Analysis with Pandas, Numpy, and ARIMA Forecasting

This repository contains code to load multiple CSV files, merge and process the data, analyze correlations, 
visualize the relationships, and perform ARIMA time series forecasting.

## Getting Started

### Prerequisites

Before you begin, ensure you have the following libraries installed:

- pandas
- numpy
- matplotlib
- statsmodels

You can install these using pip:

```
pip install pandas numpy matplotlib statsmodels
```

### Dataset

The dataset consists of multiple CSV files named as `ID_X.csv` where X is the ID of the dataset. Each file contains similar structured data, which is then concatenated into a single DataFrame.

### Code Structure

The code follows these steps:

1. **Loading Data**: Loads data from multiple CSV files into individual DataFrames and appends them to a list. An "Identifier" column is added for tracking the origin.
2. **Data Processing**: The individual DataFrames are concatenated into a single DataFrame, which is then sorted and cleaned.
3. **Visualization**: The correlations between columns are visualized, followed by scatter plots for pairs of features.
4. **Timestamp Formation**: Merges the year, month, and day columns into a single datetime column, which can then be used as a timestamp index.
5. **ARIMA Forecasting**: Splits the data into training and testing sets. An ARIMA model is then fit on the training data and forecasts are made on the test set. The predictions are visualized against the actual values.

## Running the Code

To run the code, open the provided Jupyter notebook or script and execute the cells in sequence.

## Results

The code concludes by plotting the predicted precipitation values against the actual values from the test set. The mean squared error (MSE) between the predictions and actual values is also computed.

## License

This project is licensed under the MIT License.

---

Note: The README is a general description of the project and does not cover all the details. It's important to customize and expand the README according to the specific needs and additional features of the project.