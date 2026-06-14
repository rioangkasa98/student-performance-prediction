# 🎓 Predicting Student Performance: A Linear Regression Approach

## 📌 The Idea
I've always been curious about what actually drives academic success. Is it purely the number of hours spent staring at a book, or do things like sleep and extracurricular activities matter more than we think? 

This project is my attempt to answer that using data. I built an end-to-end Machine Learning project using **Multiple Linear Regression** to predict a student's `Performance Index`. To keep things professional and organized, I followed the **CRISP-DM** (Cross-Industry Standard Process for Data Mining) framework—from exploring the raw data to exporting the final model.

## 🗂️ The Data
The dataset contains records of students with the following features:
* `Hours Studied`: Number of hours spent studying per day.
* `Previous Scores`: The score obtained in the previous test.
* `Extracurricular Activities`: Whether the student participates in after-school clubs (Yes/No).
* `Sleep Hours`: Average hours of sleep per night.
* `Sample Question Papers Practiced`: Number of practice tests completed.
* **`Performance Index`**: The target variable we are trying to predict.

## 🛠️ Tech Stack
* **Python** * **Pandas & NumPy** (Data cleaning and manipulation)
* **Matplotlib & Seaborn** (Data visualization)
* **Scikit-Learn** (Building and evaluating the regression model)
* **Joblib** (Model serialization/deployment)

## 📊 Key Findings & Results
The model performed surprisingly well! Here are the evaluation metrics on the unseen test data:
* **R-squared ($R^2$)**: 0.98 
* **Mean Absolute Error (MAE)**: 1.61

**What did the math actually tell us?**
1. **Past success is the best predictor:** `Previous Scores` had the heaviest weight. It shows that academic performance is compounding.
2. **Hard work pays off (literally):** There is a clear, mathematical linear trend between `Hours Studied` and the final index. 
3. **Burnout isn't the answer:** The model showed that `Sleep Hours` and `Extracurricular Activities` actually have a positive impact. You don't need to skip sleep to get good grades.

## 🚀 How to Run This Locally
If you want to play around with the data or test the model yourself:

1. Clone this repo:
   ```bash
   git clone https://github.com/rioangkasa98/student-performance-prediction.git
