# Multivariate_Forecasting_LSTM_Restaurant

## Problem Statement:
- Predict top 'Menu Item' and 'Item Qty' for lunch and dinner.

- These predictions need to be for future dates (Monday to Sunday, July 1st to July 7th)

Visualization View: The candidate can best determine the visualization view which will clearly outline the predictions. Visualization example, just for reference...
Monday | Item | Qty | Menu Item | Lunch | Dinner
CHICKEN TIKKA MASALA | 15 | 22 |
CHICKEN BIRYANI | 5 | 10
KADAHI PANEER 12 18
GARLIC NAAN 20 40

### Background:

[R. Data - 1 tab.xlsx](https://github.com/Ashish-Gore/Multivariate_Forecasting_LSTM_Restaurant/blob/master/R.%20Data%20-%201%20tab.xlsx) as given data file.

- The dataset is for restaurant sales for Tuesday and Wednesday, both lunch and dinner time.

- There are few instances of 'To-Go' orders like Uber Eats in this dataset.

- typical lunch hour is 11:30AM-2:00PM, and dinner hour is 6:30PM-10:00PM

- some of the data is missing so is represented as 'na' in the data set

**The candidate needs to do below things to run the challenge successfully.**

- The data set is just for Tuesday and Wednesday.

- The candidate needs to expand and randomise the data for min. of 6 months (Jan. 2019 to June 2019) for all days of the week.

- A typical restaurant has high covers (number of customers) on Wednesday, Weekend Dinner, followed by Weekend Lunch and then relatively low covers for Monday to Friday Lunch.

- the data expansion/randomization should follow the above pattern for number of customers.


## Solution:

**Based on the Problem statement provided, Problem have been sub divided tasks in below 4 sections:**

[1.	Initial_EDA:](https://github.com/Ashish-Gore/Multivariate_Forecasting_LSTM_Restaurant/blob/master/1.%20Initial_EDA.ipynb)
This File Contains the EDA part for the initial excel file provided with 200 records.

[2.	Data Expansion:](https://github.com/Ashish-Gore/Multivariate_Forecasting_LSTM_Restaurant/blob/master/2.%20Data_Expansion.ipynb)
This file Contains the Codes to Expand the data randomly for the period of 6 months.

[3.	Model Building:](https://github.com/Ashish-Gore/Multivariate_Forecasting_LSTM_Restaurant/blob/master/3.%20Model_Building.ipynb)
This file contains 5 algorithms and 4 Meta Algorithms. And Hyper parameter Tuning using cross validation method for both Randomised Search cv and Grid Search CV.

[4.	Prediction using LSTM](https://github.com/Ashish-Gore/Multivariate_Forecasting_LSTM_Restaurant/blob/master/4.%20Prediction_using_LSTM.ipynb)
This File contains the Final Prediction with multiple output variables, as Structure described In the Problem statement. 

