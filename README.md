# Credit_Risk_Prediction
Machine learning–based credit risk prediction system using the German Credit dataset.
## 📊 Credit Risk Modeling using Machine Learning
### 📌 Project Overview

This project focuses on building a **credit risk prediction model** using machine learning techniques. The goal is to classify credit applicants as **low risk (good)** or **high risk (bad)** based on their personal and financial information.

The project covers the full data science pipeline:

- Data exploration and visualization

- Data cleaning and preprocessing

- Feature engineering

- Machine learning model training and evaluation

- Preparation for deployment using a web application interface

### 📂 Dataset

The dataset used is the **German Credit Risk Dataset**, obtained from Kaggle. It contains information about loan applicants and their associated credit risk.

**Key characteristics:**

- 1 CSV file

- 11 columns

- 6 categorical features

- 5 numerical features

**Main columns:**

- age

- sex

- job

- housing

- saving accounts

- checking account

- credit amount

- duration

- purpose

- risk (target variable: good or bad)

**Target:**

- good → low credit risk

- bad → high credit risk

### 🔍 Data Exploration

**Initial exploration showed:**

- Average applicant age ≈ **35 years**

- Class imbalance:

- 700 good

- 300 bad

**Libraries used:**

- pandas

- numpy

- matplotlib

- seaborn

**Visualizations included:**

- Age distribution plots

- Histograms of numerical variables

- Box plots for outlier detection

### 🧹 Data Cleaning

**Rows with missing values in:**

- saving accounts

- checking account
**were removed as these are important indicators of financial status.***

**After cleaning:**

Final dataset size: 520 rows × 11 columns

### 📈 Exploratory Data Analysis
**Univariate Analysis**

**Histograms for:**

- age

- credit amount

- duration

**Box plots revealed:**

- Most applicants are relatively young

- Credit amounts are generally moderate

- Loan duration varies significantly

**Bivariate Analysis**

- Gender-based comparison of credit amount

- Housing type vs loan purpose

- Correlation between credit amount and duration (moderate positive correlation)

- Higher credit amounts were associated with higher risk levels

- Scatter plots and pivot tables were used to visualize relationships between:

&emsp;- Age

&emsp;- Credit amount

&emsp;- Duration

&emsp;- Risk

### 🧠 Feature Engineering

**Selected features:**

- age
  
- sex

- job

- housing

- saving accounts

- checking account

- credit amount

- duration

**Target variable:**

- risk

**Processing steps:**

- Categorical features were encoded using Label Encoding

- Scaling was not applied since tree-based models do not require it

### 🤖 Model Training

The dataset was split into training and testing sets using **train_test_split**.

**Models trained:**

- Decision Tree Classifier

- Random Forest Classifier

- Extra Trees Classifier

- XGBoost Classifier

**Techniques used:**

- GridSearchCV for hyperparameter tuning

- Parallel processing using n_jobs = -1

📊 Model Evaluation

Models were evaluated using accuracy score and best parameter selection.

**Results:**

- Extra Trees Classifier achieved the highest accuracy: 0.66

- XGBoost Classifier achieved an accuracy of 0.63, using parameters adjusted for class imbalance

Comparison of multiple models helped identify the best-performing algorithm.

### 🛠️ Technologies Used

- Python

- Pandas

- NumPy

- Matplotlib

- Seaborn

- Scikit-learn

- XGBoost

- Jupyter Notebook

### 📁 Project Structure

├── data/<br>
│   └── credit_data.csv <br>
├── notebooks/ <br>
│   └── credit_risk_model.ipynb <br>
├── models/ <br>
│   └── trained_model.pkl <br>
├── encoders/ <br>
│   └── label_encoders.pkl <br>
└── README.md <br>

🚀 Future Improvements

- Handle class imbalance using SMOTE or class weighting

- Add cross-validation metrics

- Improve feature engineering

- Deploy using Streamlit or Flask

- Add ROC curve and confusion matrix

## 👨‍💻 Author

### Abdul Wahab
**Data Science & analytics Intern**
**DevelopersHub Corporation**
