# housing-price-prediction
📌 Project Overview

This project builds and evaluates machine learning models to predict median house values using demographic and geographic data.
The goal is to demonstrate an end-to-end data analysis and machine learning workflow, from data cleaning and exploration to modeling, evaluation, and interpretation.

🎯 Objective

To predict median house prices based on features such as income, population, housing characteristics, and location, and to compare the performance of linear and non-linear regression models.

📊 Dataset

The project uses the California Housing dataset, which includes:

- Median income
- Housing age
- Total rooms and bedrooms
- Population and households
- Geographic location
- Proximity to the ocean (categorical)

🛠️ Tools & Libraries

- Python
- pandas, numpy – data manipulation
- matplotlib, seaborn – data visualization
- scikit-learn – modeling and evaluation
  
🔎 Approach

1. Data Loading & Inspection
Loaded the dataset and examined structure, data types, and summary statistics.

2. Data Cleaning
Handled missing values by imputing the median for numerical features.

3. Exploratory Data Analysis (EDA)
Analyzed distributions, correlations, and relationships between features and the target variable using histograms, scatter plots, boxplots, and a correlation heatmap.

4. Categorical Encoding
Converted the ocean_proximity categorical variable into numerical features using one-hot encoding.

5. Feature Engineering
Created new ratio-based features (e.g. rooms per household, population per household) and applied log transformation to reduce skewness.

6. Data Preparation & Scaling
Split the data into training and testing sets and applied feature scaling where appropriate.

7. Model Training

- Linear Regression (baseline model)
- Random Forest Regressor (non-linear model)

8. Model Evaluation
Evaluated models using RMSE and R² score.

9. Model Interpretation

- Feature importance analysis
- Error analysis using actual vs. predicted values

📈 Results

Random Forest outperformed Linear Regression, achieving a lower RMSE and higher R² score.
Median income was the most influential feature, followed by geographic variables such as latitude and longitude.
Error analysis showed that higher-priced houses tend to be slightly underpredicted.

🧠 Key Insights

Income level and location are strong drivers of housing prices.
Tree-based models handle non-linear relationships and outliers better than linear models.
Visual error analysis provides insights beyond aggregate metrics.
