# 🏙️ Pakistan’s Top Cities — Property Price Prediction

This repository focuses on **predicting real estate prices** across Pakistan’s top cities — **Karachi, Lahore, and Islamabad** — using machine learning.  
We cleaned, analyzed, and modeled property data to estimate fair market prices based on several important features such as **area (sq. ft.)**, **bedrooms**, **bathrooms**, and **location**.

---

## 📘 Project Overview

Property prices in Pakistan’s major cities vary widely due to location, property type, and amenities.  
The goal of this project is to develop **predictive models** that can estimate the price of a property based on its attributes.  

Each city has its own dedicated notebook, which includes:
- **Data Cleaning**
- **Outlier Removal**
- **Exploratory Data Analysis (EDA)**
- **Feature Engineering**
- **Model Training and Evaluation**

A new feature — **`Price Per Sqft`** — was added to improve dimensionality reduction and better capture property value relative to size.

---

## 🧹 Data Preprocessing

Before modeling, extensive preprocessing was carried out to ensure data quality and accuracy:

1. **Handled Missing Values:**  
   Missing or null entries were filled using statistical imputation or dropped if irrelevant.

2. **Outlier Detection and Removal:**  
   Extreme values were identified using visualizations and IQR-based filtering, which helped improve model stability.

3. **Feature Standardization:**  
   Standardized property size (square feet) and normalized numerical attributes.

4. **Feature Engineering:**  
   Created a new feature called **`price_per_sqft = price / area_sqft`**, helping capture value density and reduce variance caused by large properties.

5. **Categorical Encoding:**  
   Converted categorical attributes (like `place/area`) into numerical form for modeling.

---

## 🔍 Exploratory Data Analysis (EDA)

EDA was conducted to understand trends, relationships, and patterns in the dataset.

Key insights:
- **Property prices** show strong correlation with **area** and **number of bedrooms**.
- **Price per Sqft** helps normalize differences between small and large properties.
- **Location** is the most significant feature — prices in central or popular areas are consistently higher.
- Visualizations include **boxplots**, **heatmaps**, **distribution plots**, and **correlation matrices** for clear insights.

---

## 🧠 Model Building

After data cleaning and feature engineering, several regression models were explored for each city.  
City-wise models were trained independently to account for local market differences.

**Algorithms Used:**
- Linear Regression (Baseline)
- Random Forest Regressor
- Gradient Boosted Regressors (XGBoost / LightGBM)

**Evaluation Metrics:**
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

Each city’s notebook (`.ipynb`) contains:
- Model comparison
- Hyperparameter tuning
- Performance metrics
- Final trained model for predictions

---


🤝 Contributing
Contributions are welcome!
If you’d like to improve the project or add more datasets, feel free to:

Fork the repository

Create a new branch

Make your changes

Submit a pull request


📝 License
This project is open-source and available for educational and research purposes.
You may reuse or modify it with proper credit to the author.




