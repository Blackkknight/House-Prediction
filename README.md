# Housing Price Prediction (Machine Learning Project)

## Overview

This project focuses on predicting housing prices using machine learning techniques on the California Housing dataset. It demonstrates a complete workflow including data preprocessing, model training, evaluation, and inference.

The objective is to build a regression model that can estimate house prices based on factors such as income, location, and housing attributes.

---

## Features

* End-to-end machine learning pipeline
* Data preprocessing using Scikit-learn pipelines
* Stratified sampling for balanced data splitting
* Random Forest Regressor for prediction
* Model saving and loading using Joblib
* CSV-based input and output handling

---

## Tech Stack

* Python
* Pandas, NumPy
* Scikit-learn
* Joblib

---

## Project Structure

```
.
├── train.py
├── housing.csv
├── input.csv
├── output.csv
├── requirements.txt
├── README.md
```

---

## Workflow

### Data Preprocessing

* Separates numerical and categorical features
* Applies transformations using pipelines
* Uses stratified sampling based on income categories

### Model Training

* Trains a Random Forest Regressor
* Fits the model on processed training data
* Saves the trained model for reuse

### Inference

* Loads the saved model and pipeline
* Reads input data from `input.csv`
* Generates predictions and stores them in `output.csv`

---

## How to Run

Install dependencies:

```
pip install -r requirements.txt
```

Run the project:

```
python train.py
```

---

## Model Performance

* Metric used: RMSE (Root Mean Squared Error)
* Achieved RMSE: ~47,000

This indicates a reasonable prediction error for housing price estimation.

---

## Future Improvements

* Hyperparameter tuning using GridSearchCV
* Experiment with advanced models (Gradient Boosting, XGBoost)
* Improve feature engineering
* Deploy as a web application

---

## Key Learnings

* Building and using preprocessing pipelines
* Avoiding data leakage
* Evaluating regression models using RMSE and cross-validation
* Implementing an end-to-end ML workflow

---

## License

This project is created for learning and educational purposes.

