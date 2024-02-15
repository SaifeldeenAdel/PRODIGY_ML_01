# Prodigy InfoTech Machine Learning Internship Task 1

## **Task Details**

Implement a linear regression model to predict the prices of houses based on their square footage and the number of bedrooms and bathrooms.

## **Implementation**

There was two major steps to this process:

1. Cleaning and extracting the relevant data from the [dataset](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data).
2. Creating and fitting the linear regression model over our data and using it to perform predictions on new data.

### **Data Analysis and Cleaning**

-   Selected the relevant features needed in this task. Chose to mostly work with numerical features as the task specified numerical features and I'm not yet used to Encoding categorical features.
-   Checked for null values and dealt with them appropriately (either dropping the feature or filling in appropriate values)
-   Calculated every feature's correlation with our target `SalePrice` and removed any feature that has too low of a correlation
-   Created two new features `TotalRooms` and `SquareFootage` which correlate quite well with `SalePrice` and so are useful for our model

### **Linear Regression Model**

-   Split my clean data into training and testing sets
-   Fit a LinearRegression model from `sklearn` use my training sets
-   Used my testing set to predict values and compared them with their actual values on a plot.
-   Calculated my predictions' error percentage and my model's r2_score. Seemed to be doing quite well.

There are plenty of optimizations to be done on this dataset and so hopefully I get the time to produce even better results the more I learn.
