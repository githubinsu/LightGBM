# Customer Purchase Prediction through LightGBM

This code predicts which category of product a customer will purchase on their next visit based on their purchase data.

## Process

1. Pivot the data to check the purchase frequency by customer and remove outliers.
2. Encode the category columns using a label encoder and convert datetime data to numeric.
3. Convert each customer's purchase history into time series data and pad to the same length.
4. Replace NaN values and split the data into training and test sets.
5. Train and evaluate a LightGBM model.
6. Save the products purchased on the last purchase date and calculate the accuracy.
7. Create an empty data frame and perform model predictions for each customer, inputting the results into the data frame.
8. Create a summary data frame and check the purchase frequency by sector for each customer, creating sector columns in the data frame.

For customers who have made n purchases, the model is trained on the first n-1 purchase categories to predict which product the customer purchased on their nth (last) purchase.

## Machine Learning

This code uses machine learning to make predictions. Machine learning is a method of teaching computers to learn from data, without being explicitly programmed. The LightGBM model used in this code is a gradient boosting framework that uses tree-based learning algorithms.

To improve accuracy, hyperparameters are adjusted using Bayes search and a confusion matrix is calculated to check for errors.

## Results

The model achieved an accuracy score of 85%, indicating that it is a meaningful analysis. Although only 100,000 recent data points were used for this upload, using data from a longer period could further increase the accuracy score.

The results can be used for targeting CRM and personalized platforms based on the predicted purchase category of the customer.
