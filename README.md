# NYC Taxi Fare Prediction

## Project Overview
The goal of this project is to predict NYC taxi fares based on trip distance, number of passengers, and pickup time. The notebook demonstrates a complete machine learning workflow including data preparation, feature engineering, model training, evaluation, and visualization.

## Dataset
The dataset contains 600 sample trips with the following columns:
- `pickup_datetime`: Trip start time
- `passenger_count`: Number of passengers
- `pickup_longitude` & `pickup_latitude`: Pickup location
- `dropoff_longitude` & `dropoff_latitude`: Dropoff location
- `fare_amount`: Fare in USD

## Features
- Trip distance (calculated from pickup and dropoff coordinates)
- Passenger count
- Pickup hour
- Pickup day of the week

## Models
- **Linear Regression**  
- **Random Forest Regressor**

## Results
| Model               | RMSE   | R² Score |
|--------------------|--------|----------|
| Linear Regression  | 5.77   | 0.83     |
| Random Forest      | 6.22   | 0.80     |

Linear Regression slightly outperformed Random Forest. Feature importance analysis from Random Forest shows that **trip distance** is the most important predictor.

## Visualizations
- Actual vs Predicted fares for both models  
- Residual (error) distributions  
- Feature importance chart for Random Forest  
