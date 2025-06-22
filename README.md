# Rainfall-Prediction-project
🌧️ Rainfall Prediction Using Machine Learning
📌 Project Overview:
This project focuses on predicting whether it will rain the next day (`RainTomorrow`) using historical weather data. The analysis is done using Python in a Jupyter Notebook and involves preprocessing, exploratory data analysis (EDA), model building, and evaluation.
🧠 Problem Statement:
The goal is to build a classification model that accurately predicts the occurrence of rainfall based on various meteorological features such as temperature, humidity, pressure, and wind speed.
📁 Dataset:
- **Source**: [Rainfall in Australia dataset](https://www.kaggle.com/datasets/jsphyg/weather-dataset-rattle-package)
- **Target Variable**: `RainTomorrow` (Yes/No)
- **Features Include**:
  - Temperature (MinTemp, MaxTemp)
  - Rainfall
  - WindGustSpeed, WindSpeed9am, WindSpeed3pm
  - Humidity9am, Humidity3pm
  - Pressure9am, Pressure3pm
  - Cloud9am, Cloud3pm
  - Sunshine, Evaporation, RainToday

🔍 Methodology
1. Data Cleaning & Preprocessing
- Handled missing values by dropping or imputing relevant columns.
- Encoded categorical variables (e.g., `RainToday`, `RainTomorrow`) using Label Encoding.
- Converted wind directions to numerical values if applicable.
- Addressed class imbalance using techniques like undersampling or oversampling (if needed).

2. Exploratory Data Analysis (EDA)
- Analyzed distributions of weather features.
- Visualized correlations using heatmaps and pairplots.
- Examined which features have the most influence on rainfall.

3. Feature Selection
- Selected important features such as:
  - `Humidity3pm`, `Pressure9am`, `WindGustSpeed`, `Rainfall`, `RainToday`

4. Model Building
Used the following classification models:
- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier

5. Model Evaluation
- Evaluated models using:
  - Accuracy Score
  - Confusion Matrix
  - Precision, Recall, and F1-Score
- Compared model performances and selected the best one.

📈 Key Findings
- **Random Forest Classifier** outperformed other models with the highest accuracy.
- **Humidity at 3 PM**, **Rainfall**, and **RainToday** were strong predictors of future rainfall.
- Visual analysis showed a significant drop in pressure and rise in humidity on rainy days.

📊 Technologies Used
- Python 3.x
- Jupyter Notebook
- Pandas, NumPy
- Seaborn, Matplotlib
- Scikit-learn (ML models and metrics)
