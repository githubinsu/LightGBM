# Customer Purchase Prediction through LightGBM
## Light Gradient Boosting Machine(Tree-based Model)
Tree-based models are a type of machine learning algorithm that use a series of if-then rules to generate predictions from one or more decision trees. One popular tree-based model is LightGBM, which stands for Light Gradient Boosting Machine. LightGBM is a gradient boosting framework that uses tree-based learning algorithms and is designed to be faster and more efficient than other gradient boosting frameworks.

## Objective
The goal of this project is to use the LightGBM algorithm to predict which category of product a customer will purchase on their next visit based on their purchase data. By using the predicted results, we can display the category with the highest purchase probability on the main banner when the customer visits our store again. We can also adjust the UI to be more suitable for the recommended category, thereby increasing customer convenience and purchase conversion.

## Process
The code follows several steps to achieve this goal:

Data Preprocessing: Pivot the data to check the purchase frequency by customer and remove outliers. Encode the category columns using a label encoder and convert datetime data to numeric. Convert each customer’s purchase history into time series data and pad to the same length.

Model Training: Split the data into training and test sets. Train a LightGBM model on the training data.

Model Evaluation: Evaluate the model on the test data. 

## Results
The performance of the LightGBM model can be evaluated using metrics such as accuracy. In this case, the model achieved an accuracy score of 85%, indicating that it can predict the expected product of a customer’s purchase with high probability. 
