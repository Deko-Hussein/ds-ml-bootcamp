Part A — Theory
1. Introduction to Regression
What is Regression in Machine Learning?

Regression is a type of supervised machine learning used to predict continuous numerical values. It learns the relationship between one or more input variables (features) and a target variable. After learning from training data, the model can predict numerical values for new data. Regression is commonly used for predicting prices, salaries, temperatures, sales, and many other measurable quantities.

How is it Different from Classification?

Regression and classification are both supervised learning techniques, but they solve different types of problems. Regression predicts continuous numerical values, while classification predicts categories or class labels. For example, predicting the price of a car is a regression problem because the output is a number. Predicting whether an email is spam or not spam is a classification problem because the output belongs to one of two categories.

Examples
Regression Example

Predicting the selling price of a used car based on mileage, model year, engine size, and fuel type.

Classification Example

Predicting whether an email is Spam or Not Spam.

2. Types of Regression
Linear Regression
Basic Idea

Linear Regression predicts a continuous value by finding the best-fitting straight line between one independent variable and one dependent variable. It assumes that the relationship between the variables is linear.

Real-World Use Case

Predicting the selling price of a used car using only its mileage.

Advantages
Simple and easy to understand.
Fast to train and predict.
Works well with linear relationships.
Limitations
Cannot model complex relationships.
Sensitive to outliers.
Performs poorly when the data is non-linear.
Multiple Linear Regression
Basic Idea

Multiple Linear Regression extends Linear Regression by using two or more independent variables to predict one dependent variable. It considers the combined effect of several features on the target.

Real-World Use Case

Predicting house prices using house size, number of bedrooms, age, and location.

Advantages
Uses multiple features for better prediction.
More realistic for real-world problems.
Shows how each feature influences the target.
Limitations
More complex than simple Linear Regression.
Sensitive to multicollinearity.
Still assumes a linear relationship.
Polynomial Regression
Basic Idea

Polynomial Regression is used when the relationship between variables is not linear. It transforms the input features into polynomial terms, allowing the model to fit a curved relationship.

Real-World Use Case

Predicting crop production based on fertilizer usage when the relationship is curved.

Advantages
Models non-linear relationships.
More flexible than Linear Regression.
Can improve prediction accuracy for curved data.
Limitations
Can easily overfit the training data.
Harder to interpret.
Requires selecting the correct polynomial degree.
Comparison of Regression Types
Feature	Linear Regression	Multiple Linear Regression	Polynomial Regression
Number of Input Variables	One	Two or more	One or more
Relationship	Linear	Linear	Non-linear
Model Shape	Straight line	Linear equation	Curved line
Example	Car price by mileage	House price by multiple features	Crop yield prediction
Main Advantage	Simple and fast	Uses more information	Models complex patterns
Main Limitation	Cannot model curves	Assumes linearity	May overfit
3. Regression Metrics

Regression metrics are used to evaluate how well a regression model predicts continuous values.

Mean Absolute Error (MAE)

Mean Absolute Error (MAE) measures the average absolute difference between predicted values and actual values. It treats every error equally and is easy to understand. Lower MAE indicates better performance.

Mean Squared Error (MSE)

Mean Squared Error (MSE) measures the average squared difference between predicted and actual values. Because errors are squared, larger errors receive greater penalties than smaller ones.

Root Mean Squared Error (RMSE)

Root Mean Squared Error (RMSE) is the square root of MSE. It measures prediction error in the same unit as the target variable, making it easier to interpret.

R² (Coefficient of Determination)

R² measures how much of the variation in the target variable is explained by the regression model. A value closer to 1 indicates better performance, while a value closer to 0 indicates poor performance.

Comparison of Regression Metrics
Metric	Unit	Sensitive to Large Errors	Meaning
MAE	Same as target	No	Average absolute error
MSE	Squared target unit	Yes	Average squared error
RMSE	Same as target	Yes	Average prediction error
R²	No unit	No	Explains model accuracy
4. Underfitting and Overfitting
Underfitting

Underfitting occurs when a regression model is too simple to learn the relationship between the input features and the target variable. As a result, it performs poorly on both the training and testing data.

Overfitting

Overfitting occurs when a model learns not only the true patterns in the training data but also the noise. The model performs very well on the training data but poorly on unseen data.

Causes of Overfitting

Overfitting commonly occurs in Polynomial Regression when the polynomial degree is too high. A complex model fits almost every training point, including random noise, instead of learning the true pattern.

Methods to Prevent Overfitting
Use a lower polynomial degree.
Increase the amount of training data.
Apply regularization techniques such as Ridge or Lasso Regression.
5. Real-World Case Study
House Price Prediction Using Multiple Linear Regression

One common real-world application of regression is predicting house prices in the real estate industry. The objective is to estimate the selling price of a house based on its characteristics.

The dataset contains information such as house size, number of bedrooms, number of bathrooms, age of the house, and location. These features are used to predict the selling price.

Multiple Linear Regression is used because house prices depend on several variables rather than a single feature.

The model helps buyers, sellers, and real estate companies estimate fair market prices. Accurate predictions support better investment decisions and improve pricing strategies.

References
Springboard. Regression vs. Classification. https://www.springboard.com/blog/data-science/regression-vs-classification/
GeeksforGeeks. Regression in Machine Learning. https://www.geeksforgeeks.org/machine-learning/regression-in-machine-learning/
Scikit-learn Developers. Model Evaluation: Regression Metrics. https://scikit-learn.org/stable/modules/model_evaluation.html#regression-metrics
James, G., Witten, D., Hastie, T., & Tibshirani, R. (2021). An Introduction to Statistical Learning (2nd ed.). Springe