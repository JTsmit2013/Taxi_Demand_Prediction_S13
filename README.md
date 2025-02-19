# Taxi_Demand_Prediction_S13

# Sweet Lift Taxi Demand Prediction

## Project Description
Sweet Lift Taxi company has collected historical data on taxi orders at airports. To attract more drivers during peak hours, we need to predict the number of taxi orders for the next hour. This project focuses on building a machine learning model for such a prediction.

## Objective
Develop a predictive model to estimate the number of taxi orders in the next hour while ensuring that the RMSE (Root Mean Squared Error) on the test set does not exceed 48.

## Project Instructions
1. **Download and Preprocess Data**
   - Load the dataset from `/datasets/taxi.csv`.
   - Resample the data by one-hour intervals.
2. **Data Analysis**
   - Explore and visualize trends in the data.
   - Handle missing values and outliers if necessary.
3. **Model Training**
   - Train multiple models with different hyperparameters.
   - Use 10% of the initial dataset as the test sample.
4. **Model Evaluation**
   - Evaluate model performance on the test set.
   - Ensure that RMSE does not exceed 48.
5. **Conclusion**
   - Summarize the findings and recommendations.

## Data Description
- **File Location:** `/datasets/taxi.csv`
- **Target Variable:** `num_orders` (Number of taxi orders per hour)

## Results
- **RMSE:** Moving Average - 84.7333659242237
- **RMSE:** ARMA - 64.27024912019279
- **RMSE:** ARIMA - 62.76809456268275
- **RMSE:** SARIMA - 44.4600827121111
- **RMSE:** Tuned SARIMA - 44.155689802056536
- **RMSE:** Exponential Smoothing - 40.39903153177998

Over the 6 different model testing, half of them achieved an RMSE value of 48 or better.
The best model was **Exponential Smoothing**, followed by the **SARIMA models**.

## Technologies Used
- Python
- Pandas
- Scikit-learn
- Matplotlib/Seaborn (for visualization)
