# 🏠 Housing Price Prediction Using Linear Regression

## 📌 Project Overview
This project was completed as **Task 1** during my **Data Science Internship at HexSoftware**.  
The objective of this project is to build and evaluate **linear regression models** to predict house prices using structured real-world housing data.

The project demonstrates an **end-to-end data science workflow**, including data cleaning, feature engineering, preprocessing, model training, and evaluation.

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python) ![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Linear%20Regression-orange) ![Scikit-learn](https://img.shields.io/badge/scikit--learn-ML-yellow?logo=scikit-learn) 
---

## 🎯 Project Objectives
- Analyze housing data and understand feature relationships
- Clean and preprocess raw data
- Handle missing values effectively
- Build regression models for price prediction
- Compare model performance using evaluation metrics

---

## 📊 Dataset Information
- **Dataset Name:** House_Price.csv  
- **Total Records:** 2918  
- **Total Features:** 13  
- **Target Variable:** `SalePrice`

The dataset contains both **numerical and categorical** housing attributes such as lot area, building type, year built, basement area, and zoning.

---

## 🛠️ Tools & Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

---

## 🔍 Project Workflow

### Phase 1: Setup and Data Loading
- Imported required libraries for data manipulation, visualization, preprocessing, and modeling
- Loaded the dataset into a Pandas DataFrame
- Performed initial inspection using `shape()`, `head()`, and `tail()`
- Identified missing values in the target variable indicating combined training and testing data

---

### Phase 2: Data Cleaning and Feature Preparation
- Checked for and removed duplicate records
- Dropped unnecessary identifier column (`Id`)
- Analyzed missing values across all features
- Split the dataset into training and testing sets based on target availability
- Separated features and target variable
- Recombined feature datasets to ensure consistent preprocessing

---

### Phase 3: Feature Engineering and Preprocessing
- Identified numerical and categorical feature columns
- Imputed missing numerical values using **mean imputation**
- Converted categorical features to string format
- Applied **One-Hot Encoding** to categorical variables
- Created a final numerical feature matrix suitable for modeling

---

### Phase 4: Model Training and Evaluation
- Split training data into training and validation sets (80/20)
- Applied **MinMaxScaler** for feature normalization
- Trained and evaluated the following models:
  - Linear Regression
  - Lasso Regression (L1 Regularization)
  - Ridge Regression (L2 Regularization)

#### 📈 Model Performance (Mean Absolute Error)

| Model              | MAE        |
|-------------------|------------|
| Linear Regression | 27,838.79  |
| Lasso Regression  | 27,838.80  |
| Ridge Regression  | 29,906.49  |

---

## 📌 Conclusion
- Linear Regression and Lasso Regression achieved the **best performance** with an MAE of approximately **$27,838**
- On average, the model predictions deviated by about **$27,838** from actual house prices
- Ridge Regression performed slightly worse compared to the other models
- The project demonstrates effective data preprocessing, feature engineering, and model evaluation techniques

---

## 🧠 Key Learnings
- Handling real-world datasets with missing values
- Feature engineering and preprocessing techniques
- Implementation of linear and regularized regression models
- Model evaluation using Mean Absolute Error (MAE)
- End-to-end machine learning project workflow

---

## 🏢 Internship Credit
This project was completed as **Task 1** during my **Data Science Internship at HexSoftware**.

---

## 🧑‍💻 Author

**👤 Harsh Belekar**  
📍 Data Analyst | Python | SQL | Power BI | Excel | Data Visualization  
📬 [LinkedIn](https://www.linkedin.com/in/harshbelekar) | 🔗 [GitHub](https://github.com/Harsh-Belekar)

📧 [harshbelekar74@gmail.com](mailto:harshbelekar74@gmail.com)

---

⭐ *If you liked this project, don’t forget to star the repo and connect with me on LinkedIn!*

