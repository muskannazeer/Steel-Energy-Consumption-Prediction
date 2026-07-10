# Steel Industry Energy Consumption Prediction

## Project Overview

This project focuses on predicting energy consumption in the steel industry using machine learning regression models. The project includes Exploratory Data Analysis (EDA), feature engineering, data preprocessing, and baseline model development to identify the most suitable regression algorithm for predicting electricity usage.

---

## Dataset

**Dataset Name:** `Steel_industry_data.csv`

The dataset contains electricity consumption records from a steel manufacturing industry along with operational and electrical parameters.

---

## Project Objectives

* Perform Exploratory Data Analysis (EDA)
* Identify data quality issues
* Create meaningful engineered features
* Prepare the dataset for machine learning
* Train multiple baseline regression models
* Compare model performance using different evaluation metrics
* Select the best-performing model

---

## Feature Engineering

The following new features were created:

* Hour
* Day
* Month
* Day_Type (Weekday/Weekend)
* Power_Factor_Ratio
* High_Load (used only during EDA and excluded from modeling to prevent data leakage)

---

## Data Preprocessing

The following preprocessing steps were performed:

* Converted the `date` column to datetime format
* Extracted time-based features
* Checked missing values
* Removed duplicate records
* Detected outliers using the IQR method
* Applied One-Hot Encoding to categorical variables
* Removed unnecessary columns before model training

---

## Machine Learning Models

The following baseline regression models were implemented:

* Linear Regression
* Ridge Regression
* Decision Tree Regressor
* Random Forest Regressor

---

## Model Evaluation

The models were evaluated using:

* Mean Absolute Error (MAE)
* Root Mean Squared Error (RMSE)
* R² Score
* 5-Fold Cross Validation

---

## Best Model

Among all the evaluated models, **Random Forest Regressor** achieved the best performance with the lowest prediction error and the highest R² score, making it the most suitable model for this dataset.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook

---

## Project Structure

```text
Project/
│
├── Steel_industry_data.csv
├── steel_energy_engineered.csv
├── week2_eda.ipynb
├── week2_baseline_models.ipynb
├── requirements.txt
└── README.md
```

---

## How to Run

1. Clone the repository.
2. Install the required libraries:

```bash
pip install -r requirements.txt
```

3. Open `week2_eda.ipynb` to perform exploratory data analysis.
4. Open `week2_baseline_models.ipynb` to train and evaluate the regression models.

---

## Results

The project successfully completed exploratory data analysis, feature engineering, baseline model development, and performance evaluation. Random Forest Regressor produced the highest prediction accuracy among all evaluated baseline models.
