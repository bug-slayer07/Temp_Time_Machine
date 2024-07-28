# Temp_Time_Machine

# CS F320 - Foundations of Data Science
## Capstone project

# Maximum Temperature Forecasting using ARIMA

This project involves forecasting maximum temperatures using data collected from a weather detection app and then deploying an ARIMA (AutoRegressive Integrated Moving Average) time series analysis model. The project pipeline includes data collection, preprocessing, exploratory data analysis, model development, and performance evaluation.

## Project Overview

- **Objective**: To forecast maximum temperatures and compare model predictions with weather app forecasts.
- **Methods**: ARIMA model for time series forecasting, linear interpolation for missing value imputation, exploratory data analysis (EDA).

## Data Collection

- Collected maximum temperature data over 40 days.
- Organized data into four columns: actual temperature as observed on the present day and the follwing next three days forecast.
- While the data collection process was subjected to special care and emphasis, it was not collected for a few days.
- Imputed missing values using linear interpolation.

## Exploratory Data Analysis (EDA)

- Calculated descriptive statistics: mean, median, and mode.
- Visualized temperature distribution and patterns using histogram plots.
- Analyzed trends and seasonality in the time series data.

## Model Development

- Implemented ARIMA model using the first 3 days and first 27 days of historical data to forecast temperatures for the next 3 days.
- Evaluated model accuracy by comparing predictions with weather app forecasts.
- Calculated Mean Absolute Error (MAE) for performance assessment.

## Key Findings

- Larger datasets (27 days) improved model performance by capturing more intricate patterns and trends compared to smaller datasets (3 days).
- This demonstrates the impact of data volume on forecasting accuracy through autocorrelation analysis.

## Usage

1. **Data Preparation**: Ensure data is collected and organized as described.
2. **EDA**: Perform exploratory data analysis to understand data characteristics.
3. **Model Implementation**: Use ARIMA model for forecasting.
4. **Evaluation**: Compare predictions with actual data and calculate MAE.

## Repository Structure

- `Collected_Data`: Collected Maximum temperature data.
- `Cleaned_Data` : Cleaned data.
- `ARIMA`: Jupyter notebook for ARIMA model implementation and evaluation.
- `Exploratory_Data_Analysis`: Cleaning and preprocessing of data.
- `README.md`: Project overview and instructions.

## Requirements

- Python 3.11.0
- Libraries: pandas, numpy, matplotlib, statsmodels

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/bug-slayer07/Temp_Time_Machine.git
    cd Temp_Time_Machine
    ```

2. Install the required libraries:
    ```bash
    pip install pandas
    pip install numpy
    pip install matplotlib
    pip install statsmodels
    pip install jupyter
    ```

## Running the Project
1. Ensure `Collected_data.csv` is in the root directory.
2. Launch Jupyter Notebook in your local IDE or google colab.
3. Open `Exploratory_Data_Analysis.ipynb` to perform exploratory data analysis.
4. Open `ARIMA.ipynb` to implement the ARIMA model and evaluate its performance.
