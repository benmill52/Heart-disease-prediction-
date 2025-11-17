❤️ Heart Disease Prediction Using Machine Learning

A Complete End-to-End Machine Learning Project

This project explores the application of machine learning techniques to predict the likelihood of heart disease based on clinical patient data. It follows a full data science workflow — from data cleaning and exploratory data analysis (EDA) to feature engineering, modeling, evaluation, and insights.

The goal is to build a reliable and interpretable predictive model that can support early detection of heart disease.

🔍 Project Motivation

Heart disease is one of the major global health challenges, and early diagnosis significantly improves survival rates. Machine learning offers a scientific way to analyze medical attributes and estimate risk patterns.
This project applies ML techniques to uncover patterns in patient records and build a prediction model that achieves high performance and interpretability.

📊 Dataset

Source: Heart Disease dataset (Cleveland-based)

Rows: ~300

Features: 14 clinical attributes

Target: 1 = Heart Disease Present, 0 = No Disease

Common attributes include:

Age

Sex

Chest pain type

Resting blood pressure

Cholesterol

Fasting blood sugar

Resting ECG

Max heart rate

Exercise-induced angina

ST depression (oldpeak)

Slope

Number of major vessels

Thalassemia

🔧 Project Workflow
1. Data Cleaning

No missing values

Over 700 duplicates detected (if working with extended dataset) and removed

Consistency checks across numerical features

Outlier inspection

Verified that no feature requires encoding again (dataset already encoded)

2. Exploratory Data Analysis (EDA)

The EDA covered:

Univariate analysis of each clinical variable

Distribution plots (histogram, KDE)

Outlier analysis

Correlation heatmap

Feature–target relationships

Boxplots comparing each feature across target classes

Insights on medically meaningful patterns

Examples of insights:

Patients with higher oldpeak, thal, and cp tend to show higher disease rates

Maximum heart rate and ST slope showed strong separations between classes

Age distribution clusters between 40–60

3. Feature Engineering

Standardization using StandardScaler

Feature importance ranking

Checking variance contribution

Removal of redundant or highly correlated features (if necessary)

4. Modeling

Several algorithms were tested:

Logistic Regression

KNN

SVM

Random Forest

XGBoost

Gradient Boosting

Best Performing Model:
✔ Logistic Regression — provides explainability and stable performance
✔ Balanced simplicity + accuracy

The model was saved as Best_log_model.pkl.

5. Model Evaluation

Metrics used:

Accuracy

Precision

Recall

F1-score

ROC–AUC

Confusion matrix

Key Highlights:

High recall — important for medical diagnosis

AUC score indicates strong discrimination ability

Confusion matrix shows reduced false negatives after scaling

6. Deployment Preparation

Saved the trained model

Saved the scaler for consistent preprocessing

Built a prediction pipeline

(Optional) Streamlit app created for interactive use

📁 Project Structure
│── data/             
│── notebooks/        
│── h_app.py                 # Optional Streamlit application
│── Best_log_model.pkl       # Best performing model
│── scaler.pkl               # Scaler used for preprocessing
│── requirements.txt 
│── README.md

🧠 Key Learnings

This project strengthened my skills in:

Handling duplicates and validating dataset integrity

Conducting detailed EDA for medical datasets

Understanding feature influence on disease prediction

Comparing and selecting the best ML model

Building standardized ML pipelines

Deploying ML models using Streamlit

🚀 Future Improvements

Experiment with deep learning (ANN)

Add SHAP explainability

Expand dataset for more generalizable predictions

Integrate patient trend analysis (time series)

Deploy as a mobile-friendly health screening tool

🤝 Contributions

Feel free to fork, add new models, improve visualizations, or open issues.

📜 License

Open for educational and research purposes.
