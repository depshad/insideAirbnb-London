# Inside Airbnb-London
Exploratory Data Analysis and Predictive Modeling for Airbnb London listings

Data can be downloaded from http://data.insideairbnb.com/united-kingdom/england/london/2019-07-10/data/listings.csv.gz

## Exploratory Data Analysis

***Feature Selection***

1.Remove features with more than 90% values missing

2.Remove features with constant value for all data points

3.Remove empty features

***Feature Engineering***

1.Convert boolean features to numerical

2.Convert currency based features to numerical from string type

3.Extract features out of free form text(House Rules)

4.Create feature:host_duration using last_scraped and host_since information 

5.Convert various categorical features to numerical

6.Create 'distance to center' feature: distance between London's center to listings 

7.Create 'amenities_count' from amenities 

8.Feature imputation using the mean,median values

## Vizualization

1.Plot log tranformed price feature

2.Effect of bedrooms and accommodates on price

3.Vizualize various numerical features using boxplot 

## Modeling

The dependent variable is listing price

1.Random Forest regreesor with n_estimators tuned using GridSearch 

2.Feature importance plot

***Future Work***

1.Instead of euclidean distance use a specilaized distance (vincenty, Haversine)

2.Use zipcode,neighbourhood feature to cluster listings

3.Try different imputation strategies and observe the effect on model's prediction error

4.Tune other hyperparameters of RandomForest model

5.Use different regression models and compare the performance

6.Calculate prediction intervals 

7.Create an ensemble of regression models


