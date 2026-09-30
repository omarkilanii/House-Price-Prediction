# House Price Prediction

A beginner machine learning project for predicting house prices using the California Housing Prices dataset.

## Project Overview

The goal of this project is to build a machine learning model that predicts the median house value based on information such as location, number of rooms, population, households, and median income.

This project focuses on understanding the basic machine learning workflow:

* Data Exploration
* Exploratory Data Analysis (EDA)
* Data Preprocessing
* Train/Test Split
* Model Training
* Cross-Validation
* Model Comparison
* Hyperparameter Tuning
* Model Evaluation
* Making Predictions

## Dataset

The project uses the California Housing Prices dataset.

Dataset source:

Kaggle - California Housing Prices

The dataset contains information about housing districts in California.

### Target Variable

`median_house_value`

### Main Features

* `longitude`
* `latitude`
* `housing_median_age`
* `total_rooms`
* `total_bedrooms`
* `population`
* `households`
* `median_income`
* `ocean_proximity`

## Machine Learning Models

The following models were tested:

* Linear Regression
* Ridge Regression
* Lasso Regression
* Random Forest Regressor
* HistGradientBoosting Regressor

The models were compared using Cross-Validation.

## Preprocessing

The dataset contains both numerical and categorical features.

### Numerical Features

* Missing values were handled using median imputation.
* Features were scaled using StandardScaler.

### Categorical Features

* Missing values were handled using the most frequent value.
* `ocean_proximity` was converted using OneHotEncoder.

## Evaluation Metrics

The models were evaluated using:

* RMSE (Root Mean Squared Error)
* MAE (Mean Absolute Error)
* R² Score

RMSE was mainly used to compare the models.

## Project Workflow

```text
Dataset
   ↓
Data Exploration
   ↓
EDA
   ↓
Data Cleaning
   ↓
Train / Test Split
   ↓
Preprocessing
   ↓
Baseline Model
   ↓
Model Comparison
   ↓
Cross-Validation
   ↓
Hyperparameter Tuning
   ↓
Final Evaluation
   ↓
Prediction
```

## Project Structure

```text
house-price-prediction/
│
├── data/
│   ├── README.md
│   └── housing.csv
│
├── images/
│   ├── target_distribution.png
│   ├── correlation_heatmap.png
│   └── residual_analysis.png
│
├── house_price_prediction.ipynb
├── requirements.txt
├── .gitignore
├── README.md
└── LICENSE
```

## Installation

Clone the repository:

```bash
git clone <your-repository-url>
cd house-price-prediction
```

Install the required libraries:

```bash
pip install -r requirements.txt
```

## Dataset Setup

Download the `housing.csv` dataset and place it inside:

```text
data/housing.csv
```

The dataset is not included in the repository.

## Run the Project

Open the Jupyter Notebook:

```bash
jupyter notebook
```

Then open:

```text
house_price_prediction.ipynb
```

Run the notebook cells from top to bottom.

## What I Learned

Through this project, I practiced:

* Exploratory Data Analysis
* Data preprocessing
* Handling missing values
* Encoding categorical features
* Feature scaling
* Regression
* Cross-Validation
* Model comparison
* Hyperparameter tuning
* Model evaluation
* Residual analysis
* Making predictions with a trained model

## Future Improvements

Some possible improvements are:

* Feature engineering
* Log transformation of the target
* More hyperparameter tuning
* Trying XGBoost or LightGBM
* More detailed error analysis
* Deploying the model as an API

## Author

**Omar Fathi**

Machine Learning / AI Engineer
