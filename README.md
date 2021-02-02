# Airbnb Price Prediction 


**Overview**

Airbnb is one of the largest online marketplaces for arranging or offering apartments, homestays and lodging. The number of bookings and listings are growing fast, there are over 6 million listings worldwide in 2019(I choose 2019 instead of 2020 because of the covid 19 pandemics). New York is listed as one of the top 10 popular cities for booking experiences in the world. The total price of a reservation on Airbnb is based on the nightly rate (based price per night), which is sole set by the host, plus other fees such as service fees, cleaning fee, etc. 

**Business Benefits**

There are currently no free and accurate services which help hosts price their properties using a wide range of data points. This project aims to help hosts determine a proper nightly rate based on the pricing model built from a range of relative factors in the New York Area.

**Datasets**

The data used in this project is generated from “Inside Airbnb”, which uses data sourced from publicly available information from the Airbnb site. http://insideairbnb.com/get-the-data.html. The original raw datasets used in this project all stored in the data folder.

Size: ~96MB

Metrics: 106 metrics

Date: 2019 June, July, Auguest, September


**Project purpose**

It is important for hosts to understand Airbnb pricing and value the place correctly. This project aims to help hosts to determine a proper nightly rate based on the pricing model built from a range of relative factors in the New York Area.

**Python Libraries**

###### Data cleanning: pandas, numpy
###### Data Exploratory analysis: matplotlib, seaborn, numpy, geopandas, nltk.sentiment.vader, SentimentIntensityAnalyzer, SelectKBest, WordCloud
###### Data Model: sklearn.model_selection(train_test_split),sklearn.feature_selection, pandas, sklearn.ensemble(RandomForestRegressor),sklearn.metrics(R^2), matplotlib.pyplot, seaborn, numpy


**Part1: Data preprocessing and Feature selection**

Initial clean, detect and remove outliers with Z score, feature selection.

![Feature Importances](https://github.com/Charlotte-01/TDI-capstone-project/blob/main/Feature%20Importances.png)

reviews_per_month is one of important feature in the data analysis, but it is not that important for the renter to predict the price.


**Part2: Visualization**

The Visualization contains visual plots. 
1. Average price Per Borough
![Average price Per Borough](https://github.com/Charlotte-01/TDI-capstone-project/blob/main/Average%20price%20Per%20Borough.png)

As we can see from the plots, Mahanttan is the most expensive area

2. Total listings Per Borough
![Total listings Per Borough](https://github.com/Charlotte-01/TDI-capstone-project/blob/main/Total%20listings%20Per%20Borough_read.png)

As we can see from the plots, Queens has highest numbers of listings.

3. House Rules.png
![House Rules](https://github.com/Charlotte-01/TDI-capstone-project/blob/main/House%20Rules.png)

Wordcloud plots give some key words regarding description, house rules that host can pay attention to while renting the place.

4. Room Types Per Borough
![Room Types Per Borough](https://github.com/Charlotte-01/TDI-capstone-project/blob/main/Room%20Types%20Per%20Borough.png)

Entire home/apt constitudes about 75-80% of listings type.

**Part3: Natural Language Processing**
Coming soon...

**Part4: Model**
After running different algorithms including Linear Regression, K Means, Decision Tree, Multiple Regression, I finalize choosing Random Forest Model. Below are two output plots to visulize the result of my model:

### 1.Predicted Results vs Actual Results - bar plot
![](https://github.com/Charlotte-01/TDI-capstone-project/blob/main/Predicted%20Results%20vs%20Actual%20Results2.png)

### 2.Predicted Results vs Actual Results - line plot

![](https://github.com/Charlotte-01/TDI-capstone-project/blob/main/Predicted%20Results%20vs%20Actual%20Results1.png)

### The accuracy rate: ~ 85% 

**Part5: Web develop**

Web develop link http://aec4.com/cis9650/airbnb.py 

Hosts can use the link and input their available data. Output will be suggested price housing.


