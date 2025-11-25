# House Price Prediction using Linear Regression

## Project Overview
This project demonstrates an **end-to-end workflow for predicting house prices** using a simple Linear Regression model. The goal is to understand how the area of a house affects its price and to build a model that can predict prices for unseen areas. The project covers **data loading, preprocessing, visualization, model training, evaluation, and prediction**.

---

## Datasets
Three datasets were used in this project:  
1. **areas.csv** – Contains a list of areas (in square feet) for which house prices need to be predicted.  
2. **homeprices.csv** – Contains historical house data with `area` and `price`.  
3. **homeprices-m.csv** – Similar to `homeprices.csv` but with additional features: `bedrooms` and `age`, including some missing values.

---

## Workflow & Detailed Steps

### 1. Data Loading & Inspection
- Loaded datasets using **pandas**.
- Displayed the first few rows of each dataset to understand their structure.
- Checked data types and missing values using `.info()` and `.isnull()`.
- Calculated summary statistics with `.describe()` for numeric insights.

### 2. Handling Missing Values
- `homeprices-m.csv` had missing `bedrooms` values.
- Filled missing values using the **median** to ensure no data is lost.

### 3. Data Visualization
- Explored the relationship between **area** and **price** using scatter plots.
- Confirmed a **linear relationship**, validating the use of Linear Regression.

### 4. Data Preparation
- Defined **feature (`X`)** as `area` and **target (`y`)** as `price`.
- Split data into **training and testing sets** (33% test size) for model evaluation.

### 5. Model Building & Training
- Built a **Linear Regression model** using scikit-learn.  
- Trained the model on the training set, fitting a line to minimize differences between predicted and actual prices.

### 6. Model Testing & Predictions
- Predicted prices for the **test set** and compared them to actual prices.
- Predicted prices for the full `areas.csv` dataset for new areas.

### 7. Model Evaluation
- Metrics calculated:
  - **Mean Absolute Error (MAE)**  
  - **Mean Squared Error (MSE)**  
  - **Root Mean Squared Error (RMSE)**  
  - **R² Score**  
- Model performance showed **high accuracy**.

### 8. Visualization of Predictions
- **Actual vs Predicted Prices:** Visual assessment of prediction accuracy.
- **Regression Line:** Plotted predicted prices alongside actual data with annotated equation.

### 9. Insights
- The **linear model** effectively captures the relationship between area and price.  
- Small deviations exist due to unaccounted factors like location, age, or number of bedrooms.  
- The model can now predict house prices for any given area within the data range.

---

## Skills Demonstrated
- **Data Analysis:** Pandas, NumPy  
- **Data Visualization:** Matplotlib, Seaborn  
- **Data Preprocessing:** Handling missing values, feature selection  
- **Machine Learning:** Linear Regression, train-test split  
- **Model Evaluation:** MAE, MSE, RMSE, R²  
- **Workflow:** End-to-end project pipeline from data loading to prediction and visualization

---

## Outputs / Visualizations
- Scatter plots of Area vs Price  
- Actual vs Predicted price plots  
- Regression line plots with prediction equation annotated  

---

