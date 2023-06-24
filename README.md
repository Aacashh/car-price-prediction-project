# Car Price Prediction Project

This project involves in-depth data analysis of a car price dataset and training a machine learning model to predict car prices. The dataset contains various features of cars, including engine size, horsepower, curb weight, fuel type, aspiration, and body style, among others.

## Methods Used

The analysis involved several steps:

1. **Data Overview**: We started by getting an overview of the dataset, including the number of rows and columns and the names of the columns.

2. **Descriptive Statistics**: We generated descriptive statistics for the numerical columns in the dataset. This includes count, mean, standard deviation, minimum value, 25th percentile, median, 75th percentile, and maximum value.

3. **Data Visualization**: We created plots using Plotly to visualize the relationships between variables and the car price. This included scatter plots for numerical variables and box plots for categorical variables.

4. **Bivariate and Trivariate Analysis**: We conducted bivariate and trivariate analyses to explore the relationships between car price and two or three other variables. This involved creating a scatter plot and a 3D scatter plot, respectively.

5. **Regression Analysis**: We used a linear regression model to predict car prices based on engine size and horsepower. We visualized the results with a 3D scatter plot showing the actual and predicted prices.

6. **Feature Engineering**: We applied ordinal encoding to categorical variables and binning to numerical variables to prepare the data for machine learning.

7. **Model Training**: We trained an XGBoost model on the processed data and evaluated its performance using mean squared error and R-squared score.

8. **Feature Importance Analysis**: We calculated and plotted the feature importances from the XGBoost model to understand which features were most influential in predicting car prices.

## Key Findings

The analysis found that the 'enginesize' feature has the highest importance in predicting the car price, followed by 'highwaympg' and 'carwidth'. This makes sense as larger engines are generally more expensive, and cars with higher miles per gallon (mpg) are more fuel efficient, which can also contribute to a higher price. The car's width can also indicate its size and capacity, which can affect the price. The other features have less importance in the prediction.

The XGBoost model trained on the processed data achieved a mean squared error of approximately 5,624,787 and an R-squared score of approximately 0.929 on the test set. This indicates that the model explains about 92.9% of the variance in car prices, which is a significant improvement over the previous models.

These insights can be very useful for predicting car prices. However, it's important to remember that these are general trends, and there can be exceptions. Other factors not included in this dataset, such as brand reputation, car age, and mileage, can also significantly influence car prices.
