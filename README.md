# 🏠 Housing Price Prediction Using Linear Regression

## 📌 Project Overview

This project focuses on predicting housing prices using **Linear Regression** and other regularized regression techniques. It demonstrates an end-to-end **machine learning workflow**, including data loading, data cleaning, feature engineering, preprocessing, model training, and model evaluation.

The project uses structured housing data containing both **numerical and categorical features**, with `SalePrice` as the target variable.

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python) ![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Regression-orange) ![Scikit-learn](https://img.shields.io/badge/scikit--learn-ML-yellow?logo=scikit-learn) ![Status](https://img.shields.io/badge/Status-Completed-success) ![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)

---

## 🎯 Project Objectives

* Analyze housing data and understand feature relationships
* Clean and preprocess the dataset
* Handle missing values effectively
* Transform categorical variables into numerical features
* Build regression models for house price prediction
* Compare different regression techniques
* Evaluate model performance using Mean Absolute Error (MAE)

---

## 📊 Dataset Information

* **Dataset:** `House_Price.csv`
* **Total Records:** 2918
* **Total Columns:** 13
* **Target Variable:** `SalePrice`

The dataset contains both **numerical and categorical housing attributes**, including:

* `MSSubClass`
* `MSZoning`
* `LotArea`
* `LotConfig`
* `BldgType`
* `OverallCond`
* `YearBuilt`
* `YearRemodAdd`
* `Exterior1st`
* `BsmtFinSF2`
* `TotalBsmtSF`
* `SalePrice`

The original dataset contains **2919 rows**, with 1460 records containing known `SalePrice` values and 1459 records with missing `SalePrice`, which were treated as the prediction/test portion of the dataset.

---

## 🛠️ Tools & Technologies Used

* **Python**
* **Pandas** – Data manipulation and analysis
* **NumPy** – Numerical operations
* **Matplotlib** – Data visualization
* **Seaborn** – Statistical visualization
* **Scikit-learn** – Machine learning and preprocessing
* **Jupyter Notebook** – Development and experimentation

---

## 📂 Project Folder Structure

```text
├── Notebook/
│   └── House Price Prediction.ipynb    # Analysis Notebook
│
├── Data/
│   └── HousePricePrediction.csv        # CSV File
│
├── README.md                           # Project documentation
└── requirements.txt                    # Project Requirements
```

---

## 🔍 Project Workflow

### Phase 1: Setup and Data Loading

* Imported libraries required for data manipulation, visualization, preprocessing, and machine learning
* Loaded the housing dataset into a Pandas DataFrame
* Performed initial dataset inspection using `shape()`, `head()`, and `tail()`
* Examined the dataset structure and target variable
* Identified missing values in `SalePrice`

---

### Phase 2: Data Cleaning and Feature Preparation

* Checked the dataset for duplicate records
* Removed duplicate records using `drop_duplicates()`
* Dropped the `Id` column because it is a unique identifier and does not provide meaningful predictive information
* Analyzed missing values across the dataset
* Identified missing `SalePrice` values
* Separated the dataset into training and prediction/test portions based on the availability of `SalePrice`
* Separated the feature variables (`X_train`) from the target variable (`y_train`)
* Combined training and test features to ensure consistent preprocessing

---

### Phase 3: Feature Engineering and Preprocessing

#### Numerical Features

* Identified numerical feature columns
* Used `SimpleImputer(strategy='mean')` to handle missing numerical values
* Replaced missing numerical values with the corresponding column mean

#### Categorical Features

* Identified categorical feature columns
* Converted categorical values to string format
* Applied `OneHotEncoder` to transform categorical variables into numerical binary features
* Removed the original categorical columns
* Merged the encoded features with the numerical features

The resulting dataset was converted into a **fully numerical feature matrix** suitable for machine learning models.

---

### Phase 4: Model Training and Evaluation

The processed dataset was divided into training and validation sets using:

* **Training Set:** 80%
* **Validation Set:** 20%
* **Random State:** `42`

Feature scaling was also explored using `MinMaxScaler`.

Three regression models were trained and evaluated:

1. **Linear Regression**
2. **Lasso Regression**
3. **Ridge Regression**

---

## 📈 Model Performance

The models were evaluated using **Mean Absolute Error (MAE)**.

| Model             |       MAE |
| ----------------- | --------: |
| Linear Regression | 27,838.79 |
| Lasso Regression  | 27,838.80 |
| Ridge Regression  | 29,906.49 |

### 🏆 Best Performing Models

**Linear Regression** achieved an MAE of **27,838.79**, while **Lasso Regression** achieved an almost identical MAE of **27,838.80**.

Ridge Regression produced a higher MAE of **29,906.49**.

A lower MAE indicates that the model's predictions are, on average, closer to the actual house prices.

---

## 📌 Key Findings

* Linear Regression provided the lowest MAE among the evaluated models.
* Lasso Regression performed almost identically to Linear Regression.
* Ridge Regression produced a comparatively higher MAE.
* One-hot encoding successfully transformed categorical housing features into numerical variables.
* Mean imputation provided a straightforward approach for handling missing numerical values.
* Proper separation of records based on `SalePrice` availability allowed the known-price records to be used for model training.

---

## 🧠 Key Learnings

* Understanding and inspecting real-world datasets
* Handling missing values
* Removing unnecessary features
* Separating features and target variables
* Numerical feature imputation
* One-hot encoding of categorical variables
* Feature scaling using MinMaxScaler
* Implementing Linear Regression
* Implementing Lasso and Ridge Regression
* Comparing regression models using MAE
* Building an end-to-end machine learning workflow

---

## 🚀 Future Improvements

The project can be further improved by:

* Performing more extensive exploratory data analysis
* Applying feature selection techniques
* Using cross-validation for more reliable model evaluation
* Performing hyperparameter tuning for Lasso and Ridge Regression
* Testing additional regression algorithms such as Random Forest, Gradient Boosting, and XGBoost
* Evaluating additional metrics such as RMSE and R² Score
* Building a deployment interface for interactive house price predictions

---

## 🧑‍💻 Author

**👤 Harsh Belekar**  
📍 Data Analyst | Python Developer | SQL | Power BI | Excel | Data Visualization  
📬 [LinkedIn](https://www.linkedin.com/in/harshbelekar) | 🔗[GitHub](https://github.com/Harsh-Belekar)

📧 [harshbelekar74@gmail.com](mailto:harshbelekar74@gmail.com)

---

⭐ *If you found this project helpful, feel free to star the repo and connect with me for collaboration!*
