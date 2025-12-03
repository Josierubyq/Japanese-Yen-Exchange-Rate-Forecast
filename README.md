# Japanese Yen Exchange Rate Forecast
## 1.Data set definition

This project uses a dataset containing data on the exchange rate of the Japanese yen against the U.S. dollar, with the file name “JPY_Japanese-Yen.csv”. This dataset records daily exchange rate changes from the beginning of 1996 to May 2024, including information on opening price, high price, low price, closing price, and volume. The data span a wide range of time frames and can be used to analyze trends and patterns over time.
https://www.kaggle.com/datasets/usamabuttar/global-currency-historical-prices-updated-daily

## 2.Project objectives.

- Explore the yen-dollar exchange rate data and examine trends, seasonality and anomalies in it.
- Evaluate the smoothness of the data and perform appropriate transformations to meet modeling assumptions where necessary.
- Use different time series forecasting models (e.g., ARIMA, SARIMA) to forecast future exchange rate changes.
- Compare the forecasting performance of different models, select the best model and explain its advantages.
- Based on the model, forecast the exchange rate movement in the future period. 3.

## 3.Research questions.

- Is there a significant upward or downward trend in the exchange rate data of the yen against the U.S. dollar?
- Is there a significant cyclical or seasonal pattern in the exchange rate data?
- What specific events or periods have had a significant impact on the exchange rate?
- Which time-series model can be used to most accurately characterize and forecast the exchange rate data?
- How will the exchange rate change over time based on the forecasting model?

## 4.Preliminary data analysis.

Before starting the modeling, a thorough exploratory analysis of the data was first conducted, including.

- Checking the size, column names and data types of the dataset.
- Reviewing the first few rows of the data set to understand its structure and content.
- Calculating descriptive statistics such as mean, median and standard deviation.
- Identify and deal with missing values and interpolate missing values using linear interpolation.
- Plot time series graphs to visualize exchange rate trends.
- Calculate rolling averages and expanded averages to smooth data and better visualize trends.
- Use heat maps to visualize monthly and yearly exchange rate patterns.
- Plot scatter plots to see the relationship between opening and closing prices.
- Calculate correlation coefficients to analyze the correlation between variables.
- Plotting the autocorrelation function (ACF) and partial autocorrelation function (PACF) to investigate the time dependence of the data.

These preliminary analyses provide us with knowledge about the structure, distribution and pattern of the data, and lay the foundation for subsequent modeling work. Some important events are also labeled to better explain exchange rate fluctuations.

Next, several simple baseline forecasting methods, such as the mean, plain and drift methods, were explored and their evaluation metrics were calculated for comparison with more sophisticated models.

Then, more advanced time series modeling techniques, including methods such as ARIMA and SARIMA, were attempted. These models are capable of capturing autoregressive, moving average and seasonal patterns in the data, thereby improving forecasting accuracy. The performance of the different models was evaluated and the best model was selected.

Using the SARIMA model, we have forecasted the exchange rate changes in the coming month and compared and visualized the forecast results with the historical data.

Finally, use LSTM, CNN, MLP to forecasted the exchange rate, and also import two new dataset,US Bond Yield and Japan Bond Yield.

Calculate Interest Rate Differential:

For each date, compute the differential between the U.S. Bond Yield and the Japan Bond Yield:

Bond_Yield_Diff = US_Bond_Yield - Japan_Bond_Yield.

Use Interest Rate Differential in Predictions:

Incorporate the calculated interest rate differential as an input feature, combined with JPY/USD exchange rate data, into the model to perform multi-step predictions of the exchange rate.

Overall, the aim of this project is to gain a deeper understanding of the yen-dollar exchange rate data, identify patterns and influencing factors, and provide reliable forecasts of future exchange rate changes through exploratory analysis and time series modeling methods.
