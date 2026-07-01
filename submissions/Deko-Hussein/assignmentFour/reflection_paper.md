# Reflection Paper

## Assignment Four: Car Price Prediction Using Regression Models

### 1. What Did You Implement?

In this assignment, I implemented two machine learning regression models to predict car prices using the cleaned dataset from Assignment Three. I first loaded the cleaned dataset and selected **Price** as the target variable while using all other columns except **Price** and **LogPrice** as the input features.

Next, I divided the dataset into training and testing sets using an 80% training and 20% testing split with a random state of 42. After preparing the data, I trained two regression models: **Linear Regression** and **Random Forest Regressor**. Finally, I evaluated both models using four regression metrics: R², MAE, MSE, and RMSE. I also performed a sanity check by comparing the predicted price of one test sample with its actual price.

---

## 2. Comparison of Models

During the sanity check, the actual price of the selected car was **7000**. The Linear Regression model predicted approximately **5712**, while the Random Forest model predicted approximately **6821**.

For this particular example, the Random Forest prediction was closer to the actual price than the Linear Regression prediction. However, a single prediction is not enough to determine the best model. The overall evaluation metrics provide a more reliable comparison because they measure the performance across the entire testing dataset.

---

## 3. Understanding Random Forest

Random Forest is an ensemble machine learning algorithm that combines many decision trees into one model. Instead of relying on a single decision tree, the algorithm builds multiple trees using different samples of the training data. Each tree makes its own prediction, and the final prediction is calculated by averaging the predictions of all the trees.

This approach usually produces more stable and accurate predictions than a single decision tree because it reduces the effect of random errors and helps improve generalization.

---

## 4. Metrics Discussion

The evaluation results showed that **Linear Regression** achieved a higher **R² score (0.436)** compared to **Random Forest (0.288)**. This means that the Linear Regression model explained more of the variation in car prices within the dataset.

When comparing the error metrics, Random Forest produced a slightly lower **MAE**, which means its average prediction error was smaller. However, Linear Regression achieved a lower **RMSE**, indicating that it handled larger prediction errors more effectively.

These results suggest that Linear Regression provided better overall performance for this dataset, while Random Forest produced better predictions for some individual cases.

---

## 5. My Findings

Based on the overall evaluation, I prefer the **Linear Regression** model for predicting car prices in this dataset. Although the Random Forest model generated a prediction closer to the actual price during the sanity check, Linear Regression achieved a higher R² score and a lower RMSE, indicating stronger overall performance across the testing dataset.

This assignment helped me understand that choosing the best machine learning model should not be based on a single prediction. Instead, evaluation metrics such as R², MAE, MSE, and RMSE provide a more accurate way to compare models. I also learned that different regression algorithms have different strengths, and the most suitable model depends on the characteristics of the dataset.