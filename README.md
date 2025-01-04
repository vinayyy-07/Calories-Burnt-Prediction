# Calories-Burnt-Prediction


# Objective:
The project aims to build a machine learning model to predict the number of calories burned based on various exercise-related parameters such as age, gender, duration, and heart rate.

1.Data Collection and Preprocessing:

i.Datasets:
Two datasets were used: exercise.csv, which contains user exercise details, and calories.csv, which provides the corresponding calories burned.

ii.Exploratory Data Analysis (EDA):
Checked for missing values and gained insights using descriptive statistics and visualizations (e.g., count plots for gender and distribution plots for age and weight).
Created a correlation heatmap to understand relationships between variables.

iii.Data Cleaning and Transformation:
Merged the datasets into a single DataFrame using pandas.concat().
Encoded the categorical variable "Gender" (male as 0, female as 1) for machine learning compatibility.

# 2.Feature Selection:

Dropped irrelevant columns such as User_ID and the target variable Calories.
The input features (X) and target (Y) were separated for model training.

# 3.Model Development:

 i.Algorithm Used:
  Employed the XGBoost Regressor (XGBRegressor), a gradient-boosting algorithm optimized for performance and speed.
ii.Data Splitting:
  Divided the dataset into training (80%) and testing (20%) sets using train_test_split.
iii.Training:
  Wrapped the model training (model.fit) in a custom function to ensure modularity and handle compatibility issues.
iv.Prediction:
  Predicted calorie burn for the test dataset.
  
# 4.Evaluation:

Calculated the Mean Absolute Error (MAE) to measure model accuracy. The MAE indicates how close the predicted values are to the actual values.
