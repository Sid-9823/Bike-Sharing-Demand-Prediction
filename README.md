# Bike-Sharing-Demand-Prediction
![0_gTer_2Mf4cjVl5v5](https://github.com/Sid-9823/Bike-Sharing-Demand-Prediction/assets/125801958/befae13c-150c-43eb-93ae-7651b4aa0c3e)


<H2>Problem Statement</H2>

Rental bikes have become an increasingly popular mode of transportation in urban areas, as they provide a convenient and eco-friendly alternative to traditional means of getting around. However, one of the key challenges in implementing rental bike schemes is ensuring a stable supply of bikes at all times. In order to address this issue, it is crucial to accurately predict the number of bikes required at different hours of the day.

In this project, I am using various machine learning regression models to analyze various factors that impact bike usage, such as temperature, season, rainfall, holidays, the number of rented bikes at different times of the day, etc. By taking these factors into account, it becomes possible to forecast demand and allocate resources accordingly, ensuring a steady supply of rental bikes and reducing wait times for users.

<H2>Project Summary</H2>

Bikes have grown in popularity as a practical and environmentally friendly alternative to traditional modes of transportation in metropolitan areas. However, one of the most difficult issues in implementing rental bike programs is ensuring a constant supply of bikes. To overcome this issue, it is critical to precisely forecast the number of bikes needed at various times of the day.

In the beginning, we imported the required libraries that were necessary to perform operations, and then we performed basic operations such as mounting the drive, loading the dataset (there are a total of 8760 columns and 14 rows in this dataset), and storing it in a data frame. Performed basic analysis like checking dimensions, finding null values, and a bit of data wrangling in which we performed some feature engineering on the 'Date' column and divided it into several others to get deeper insights.

Further on, we did some EDA on our dataset, performed univariate and bivariate analysis on our dataset separately to derive in-depth insights, and plotted the distribution of each feature. We checked the correlation and treated multicollinearity with the help of heatmap correlation.

We create three hypothetical assertions and do hypothesis testing based on our visualizations. The statements are as follows:

At any given time, the average number of bikes in Seoul is more than 100.

At every location in Seoul, the average temperature is greater than 10 degrees Celsius.

The standard deviation of humidity in Seoul is 20.

In our feature engineering part, we handled outliers by the square root transformation method and treated moderate right skewness of the dataset. With the help of one hot encoding technique, we converted our categorical features into numerical features.

For the model implementation part, we divided our dataset into an 80:20 training: testing split. We then utilized six machine learning algorithms: linear regression, lasso, ridge, decision tree, random forest, and gradient boosting. We used hyper-tuning to increase the performance of our model and put the results in a data frame so we could compare them later. The best r2 scores we got were with gradient boosting and random forest models: overall 92% for gradient boosting and 91% for random forest.

So in the end, the bike rental firm can deploy a model that either uses one of the above-mentioned models to maintain a stable supply of rental bikes or reduce wait times for users.

<H2>Conclusion</H2>

The experiment successfully proved the potential of predicting bike demand in Seoul using machine learning techniques.

The following are some essential points:

* In the morning and evening, there is high demand.
* In the winter, there is less demand.  
* June has the most demand.
* Temperature and dew point temperatures were discovered to be multicollinear.
* We used six machine learning algorithms: linear regression, lasso, ridge, decision tree, random forest, and gradient boosting. Gradient 
  boosting produced the maximum accuracy (94% on the train and 91% on the test).
* There is no evidence of overfitting.
* We can deploy this model.
* Overall, the study illustrates machine learning's potential for tackling real-world issues and provides a path for future research in this 
  field. The findings of this experiment can be applied to other cities with similar bike infrastructure.
