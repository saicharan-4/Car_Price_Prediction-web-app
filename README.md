# [car_price_prediction_webapp](https://github.com/parthshah28/car_price_prediction_webapp)

![](https://github.com/parthshah28/car_price_prediction_webapp/blob/main/images/download.jpg)

## Web App on Heroku - [Click Here](https://car-price-prediction-webapp.herokuapp.com/)

![](https://github.com/parthshah28/car_price_prediction_webapp/blob/main/images/captured.gif)

## Dataset:

Dataset is taken from [Kaggle](https://www.kaggle.com/nehalbirla/vehicle-dataset-from-cardekho)

Dataset has (301, 9) rows and columns.

#### Data set has 9 columns: 'Car_Name', 'Year', 'Selling_Price', 'Present_Price', 'Kms_Driven', 'Fuel_Type', 'Seller_Type', 'Transmission', 'Owner'

![](https://github.com/parthshah28/car_price_prediction_webapp/blob/main/images/1.png)

## Feature Engineering:
to understand it in more detail go to [car.ipynb](https://github.com/parthshah28/car_price_prediction_webapp/blob/main/Untitled.ipynb)

First I have created **dummy variables** for categorical features which are **'Fuel_Type', 'Seller_Type', 'Transmission'**.

After that I have used **ExtraTreeRegressor** to understand feature importance.

![](https://github.com/parthshah28/car_price_prediction_webapp/blob/main/images/2.png)

## Algorithms Used:

I have used **RandomForestRegressor Algorithm and RandomizedSearchCV** for selecting best parameters.

#### Best Parameters - {'n_estimators': 1000, 'min_samples_split': 2, 'min_samples_leaf': 1, 'max_features': 'sqrt', 'max_depth': 25}
#### Best Score - -3.9462177171800144

## Result:

Distribution plot of predictions-

![](https://github.com/parthshah28/car_price_prediction_webapp/blob/main/images/3.png)

MAE: 0.8940449450549446

MSE: 3.9896801576648344

RMSE: 1.997418373216997
