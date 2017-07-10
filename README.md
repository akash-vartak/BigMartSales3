# Big Mart Sales

## Problem Statement
This is as found on [Big Mart Sales 3 Problem Statement](https://datahack.analyticsvidhya.com/contest/practice-problem-big-mart-sales-iii/ "Big Mart Sales 3").

**The data scientists at BigMart have collected 2013 sales data for 1559 products across 10 stores in different cities.
Also, certain attributes of each product and store have been defined.
The aim is to build a predictive model and find out the sales of each product at a particular store.
Using this model, BigMart will try to understand the properties of products and stores which play a key role in increasing sales.**

## Data
We have train (8523) and test (5681) data set, train data set has both input and output variable(s).
We need to predict the sales for test data set.

## Data Dictionary
| Variable        | Description|
| :-------------: | :-------------: |
| Item_Identifier| Unique product ID|
| Item_Weight | Weight of product|
| Item_Fat_Content | Whether the product is low fat or not|
| Item_Visibility | The % of total display area of all products in a store allocated to the particular product|
| Item_Type | The category to which the product belongs|
| Item_MRP | Maximum Retail Price (list price) of the product|
| Outlet_Identifier | Unique store ID|
| Outlet_Establishment_Year | The year in which store was established|
| Outlet_Size | The size of the store in terms of ground area covered|
| Outlet_Location_Type | The type of city in which the store is located|
| Outlet_Type | Whether the outlet is just a grocery store or some sort of supermarket|
| Item_Outlet_Sales | Sales of the product in the particulat store. This is the outcome variable to be predicted.|

## Evaluation Metric Used
As stated on [Evaluation Metric](https://datahack.analyticsvidhya.com/contest/practice-problem-big-mart-sales-iii/ "Big Mart Sales 3").

## Submission
Submission needs to be in the format as shown in ["SampleSubmission.csv"](https://datahack-prod.s3.ap-south-1.amazonaws.com/sample_submission/SampleSubmission_TmnO39y.csv "Sample Submission Format").

## Summary
I have first calculated the least RMSE error on the train dataset for each of *RandomForestRegressor*, *GradientBoostingRegressor* and *XGBoost*
Then which ever model has least RMSE is used on test data. This is done so that the code runs optimised on private the data test.

## Rank
**As of 13th March, 2017**

This code was ranked 44/5129

RMSE: 1146.900301

RMSE of rank #1: 1135.203200
