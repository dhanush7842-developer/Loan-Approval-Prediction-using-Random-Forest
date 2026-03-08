# Loan Approval Prediction using Random Forest

This project aims to predict the loan approval status of applicants based on various features such as gender, marital status, education, income, and credit history. It utilizes a **Random Forest Classifier** to achieve high accuracy and robustness.

## 🚀 Features

- **Data Preprocessing**: Comprehensive handling of missing values (median for numeric, mode for categorical).
- **Feature Engineering**: Automatic encoding of categorical variables.
- **Model Training**: Implementation of a Random Forest Classifier with 100 estimators.
- **Robust Evaluation**: Includes 5-fold cross-validation and detailed classification reports.
- **Model Persistence**: Saves the trained model using `joblib` for future deployment.
- **Interactive Showcase**: A premium web-based visualization of model performance and insights.

## 🎨 Interactive Showcase

The project includes a standalone **Interactive Showcase** (`loan-showcase.html`) that provides a premium visual overview of the model's performance.

### Key Features:
- **Live Metrics**: Real-time animation of Accuracy, Cross-Validation scores, and Approval rates.
- **Feature Importance**: Dynamic bar chart showing which factors (like Credit History) drive the model's decisions.
- **Accuracy Breakdown**: Visual representation of correct vs. incorrect predictions on the test set.
- **Data Insights**: Curated findings discovered during the analysis of 500 applicants.

To view it, simply open `loan-showcase.html` in any modern web browser.


## 📊 Dataset

The project uses `loan_application.csv`, which includes:
- **Demographics**: Gender, Married, Dependents, Education, Self_Employed.
- **Financial Details**: ApplicantIncome, CoapplicantIncome, LoanAmount, Loan_Amount_Term, Credit_History, Property_Area.
- **Target**: `Loan_Status` (Y/N).

## 📈 Results

The model achieved the following performance:
- **Test Set Accuracy**: **87%**
- **Cross-Validation Mean Accuracy**: **79% (+/- 0.06)**

### Feature Importance
The project provides a sorted visualization of feature importance, highlighting that **Credit History**, **Total Income**, and **Loan Amount** are the most significant predictors.

## 🛠️ Requirements

- Python 3.x
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Joblib

## 📖 Usage

1. Open `Random Forest.ipynb` in a Jupyter Notebook environment.
2. Run all cells to load data, preprocess, train the model, and evaluate performance.
3. The final model will be saved as `loan_rf_model.pkl`.

---
*Created as part of the Loan Approval Prediction project.*
