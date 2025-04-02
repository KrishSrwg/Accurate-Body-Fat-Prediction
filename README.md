# Accurate-Body-Fat-Prediction

##Overview
Body Fat Prediction is a machine learning project designed to predict an individual's body fat percentage based on their physical measurements. The project uses regression models to analyze data and provide accurate predictions. A web interface built with Flask allows users to input their measurements and get predictions instantly.

## Features

- **Machine Learning Models**: Multiple regression models implemented and compared.
- **Interactive Web Application**: Flask-based GUI for predictions.
- **Dataset Analysis**: Exploratory data analysis and preprocessing.
- **Model Comparison**: Evaluation of different algorithms to select the best-performing model.


## Dataset

The dataset contains physical measurements like density, age, weight, height, neck circumference, chest circumference, etc., along with the corresponding body fat percentage.

| Feature       | Description                          |
|---------------|--------------------------------------|
| `Density`     | Body density                         |
| `BodyFat`     | Body fat percentage (target)         |
| `Age`         | Age of the individual                |
| `Weight`      | Weight in pounds                     |
| `Height`      | Height in inches                     |
| ...           | Other physical measurements          |


## Project Workflow

### 1. Data Analysis & Preprocessing
Performed exploratory data analysis (EDA) using `pandas`, `seaborn`, and `matplotlib`. Key insights include correlations between features and target variable (`BodyFat`).

### 2. Model Training
Implemented multiple regression models in [model.ipynb](./model.ipynb):
- Linear Regression
- Lasso Regression
- Ridge Regression

Additional models explored in [ADS-Project-models-2.ipynb](./ADS-Project-models-2.ipynb):
- Random Forest Regressor
- Gradient Boosting Regressor

### 3. Model Comparison
Compared performance metrics like R² score and Mean Squared Error across models in [ADS-Project-models-comparision.ipynb](./ADS-Project-models-comparision.ipynb).

### 4. Deployment with Flask
Created a Flask web app ([app.py](./app.py)) for user interaction:
- Users input their physical measurements.
- The trained model predicts body fat percentage.

## Results

The best-performing model achieved:
- **R² Score**: 0.92
- **Mean Squared Error**: 3.5%


## License

This project is licensed under the MIT License - see the [LICENSE](./LICENSE) file for details.
