The programming language used in this project is Python . The following libraries were used for data analysis and data visualization and to build a classifier to predict the price range of mobile phones.

Pandas : For loading the dataset and performing data wrangling

Matplotlib: For data visualization.

Seaborn: For data visualization.

NumPy: For some math operations in predictions.

Statsmodels: For statistical computations

Sklearn: For the purpose of analysis,prediction and evaluation.
📑 Steps involved

Data Preprocessing : Checked for outliers, incorrect values, missing values, duplicates and performed data type correction.

Feature Extraction : Created new columns such as Day, Month, Year, Days_of_week and Weekend from Date column .

Exploratory Data Analysis : Performed Univariate, Bivariate, and Multivariate analysis with various graphs and plots to better understand the distribution of features and their relationships.

Feature Selection : Checked the VIF value (measure of multicollinearity) and dropped Dew point Temperature and Year which were highly correlated with other independent features.

Feature encoding : The categorical features present in the dataset Seasons, Holiday, Weekend, Functioning Day were dummified.

Feature Scaling : Brought features to a similar range using MinmaxScaler.

Implementation of Regression models

Hyperparameter tuning

Comparison of models
💻 Algorithms used

Linear Regression

Polynomial Regression

Decision Tree

Random Forest

XGBoost

Gradient Boosting

Stacking

Conclusion

Findings from EDA:

Temperature and Hour have a strong correlation with the count of rented bikes.

Dew point temperature is highly positively correlated to the Temperature.

Over the weekend and during holidays, rental bike demand decreases.

There is a significant drop in the number of rented bikes during Winters(Dec-Feb) because it's freezing cold!

The demand for bikes increases during warmer temperatures,which is why there's maximum count of rented bikes during the Summer season.

In all seasons,the peak demands for rental bikes occur on the opening (8-9 AM) and closing times (6-7pm) of offices and institutions.

Conclusion Based on Model Evaluation:

Stacking was found to be most suitable for making predictions of hourly demand for rental bikes.

An adjusted R2 score of 0.91 was obtained.

Temperature and Hour were found to be most influential variables in predicting the hourly demand for rental bikes.

When compared to other models used, decision tree-based models have performed well.

Linear and Polynomial regression models did not perform well in this case, since there is no significant linear correlation between Rented bike count and the independent features.
