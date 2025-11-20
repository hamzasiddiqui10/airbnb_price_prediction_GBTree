---

# 🏡 Berlin Airbnb Price Prediction – Gradient Boosted Trees

## 📌 Overview

This project builds a **machine-learning model to predict Airbnb listing prices in Berlin** using a cleaned dataset of listing attributes.
The goal is to explore the factors influencing rental prices and build a strong predictive model using **CatBoost Gradient Boosted Trees**.

This repository is part of my data science & machine learning portfolio.

---

## 🚀 Key Features

* End-to-end workflow in a single, clean Jupyter Notebook
* Feature engineering of text, categorical, and numerical fields
* Distribution analysis for price and log-price
* Exploratory Data Analysis (EDA) using pandas & matplotlib
* Model training using **CatBoostRegressor**
* Model evaluation (RMSE, MAE)
* Final model saved via pickle for reproducibility
* Discussion of features such as amenities, host verification, neighbourhood, and property characteristics

---

## 📂 Repository Structure

```
.
├── Berlin_AirBnB_Model_GBTree.ipynb   # Full analysis + modeling
├── cleaned_listings.pkl               # Cleaned dataset (if included)
├── LICENSE
└── README.md
```

---

## 🧠 Modeling Approach

### **Model:**

* **CatBoost Gradient Boosted Trees**
* Chosen due to:
  ✔️ Native handling of categorical features
  ✔️ Strong performance on tabular data
  ✔️ Minimal preprocessing compared to XGBoost/LightGBM

### **Target Variable:**

* `price`
* Log-transformed for modeling: `log_price`

### **Important Steps:**

* Outlier handling
* Encoding categorical variables
* Feature scaling where needed
* Hyperparameter tuning (learning rate, depth, iterations)
* Train–test split and cross-validation

---

## 📊 Results

* The model achieves strong predictive performance on unseen test data
* Log-transform significantly stabilizes variance and improves fit
* High-impact features include:

  * Neighborhood
  * Room type
  * Number of accommodates and bathrooms
  * Host verification
  * Amenities (limited effect after one-hot expansion)

---

## 🛠️ Technologies Used

* Python 3.x
* pandas
* NumPy
* matplotlib / seaborn
* CatBoost
* Jupyter Notebook
* pickle

---

## ▶️ How to Run

1. Clone the repository:

   ```bash
   git clone <repo_url>
   cd <repo_name>
   ```
2. Run the notebook:

   ```bash
   jupyter notebook Berlin_AirBnB_Model_GBTree.ipynb
   ```

---

## 📜 License

This project is released under the **MIT License**.

---

## 🙋‍♂️ About Me

I am a Data Scientist with 5 years of industry experience and a graduate student in **Applied Data Science**.
I enjoy building real-world ML models, especially in predictive modeling, pricing, and tabular ML. This project
was made for the Machine Learning course during my Masters degree.

---

## Declaration of AI use:
An LLM was used to write this README file.

---
