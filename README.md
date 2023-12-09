# EnergyPrediction-Arima-Transformer

## 1) Energy Consumption.xlsx:

The provided dataset, Energy Consumption.xlsx, captures monthly energy consumption over a span of 50 years, from June 1970 to May 2020. Each data point in the Excel file represents the energy consumption value for a specific month. This comprehensive record serves as the foundation for the exploratory analysis and time series modeling conducted in the following Jupyter Notebooks.

## 2) Arima.ipynb:

This Jupyter Notebook is a crucial part of the Energy Consumption Prediction Project, encompassing the exploratory analysis. It includes a stationarity check using ADF tests, identification of trends and periodicity through visual inspection and decomposition, and the removal of trends and periodic components using techniques such as differencing, decomposition, or Fourier transformation. The notebook covers model selection considerations, such as ARIMA, SARIMA, or other advanced options, based on insights from the exploratory analysis. It also details model order estimation, evaluation using diagnostic tests on residuals, and selection criteria employing AIC and BIC. The forecasting stage involves predicting future values on a validation set, ensuring a robust and accurate approach to energy consumption prediction.

## 3) Transformer.ipynb:

The Jupyter Notebook presented herewith constitutes an integral component of the Energy Consumption Prediction Project, specifically tailored for time series analysis and deep learning methodologies. This document meticulously delineates an exhaustive feature extraction protocol encompassing lag features, rolling statistics, interaction features, seasonal features, rate of change, cumulative sum, exponentially weighted moving average (EWMA) statistics, additional statistics, z-scores, and log returns.
The modeling framework employed in this project embraces the Transformer model due to its adeptness in capturing temporal dependencies and handling irregular patterns inherent in time series data. Additionally, an LSTM neural network is implemented, providing a comparative analysis between the Transformer and LSTM models. The comparative evaluation reveals that the Transformer model surpasses the LSTM in predictive performance.
The subsequent phase of post-modeling evaluation incorporates an in-depth analysis, including Autocorrelation Function (ACF) and Partial Autocorrelation Function (PACF) assessments, Shapiro-Wilk tests, and histogram distribution analysis for residuals. These analytical measures collectively contribute to a comprehensive understanding of the model's performance and adherence to underlying statistical assumptions.

## Instructions for Usage:

1. **Upload Energy Consumption.xlsx to Google Drive:**
   - Before running the Jupyter Notebooks, ensure that the Energy Consumption.xlsx file is uploaded to your Google Drive.

2. **Run the Following Code to Load Data:**
   ```python
   import pandas as pd

   # Replace '/content/drive/MyDrive/Energy Consumption.xlsx' with the path where you uploaded the file.
   data_df = pd.read_excel('/content/drive/MyDrive/Energy Consumption.xlsx')
   
   columns_name = ['Energy Consumption']
   Data = pd.DataFrame(data_df, columns=columns_name)
   ```
   - Execute this code to load the dataset for analysis in the Arima.ipynb and Transformer.ipynb notebooks.

3. **Explore and Analyze:**
   - After loading the data, run the provided Jupyter Notebooks to explore the dataset, perform in-depth analysis, and make energy consumption predictions.

By following these instructions, you'll be ready to delve into the Energy Consumption Prediction Project and harness the power of Arima.ipynb and Transformer.ipynb for accurate and insightful predictions.
