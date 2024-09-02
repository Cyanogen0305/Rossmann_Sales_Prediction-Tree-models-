# Rossmann Store Sales Prediction

## Project Overview

This project involves predicting daily sales for Rossmann stores using historical sales data. The goal is to forecast future sales based on various features, including store-specific information, promotional events, and seasonal effects. The project uses XGBoost, a powerful gradient boosting framework, to model and predict the sales.

## Project Structure

- `rossmann_sales_prediction.ipynb`: The main Jupyter Notebook that contains all the code for data preprocessing, model training, evaluation, and prediction generation.
- `solution.csv`: The output file containing the predicted sales for the test dataset, formatted for submission.

## Data

The dataset includes sales data for various Rossmann stores, with features such as:

- `Store`: Store ID
- `Sales`: The sales amount for a specific day
- `Customers`: The number of customers for a specific day
- `Open`: Indicator if the store was open or closed
- `Promo`: Indicator if the store was running a promotion on that day
- `StateHoliday`: Public holiday indicator
- `SchoolHoliday`: Indicator if the day was a school holiday
- Additional features related to the store type, assortment, competition, and promotional intervals.

## Workflow

1. **Data Preparation**:
   - Filter and split the data into training and testing sets.
   - Handle missing values using mean imputation.

2. **Model Training**:
   - Train an XGBoost model on the prepared data.
   - Evaluate the model using Root Mean Squared Error (RMSE) on a validation set.

3. **Prediction**:
   - Generate predictions on the test set.
   - Format the predictions and save them to a CSV file for submission.

## How to Run the Project

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/rossmann-sales-prediction.git
   cd rossmann-sales-prediction
   ```

2. **Install Dependencies**:
   - Ensure you have Python 3.x installed.
   - Install the required Python packages using pip:
  ```bash
  pip install -r requirements.txt
  ```

3. **Run the Jupyter Notebook**:
   - Launch Jupyter Notebook; open rossmann_sales_prediction.ipynb and run all the cells.:
  ```bash
  jupyter notebook
  ```
4. **Generate Submission**:
    - After running the notebook, the predictions will be saved as solution.csv.
    - Submit solution.csv to the competition or your evaluation platform.

## Results
The model is evaluated using RMSE, with lower values indicating better performance. The final predictions are saved in solution.csv for submission.

## Acknowledgments
The dataset is provided by the Rossmann Store Sales competition on Kaggle.
XGBoost, a powerful machine learning framework, is used for model training.
