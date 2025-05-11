#  Walmart Sales Forecasting

This project focuses on building a predictive model for Walmart's sales data using machine learning techniques. It explores the relationships between various features like store type, holidays, markdowns, and economic indicators to forecast weekly sales.

## Project Overview

The notebook `Final_Model.ipynb` includes:
- Data loading from multiple CSV files
- Data merging, cleaning, and feature engineering
- Model training using Random Forest and XGBoost
- Evaluation using regression metrics

## Dataset Description

The following CSV files are used:
- `features.csv`: Economic and promotional data (fuel price, CPI, etc.)
- `stores.csv`: Metadata about each store (type, size)
- `train.csv`: Historical sales data (used for training)
- `test.csv`: Test set for prediction
- `sampleSubmission.csv`: Submission format for predictions

## Preprocessing Steps

- Merged multiple datasets into a single DataFrame
- Parsed and transformed date features
- Encoded categorical variables
- Filled or dropped missing values

##  Models Used

- **Random Forest Regressor**: Ensemble-based decision tree model
- **XGBoost Regressor**: Optimized gradient boosting framework
- **LGBM Regressor**: Light gradient boosting framework

## Evaluation Metrics

- **Mean Absolute Error (MAE)**: Measures average absolute error
- **Root Mean Squared Error (RMSE)**: Penalizes large errors
- **R² Score**: Indicates the proportion of variance explained by the model

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/walmart-sales-forecast.git
   cd walmart-sales-forecast
   ```

2. Make sure all dataset CSV files are in the same directory.

3. Launch Jupyter Notebook:
   ```bash
   jupyter notebook Final_Model.ipynb
   ```

4. Run each cell sequentially to train the model and evaluate performance.

## Future Enhancements

- Add time series-specific models (e.g., LSTM, ARIMA)
- Deploy the model via Flask/Streamlit for public interaction
- Integrate feature selection and cross-validation pipelines
