**Seoul Bike Sharing Analysis**

**Project Overview**

The project aims to analyze bike sharing patterns in Seoul to improve the availability and accessibility of rental bikes, thereby reducing waiting times. 
The dataset includes weather information (Temperature, Humidity, Windspeed, Visibility, Dewpoint, Solar radiation, Snowfall, Rainfall), 
along with hourly bike rental counts and date information. 
The dataset was extracted from the UCI Machine Learning Repository: https://archive.ics.uci.edu/dataset/560/seoul+bike+sharing+demand

**Dataset Description**

The Seoul Bike Sharing Dataset includes hourly rental data spanning multiple years, featuring date, weather conditions, temperature, humidity, and bike rental counts.

**Data Analysis**

The analysis began with importing the dataset, checking data types, and performing descriptive statistics to determine the need for scaling.
Dummy variable encoding was used to convert textual data into numeric format, and the data was split into feature and target variables. 
Preprocessing included using MinMaxScaler to scale numerical features to a range between 0 and 1.
Feature selection was performed to remove features with low variance from the dataset. Different variance thresholds were tested,
and the data was split into training and testing sets. Training was conducted, and linear regression models were evaluated with variance thresholds.

**Evaluation Metrics**

Two models were built: one without feature selection and another with variance thresholding applied. 
Linear regression models were plotted, and RMSE was calculated to assess model performance.

**Conclusion**

The model with feature selection applied demonstrated a lower RMSE compared to the model without feature selection.
Future improvements could focus on real-time predictive modeling for demand forecasting and optimizing bike allocation strategies.
