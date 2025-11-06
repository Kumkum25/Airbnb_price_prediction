# 🏠 Airbnb (Air Bed & Breakfast) Price Prediction

## 📖 Overview
This project focuses on predicting the **price of Airbnb listings** using **machine learning techniques**.  
**Airbnb (Air Bed & Breakfast)** is an online platform that allows individuals to rent out homes, apartments, or rooms to travelers.  
The aim is to analyze how different features — such as property type, location, amenities, and host attributes — influence listing prices and to build a predictive model for accurate price estimation.

---

## 🎯 Objective
To develop and evaluate machine learning models that predict the **log-transformed Airbnb price (`log_price`)** based on property, host, and review features.

---

## 📊 Dataset Information
The dataset contains **74,111 entries** and **29 columns**, describing listings from multiple cities.

| Feature | Description |
|----------|-------------|
| `id` | Unique listing identifier |
| `log_price` | Log-transformed price of the Airbnb listing *(target variable)* |
| `property_type` | Type of property (e.g., Apartment, House, Villa) |
| `room_type` | Type of room (Entire home, Private room, Shared room) |
| `amenities` | List of facilities available in the property |
| `accommodates` | Number of guests that can be accommodated |
| `bathrooms`, `bedrooms`, `beds` | Property size and sleeping arrangements |
| `bed_type` | Type of bed provided |
| `cancellation_policy` | Type of cancellation policy applied |
| `cleaning_fee` | Whether a cleaning fee is charged |
| `city`, `neighbourhood`, `zipcode` | Location details |
| `description`, `name`, `thumbnail_url` | Text and image-related data |
| `first_review`, `last_review` | Dates of first and last guest reviews |
| `host_since` | Date when the host joined Airbnb |
| `host_response_rate` | Host’s response rate to messages |
| `host_identity_verified` | Whether the host’s identity is verified |
| `host_has_profile_pic` | Whether the host has a profile picture |
| `instant_bookable` | Whether the listing can be booked instantly |
| `number_of_reviews` | Total number of reviews received |
| `review_scores_rating` | Average guest rating |
| `latitude`, `longitude` | Geographic coordinates of the listing |

---

## ⚙️ Data Preprocessing & Feature Engineering
- Handled **missing values** and ensured data consistency  
- Extracted numeric features from text columns like `amenities`  
- Calculated **host experience duration** using `host_since`  
- Applied **log transformation** on prices for normalization  
- Encoded categorical variables using One-Hot and Label Encoding  
- Scaled numerical features where necessary  

---

## 🔍 Exploratory Data Analysis (EDA)
- Visualized **price distributions** and feature correlations  
- Analyzed **room types, property types, and cities** with highest prices  
- Checked **review trends** and **rating distributions**  
- Detected and capped **outliers** for model stability  

---

## 🤖 Model Development
Implemented and compared multiple regression models:
- **Linear Regression**
- **Random Forest Regressor**
- **Gradient Boosting Regressor**
- **XGBoost Regressor**
- **CatBoost Regressor**

---

## 📈 Model Evaluation
Evaluated models using:
- **R² Score (Coefficient of Determination)**  
- **Mean Absolute Error (MAE)**  
- **Root Mean Squared Error (RMSE)**  

✅ Selected the best-performing model based on accuracy and generalization.

---

## 🧠 Key Insights
- **Location (latitude & longitude)** strongly influences prices  
- Listings with **more amenities** and **higher ratings** are priced higher  
- **Host experience** and **number of reviews** impact credibility and pricing  
- **Entire home/apartment** listings are generally more expensive than private rooms  

---

## 🧰 Tools & Technologies Used
- **Python**
- **Pandas**, **NumPy**
- **Matplotlib**, **Seaborn**
- **Scikit-learn**
- **XGBoost**, **CatBoost**
- **Jupyter Notebook**

---


