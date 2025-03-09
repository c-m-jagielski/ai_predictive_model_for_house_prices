# ai_predictive_model_for_house_prices
Getting started with AI: a predictive model for house prices

Data came from Kaggle: "House Prices: Advanced Regression Techniques" competition
  - https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data

Start out with:
`python -m venv venv`

Then active it:
`source venv/bin/activate`

Install dependencies:
`pip install -r requirements.txt`

Start the data manipulation:
`jupyter notebook`

--------------

# House Price Prediction Model

This project builds a machine learning model to predict house prices based on various features like square footage, neighborhood, amenities, etc.

## Project Structure
- `01_data_exploration.ipynb`: Initial data analysis and visualization
- `02_data_preprocessing.ipynb`: Data cleaning and feature engineering
- `03_model_training.ipynb`: Model selection, training, and evaluation
- `04_model_application.py`: Production-ready model deployment example
- `data/`: Directory containing raw and processed datasets
- `models/`: Directory storing trained model files

## Key Features
- Extensive data preprocessing including handling missing values
- Feature engineering to improve model performance
- Evaluation of multiple regression algorithms
- Feature importance analysis
- Production-ready prediction function

## Results
- Best performing model: [Your best model]
- RMSE on validation data: [Your score]
- Most important features: [Top features]

## Usage
To make predictions with the trained model:
```
python
from model_application import predict_price

house_features = {
    'GrLivArea': 1500,  # Living area in square feet
    'OverallQual': 7,   # Overall quality rating
    # Add other features
}

predicted_price = predict_price(house_features)
print(f"Predicted house price: ${predicted_price:,.2f}")
```