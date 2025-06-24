# Appliance Energy Consumption Prediction

This project focuses on developing a machine learning model to solve a regression problem: predicting the energy consumption of home appliances (in Wh). The model uses environmental sensor data, such as temperature and humidity, collected from inside and outside a residence.

## File Description

- `main-analysis`: The main project notebook, containing the Python code for exploratory data analysis and prediction modeling.
- `KAG_energydata_complete.csv`: The dataset used in the project, containing sensor data and the energy consumption of appliances.

## Requirements

* **Language:** Python 3
* **Core Libraries:**
    * Pandas & NumPy for data manipulation.
    * Scikit-learn & XGBoost for modeling and evaluation.
* **Visualization:**
    * Matplotlib & Seaborn
* **Environment:** Jupyter Notebook

## Data Source

The project uses the "Appliances Energy Prediction" dataset from Kaggle. It contains sensor measurements of temperature and humidity from a home, collected every 10 minutes.

* Kaggle Link: [Appliances Energy Prediction](https://www.kaggle.com/datasets/loveall/appliances-energy-prediction)

## Setup and Usage

To run this project locally, follow these steps:

1.  Clone the repository:
    ```bash
    git clone https://github.com/andredeoliveiraa/ml-energy-prediction.git
    ```
2.  Open the `main-analysis` notebook and run the cells.

## Results

The Optimized Random Forest model demonstrated the best performance across all evaluation metrics. The final model can explain approximately 59.5% of the variance in energy consumption and has a Mean Absolute Error (MAE) of just 30.23 Wh.

| Model                       | MAE (Wh) | RMSE (Wh) | R²     |
| --------------------------- | -------- | --------- | ------ |
| **Random Forest (Optimized)** | **30.23**| **63.70** | **0.5945** |
| Random Forest (Default)     | 32.44    | 68.43     | 0.5320 |
| XGBoost (Default)           | 35.48    | 69.72     | 0.5143 |
| KNN (Default)               | 45.47    | 88.43     | 0.2185 |





