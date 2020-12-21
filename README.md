# House Price Prediction
 EDA & Regressional Analysis on Kaggle House Price dataset

## Description

In this notebook, I did an exploratory data analysis and a regressional analysis using **XGB Regressor** on Kaggles [Hotel Booking dataset](https://www.kaggle.com/jessemostipak/hotel-booking-demand). Specifically, I 

 - analyzed the **general shape and columns** of the dataset
 - created **a heatmap with correlation matrix** to see how the variables are correlated,
 - made **bivariate data analysis** with columns that have high correlation with the price of a house,
 - checked **outliers for 3 quantitative variables**,
 - evaluated **3 regression models** with root mean squared log error and chose XGB Regressor, and
 - predicted **the price of a house** using other features of a house.
 
After creating additional variables and tuning the paramaters, the model achieves a **root mean squared log error of 0.12717** on the test set and is ranked at Top **12%** of all models submitted to the competition. 

## EDA Samples

Here are some of properties of the dataset I examined

<p align="left">
  <img width="800" height="120" src="https://github.com/RandomY-2/House_Price_Prediction/blob/main/images/data_shape.jpg">
</p>

<p align="left">
  <img width="800" height="300" src="https://github.com/RandomY-2/House_Price_Prediction/blob/main/images/data_missing.jpg">
</p>

<p align="left">
  <img width="800" height="600" src="https://github.com/RandomY-2/House_Price_Prediction/blob/main/images/heatmap.jpg">
</p>
 
<p align="left">
  <img width="800" height="600" src="https://github.com/RandomY-2/House_Price_Prediction/blob/main/images/overallcond_price.jpg">
</p>

<p align="left">
  <img width="800" height="200" src="https://github.com/RandomY-2/House_Price_Prediction/blob/main/images/totalBsmt_box.jpg">
</p>

 ## Prediction
 
I first compared three regression models(RandomForest Regressor, XGB Regressor, and AdaBoostRegressor) and selected XGB Regressor because it has the best baseline performance. 

(RMSLE stands for "Root Mean Squared Log Error")

Random Forest Regressor:

<p align="left">
  <img width="800" height="70" src="https://github.com/RandomY-2/House_Price_Prediction/blob/main/images/RF_baseline.jpg">
</p>

XGB Regressor:

<p align="left">
  <img width="800" height="70" src="https://github.com/RandomY-2/House_Price_Prediction/blob/main/images/XBG_baseline.jpg">
</p>

AdaBoost Regressor:

<p align="left">
  <img width="800" height="70" src="https://github.com/RandomY-2/House_Price_Prediction/blob/main/images/Ada_baseline.jpg">
</p>

After tuning the parameters and created some additional columns, the performance of the model on the validation set is:

<p align="left">
  <img width="800" height="70" src="https://github.com/RandomY-2/House_Price_Prediction/blob/main/images/final_performance.jpg">
</p>

and on the test set the error is 0.12717. 
