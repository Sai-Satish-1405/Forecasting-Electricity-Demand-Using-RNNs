# Forecasting-Electricity-Demand-Using-RNNs
Forecasting Electricity Demand Using RNNs

Project Proposal 
Forecasting Electricity Demand Using RNNs
Sai Satish Pallapolu - 11753831

Purpose and Story: 
I wanted to forecast electricity demand. This is very important for the energy grid, especially today when we use more renewable energy for an instance like solar and wind. The key challenge with renewables is that it is not every time predictable, so we need to forecast how much electricity can be required. These things will aid in keeping the grid stable, enhancing energy production and lowering the costs.
In the current project, we are going to forecast the electricity demand for each hour making the use of past data. This can assist energy system managers to make better choices regarding energy thus enhancing system efficiency and eco-friendliness.

Data Set Summary
Data Source:
I will use data from the U.S. Energy Information Administration (EIA) which are the "BALANCE" files between 2022 and 2025. These files comprise of hourly data on electricity production, demand and sharing among the various U.S regions. It’s trustworthy and fine for time-based forecasting.


Link to Data Source:
EIA Electricity Data https://www.eia.gov/electricity/gridmonitor/dashboard/electric_overview/US48/US48
Data can be downloaded from the above-mentioned website by navigating to Download Data > Six Months Files > Balance Jan to June, June to Dec from 2023-25. All the files are being upload to drive link given below EIA Electricity Data .

Target Variable:
		Demand (MW): The actual electricity demand for the hour. This target variable is forecasted for the upcoming years based on the previous historic data.

Research Questions:
1.	Can we forecast hourly electricity demand by making use of past data?
2.	What are the key patterns in usage of electricity? (for instance, daily, weekly, seasonal)
3.	Will the holidays and temperature aid in enhancing the model?


Data Set:
Variables in the data
1.	Balancing Authority:  It represents the group whose responsibility is controlling the grids (like AECI).
2.	Data Date: It refers to the recorded data date.
3.	Hour Number: It represents the hour of the day ranges from 1 to 24.
4.	Local Time at End of Hour: It defines the local time of a region when the hour concludes.
5.	UTC Time at End of Hour: It refers to the UTC time when the hour concludes.
6.	Demand Forecast (MW): It represents the forecasted electricity demand for that hour.
7.	Demand (MW): It implies to the actual demand of current for that hour (we want to forecast this).
8.	Net Generation (MW): It’s the amount of electricity generated in the region.
9.	Total Interchange (MW): It defines the way of electricity being imported or exported from the regions.
10.	Net Generation by Fuel Type: To produce electricity which type of energy is employed (such as coal, solar etc.).
11.	Region: It represents a particular area in the country U.S.A(like MIDW for Midwest).
Other characteristics to add:
Temperature (°F): It defines the average temperature for a particular region. This can be achieved using a weather API.
Day of Week: It represents which day (like Monday, Tuesday).
Holiday Indicator: If it’s a holiday or not (1 for holiday, 0 for not).

Data Size:
		This dataset comprises of data for approximately 3 years from 2022 to 2025 with hourly data around 43,800 data points from each region. For making analysis and training the model this will be sufficient. 

Why we choose this data:
•	As it is taken from a trusted government agency which ensures reliability.
•	It comprises of hourly records allowing for better analysis on the patterns.
•	It provides insights on how much energy is produced and exchanged aiding to understand electricity demand efficiently.



