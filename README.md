# NYC Airbnb Price Prediction

This repository contains a comprehensive machine learning project aimed at predicting Airbnb prices in New York City. The project covers data preparation, feature engineering, model training, evaluation, and optimization. By combining traditional statistical methods with modern AutoML techniques, the final model is both accurate and interpretable—ready for real-world deployment.

---

## Project Overview

This project follows a systematic process to develop a robust price prediction model:

### **Data Preparation and Feature Engineering**

1. **Outlier Detection & Handling**  
   - Detected and managed outliers using visualizations (box plots, scatter plots) and the IQR method.
   - Improved data quality by reducing the impact of extreme values.

2. **Feature Encoding**  
   - Applied **label encoding** and **one-hot encoding** to convert categorical variables into numerical formats, ensuring compatibility with machine learning algorithms.

### **Feature Selection**

3. **Correlation Matrix Analysis**  
   - Analyzed feature correlations to identify multicollinearity and redundancy.
4. **Recursive Feature Elimination (RFE)**  
   - Ranked and selected the most relevant features, reducing noise and focusing the model on key predictors.

### **Model Training and Evaluation**

5. **Initial Model Training**  
   - Compared multiple models including **Linear Regression**, **Random Forest**, and **Gradient Boosting Regressor**.
   - Evaluated model performance using RMSE and R-squared metrics.

6. **SHAP Analysis**  
   - Used SHAP values to interpret individual models and understand feature importance.

### **Model Selection and Optimization**

7. **Tree-Based Model Interpretation**  
   - Employed Random Forest and Gradient Boosting to interpret decision paths and feature splits.
8. **AutoML for Best Model Selection**  
   - Automated model selection, which identified a **Stacked Ensemble** as the best performer.
9. **SHAP Analysis on the Stacked Ensemble**  
   - Confirmed feature impacts and maintained interpretability on the final model.

### **Hyperparameter Tuning and Regularization**

10. **Hyperparameter Tuning**  
    - Fine-tuned key parameters (e.g., learning rate, maximum depth) to optimize accuracy and generalization.
11. **Regularization (Ridge/Lasso)**  
    - Applied regularization techniques to control model complexity, prevent overfitting, and stabilize predictions.

### **Final Steps**

12. **Final Evaluation**  
    - Assessed the final model on a test set to ensure robust generalization performance.
13. **Model Saving and Documentation**  
    - Saved the final model and preprocessing steps for future use and provided detailed documentation for transparency and reproducibility.

---

## Dataset Details

The dataset used for this project consists of historical Airbnb listings and price data in New York City. It includes features such as:
- Listing details (e.g., location, number of reviews, room type)
- Pricing information
- Host details
- Calendar availability

By cleaning and engineering features from this dataset, the project aims to capture the key drivers behind Airbnb pricing, which can then be leveraged for improved investment and operational decision-making.

---

## Why This Project is Useful

- **Informed Decision-Making:**  
  The model provides accurate predictions, enabling hosts and investors to understand pricing dynamics and optimize their strategies.

- **Time Efficiency:**  
  Automates the data analysis process that would otherwise take hours of manual research.

- **Transparency and Interpretability:**  
  Through the use of SHAP and model interpretation techniques, the model’s predictions can be understood in terms of key features—helping stakeholders trust and verify the results.

- **Scalability:**  
  The techniques used in this project can be adapted to other cities or types of property rental predictions, making it a versatile tool for real estate analytics.

---

## Installation Guide

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/yourusername/nyc-airbnb-price-prediction.git
   cd nyc-airbnb-price-prediction
