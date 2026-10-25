# Time Series Analysis for Sales and Demand Forecasting
<div align="justify">
  
## 📝 **Objectives**   

1. To conduct a comprehensive analysis on select books from Nielsen's data, identifying key sales patterns that exhibit clear seasonal trends 
or other distinctive characteristics. 
2. To help develop a data-driven foundation for optimising procurement, re-ordering, and stocking decisions, 
ensuring efficient inventory management.

## 💡 **Business Context**

The Nielsen BookScan service is the world’s largest continuous book sales tracking service in the world which collects 
transactional data at the point of sale, directly from tills and dispatch systems of all major book retailers. 
This ensures detailed and highly accurate sales information on which books are selling and at what price, giving clients the most up-to-date 
and relevant data. 

Nielsen BookScan sales data can be analysed by various criteria, including category, publisher, and format,
allowing users to see which genres are selling in which format. Users can track market trends to see which titles are driving the results, 
and patterns can easily be interpreted. Some titles experience fluctuations in sales due to various factors, such as increased media attention or cultural relevance 
(e.g. the recent resurgence of interest in George Orwell’s 1984). However, certain books endure over time and are often studied in academic settings 
for their deeper significance.

For this project, Nielsen has provided us with two data sets. The objective is to identify sales patterns that demonstrate seasonal trends or any other traits, 
providing insights to inform reordering, restocking, and reprinting decisions for various books (by their International Standard Book Number, or ISBN).

## 📊 **Data Pre-processing Approaches**
* Resampled weekly sales data to ensure missing weeks were filled with zeros,
* Converted ISBNs to strings and dates to datetime objects,
* Filtered out ISBNs with sales data beyond 2024-07-01, 
* Investigated the general sales patterns across different time periods (1-12 years vs. 12-24 years),
* Focused on two specific books, *The Alchemist* and *The Very Hungry Caterpillar*, for a deeper analysis and sales forecasting.

## 🚀 **Methods Implemented**
* Performed time series decomposition, ACF/PACF analysis, and stationarity checks for both books.
* Used Auto ARIMA to identify the best model and forecast the final 32 weeks of data.
* Prepared the data for machine learning models.
* Created an XGBoost pipeline, tuned parameters using grid search, and forecast the final 32 weeks for both books.
* Built and tuned an LSTM model using KerasTuner, forecast the final 32 weeks of data, and evaluated the performance using MAE and MAPE.
* Applied both sequential and parallel hybrid models combining SARIMA and LSTM, tuned the models, and evaluated their performance using MAE and MAPE.
* Aggregated weekly data to monthly data, trained XGBoost and SARIMA models to forecast eight months, and compare results with weekly predictions.


## 📝 **Summary**
* Pre-processed a real industry data set to make it suitable for time series analysis.
* Applied various statistical tests to understand underlying characteristics of the data such as stationarity, seasonality and autocorrelation patterns.
* Performed time series decomposition to separate the data into trend, seasonal and residual components.
* Implemented time series forecasting models including classical and machine learning approaches.
* Fine-tuned the models to improve model performance.

## 📌 **Detailed Analysis**
A report outlining the analytical insights derived and the approaches undertaken for sales volume forecasting
is provided.

</div>
