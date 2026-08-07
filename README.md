# 📊 Stress Level Prediction Using Lifestyle and Sleep Health Data

## 📝 Overview
In this project, I built a machine learning model to predict stress levels using daily habits like sleep and physical activity. My goal was to explore lifestyle data and find hidden patterns that affect mental health.

## 🗂️ Dataset
The dataset utilized in this project is sourced from Kaggle and contains comprehensive medical and lifestyle records. 
Key features include:
*   **Sleep Metrics:** Sleep Duration, Quality of Sleep.
*   **Physical Metrics:** Physical Activity Level, Heart Rate, BMI Category.
*   **Medical Data:** Blood Pressure, Presence of Sleep Disorders.
*   **Demographics:** Gender, Occupation.

## ⚙️ Data Preprocessing & Cleaning
To ensure the highest quality of data for our Machine Learning model, a rigorous data cleaning and feature engineering pipeline was implemented:
1.  **Handling Missing Values:** Conducted initial checks to ensure data integrity.
2.  **Feature Engineering (Blood Pressure):** Extracted numerical data from the text-based 'Blood Pressure' column by splitting it into two distinct continuous variables: `Systolic_BP` and `Diastolic_BP` (converted to float).
3.  **Data Standardization:** Merged overlapping categories (e.g., replacing 'Normal Weight' with 'Normal' in the BMI Category).
4.  **Categorical Encoding:** Applied `LabelEncoder` from Scikit-learn to convert categorical text data (Gender, Occupation, BMI Category, Sleep Disorder) into machine-readable numeric formats.
5.  **Target Isolation:** Dropped non-predictive identifiers (like `Person ID`) and isolated `Stress Level` as the target variable (y).

## 🏆 Results
The Random Forest model demonstrated exceptional predictive capabilities on the testing subset:
*   **Overall Accuracy:** **98.67%**

This high level of accuracy indicates that the chosen lifestyle and physiological features are strong indicators of an individual's stress level, and the model has successfully minimized the noise to capture the underlying patterns.

## 💻 Technologies Used
*   **Python 3**
*   **Pandas** (Data manipulation and analysis)
*   **Scikit-learn** (Machine Learning, Preprocessing, and Evaluation)
*   **Google Colab** (Development Environment)

## 🚀 How to Run
1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/lianafarsi/Sleep-Stress-Model.git
