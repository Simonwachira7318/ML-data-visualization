# Maintenance Dataset Analysis

This project analyzes the `Maintenance.csv` dataset, performing various data exploration and machine learning tasks.

## Files

- `Maintenance.csv`: The dataset used for analysis.
- `README.md`: This file, containing project information.
- `maintenance_analysis.py` (or similar): The Python script performing the analysis.

## Libraries Used

- `pandas`: For data manipulation and reading the CSV file.
- `matplotlib.pyplot`: For creating visualizations.
- `seaborn`: For enhanced data visualizations, especially correlation heatmaps.
- `sklearn.model_selection`: For splitting data into training and testing sets.
- `sklearn.linear_model`: For building and training the Linear Regression model.
- `sklearn.neighbors`: For building and training the K-Nearest Neighbors (KNN) Regressor model.
- `sklearn.metrics`: For evaluating model performance (MSE, RMSE, R-squared).
- `numpy`: For numerical operations (e.g., calculating RMSE).

## Analysis Steps

1.  **Import Libraries:**
    - Imports necessary libraries for data manipulation, visualization, and machine learning.

2.  **Load Dataset:**
    - Reads the `Maintenance.csv` file into a pandas DataFrame.

3.  **Visualize Data:**
    - Generates histograms for selected columns to understand their distributions.

4.  **Visualize Correlation Between Features:**
    - Creates a heatmap to visualize the correlation matrix of the features, helping identify relationships between variables.

5.  **Prepare Data for Linear Regression:**
    - Selects relevant features (numerical columns, excluding target and label columns).
    - Splits the data into training and testing sets.

6.  **Linear Regression Prediction:**
    - Trains a Linear Regression model on the training data.
    - Makes predictions on the test data.

7.  **Plot Linear Regression Features:**
    - Visualizes the actual vs. predicted values from the Linear Regression model using a scatter plot.
    - Calculates and prints the Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and R-squared (R2) to evaluate model performance.

8.  **Visualizing a Nearest Neighbor Algorithm (KNN):**
    - Trains a KNN Regressor model on the training data.
    - Makes predictions on the test data.
    - Visualizes the actual vs. predicted values from the KNN model using a scatter plot.
    - Calculates and prints the MSE, RMSE, and R2 to evaluate KNN model performance.

## Usage

1.  Place the `Maintenance.csv` file in the same directory as the Python script.
2.  Run the Python script (`python maintenance_analysis.py`).
3.  The script will generate visualizations and print model evaluation metrics to the console.

## Notes

-   The script assumes the target variable is named 'ttf' and label columns are 'label_bnc' and 'label_mcc'.
-   Feature selection in the script is a basic example (selecting numerical columns). More advanced techniques might be needed for optimal performance.
-   The number of neighbors (k) in the KNN model is set to 5. You can adjust this parameter.
-   The random state in the train-test split is set to 42 for reproducibility. You can change it if needed.
