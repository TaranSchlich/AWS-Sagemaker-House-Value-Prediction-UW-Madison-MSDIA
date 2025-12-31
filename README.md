# SageMaker Housing Value Prediction  
Machine Learning with Amazon SageMaker  

**By: Taran Schlichtmann**

**Date: 11/29/2025**

Demonstrates the use of Amazon SageMaker Canvas to build a machine learning model that predicts median home values using the California housing dataset. The workflow includes model creation, data validation, feature impact analysis, and batch prediction generation.

---

## Project Overview

The goal of this assignment was to:

- Build a predictive model in SageMaker Canvas  
- Use the “canvas-sample-housing.csv” dataset  
- Predict the **median_house_value** column  
- Validate data quality and distribution  
- Generate batch predictions for a new dataset  
- Export predictions as a CSV file  

This project simulates a real-world ML workflow where a business needs automated home value predictions for planning, pricing, or investment decisions.

---

## Model Development in SageMaker Canvas

### Model Setup
- Tool: **Amazon SageMaker Canvas**  
- Model name: **housing_model**  
- Target column: **median_house_value**  
- Build type: **Quick Build**  
- Dataset: Provided housing CSV file  

### Data Validation
Canvas automatically evaluated:
- Missing values  
- Column distributions  
- Data types  
- Outliers  

---

## Key Findings from Model Build

### 1. Business Question Type  
The prediction task is **not** a classification problem.  
It is a **regression** problem because the target is a continuous numeric value.

### 2. Shape of `total_bedrooms`  
Distribution shape: **Right Skewed**

### 3. Highest Impact Feature  
Canvas identified **latitude** as the feature with the greatest impact on predicted home values.

### 4. Advanced Metrics Provided  
Canvas provides:  
- R²  
- MAE  
- RMSE  

Canvas does **not** provide:  
- Accuracy (only used for classification models)

---

## Batch Predictions

After the model was built:

- Imported the **housing_to_predict.csv** dataset  
- Generated batch predictions using the trained model  
- Exported predictions as a CSV file  
- Submitted the file as required
  ---

## Tools & Technologies

- Amazon SageMaker Canvas  
- Machine Learning (Regression)  
- Cloud-based model training  
- Batch inference  
- CSV data processing  

---

## Skills Demonstrated

- No‑code ML model creation  
- Data validation and distribution analysis  
- Feature impact interpretation  
- Regression model evaluation  
- Batch prediction generation  
- AWS resource management  

---

## Summary

This assignment provided hands-on experience using SageMaker Canvas to build, evaluate, and deploy a machine learning model. By predicting home values and generating batch outputs, this project demonstrates practical ML workflow skills applicable to real-world business analytics and data science tasks.
