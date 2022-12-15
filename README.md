# Explore-Linear-models-on-weather-data-set
Comparing Linear &amp; Multilinear &amp; Polynomial Regression 
- Browsing the weather data set it contains 12 columns with different data types and I checked for duplicate rows and it turned out that there were 24 duplicate rows So, I removed them and for nulls there are over 500 rows with nulls in the Precip Type column but we won't be using them so I'll leave them
 I have selected the most correlated columns that affected the apparent temperature that I know from the Seaborn heatmap. So I create a new dataframe that only has five columns
- <img src = "https://user-images.githubusercontent.com/85246622/207987160-bd43c7b9-e6b8-40d1-a2fb-fad1edd179b0.png" width="400" height="400"/>
---------------------------------------------
- Next, to better understand the selected columns, I draw a scatterplot with 5 figures for each column versus the apparent temperature column, with 4 of them showing scattered random data
- <img src = "https://user-images.githubusercontent.com/85246622/207987723-1fb028b6-8780-40a8-8d1e-c38a84476ed4.png" width="400" height="400"/>
---------------------------------------------
- In the linear regression model, I first split the data into training and test sets, then do data normalization by MinMaxScaler, then fit the data into the sklearn linear regression model and predict the test set and get the R2_score and finally plot Scatterplot with line plot representing the line fitted  to the data
- <img src = "https://user-images.githubusercontent.com/85246622/207988296-039ca2e2-0b06-41c0-b79a-2bd41145efe3.png" width="400" height="400"/> 
- Finally, I print out the statistical models for the linear regression model to show the R-Squared, Adj.R-Squared, and F-Statistics
- <img src = "https://user-images.githubusercontent.com/85246622/207988691-914106f1-e7b4-4332-9756-965d5817c993.png" width="400" height="400"/>
--------------------------------------------- 
- Then in the multilinear regression we do  the same as above but use the dataframe with the five correlated columns and show the statistical models for the multilinear regression model
- <img src = "https://user-images.githubusercontent.com/85246622/207989016-89ec4c6d-c364-4080-8e92-d60a314d8b26.png" width="400" height="400"/>
---------------------------------------------
- Finally in the polynomial regression model we use the data with one column but  choose its degree to  4 and fit the data and predict the test set, then print the R2_score and show the statistical models for the polynomial of the regression model
- <img src = "https://user-images.githubusercontent.com/85246622/207989364-a98ccd74-71cc-40aa-9301-5a8d894b0e04.png" width="400" height="400"/>
