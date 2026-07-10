# CarValue Pro

CarValue Pro is a machine learning project for predicting used car selling prices from a few key vehicle details. It includes a Jupyter notebook for data preprocessing and EDA, a trained XGBoost model, and a Streamlit web app for interactive price prediction.

## Short Summary

The project uses historical car data to estimate resale value based on price, mileage, fuel type, seller type, transmission, ownership count, and car age. The trained model is saved as `xgb_model.json` and is used by the Streamlit app in `car_price_prediction.py`.

## Features

- Predicts car selling price in lakhs.
- Simple Streamlit interface for quick user input.
- Uses a trained XGBoost regression model.
- Supports common car attributes such as fuel type, seller type, transmission, ownership, and age.
- Includes an exploratory data analysis and preprocessing notebook.

## Specifications

- Language: Python
- UI Framework: Streamlit
- ML Library: XGBoost
- Data Handling: Pandas, NumPy
- Visualization and analysis support: Seaborn, scikit-learn
- Model file: `xgb_model.json`
- Main app file: `car_price_prediction.py`
- Notebook file: `Car_Price_Prediction.ipynb`
- Dataset file: `car_data.csv`(not included in the repository)

## Project Workflow

1. Load and clean the car dataset.
2. Perform exploratory data analysis in the notebook.
3. Train a regression model on the processed data.
4. Save the trained model to `xgb_model.json`.
5. Run the Streamlit app to predict prices from user inputs.

## Installation

1. Create and activate a virtual environment.
2. Install the required packages:

```bash
pip install -r requirements.txt
```

## Run the App

Start the Streamlit application with:

```bash
streamlit run car_price_prediction.py
```

## How to Use

1. Enter the car's ex-showroom price.
2. Enter the kilometers driven.
3. Select fuel type, seller type, and transmission.
4. Choose the number of owners.
5. Enter the purchase year.
6. Click Predict to see the estimated selling price.

## Repository Structure

- `car_data.csv` - source dataset, not included in the repository
- `Car_Price_Prediction.ipynb` - preprocessing, EDA, and model development notebook
- `car_price_prediction.py` - Streamlit prediction app
- `xgb_model.json` - saved trained model
- `requirements.txt` - Python dependencies

## Notes

- The app expects `xgb_model.json` to be present in the project root.
- The notebook has not been executed in this workspace, so rerun it if you want to reproduce training from scratch.