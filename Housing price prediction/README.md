# 🏠Housing Rent Category Prediction
---


## 📌 Problem Statement
The goal of this project is to build a machine learning model that predicts the rent category of a house (Low / Medium / High) based on property features such as BHK, size, city, furnishing status, and tenant type.
This helps users, tenants, and rental companies make better rental pricing decisions.

---
## 🧱 Tech Stack

- 🐍 **Python**
- 📓 **Jupyter Notebook**
- 📊 **Pandas, NumPy** – data manipulation
- 📈 **Matplotlib, Seaborn** – visualisation
- 🤖 **Scikit-learn, XGBoost** – machine learning models & evaluation

All implementation details (code, plots, experiments) are inside the `.ipynb` notebook.

---
## 📂 Data Description

BHK	:Number of Bedrooms	Numeric

Size :	House size (sq. ft)	Numeric

City	:City Name	Categorical

Furnishing Status	:Furnished / Semi-Furnished / Unfurnished	Categorical

Tenant Type:	Family / Bachelors / Company	Categorical

Rent Category	:Low / Medium / High	Target Variable (Categorical)

### 1️⃣ Data Cleaning & Preparation

Checked and handled missing values

Removed duplicate entries

Encoded categorical variables using Label Encoding / One-Hot Encoding

Scaled numeric values using StandardScaler

Converted Rent column into categories (Low / Medium / High)

---
### 2️⃣Exploratory Data Analysis (EDA)

Distribution of rent categories

Impact of BHK on rent category

Boxplot: Size vs Category

City-wise rent segmentation

Furnishing status vs category

Tenant type analysis

---
### 3️⃣ Feature Engineering

Created price_per_sqft = Rent / Size (if required)

Binning rent into Low / Medium / High

Converted categorical to numeric

Feature selection using correlation and Chi-Square

---
### Model Building

Model Used: Multi-Class Logistic Regression

---
### Model Evaluation

Accuracy Score	: How correctly model predicts rent category

Confusion Matrix : Shows actual vs predicted

### Results & Key Insights

📌 Multi-Class Logistic Regression achieved good accuracy
📌 Furnishing status and City are strong predictors of rent category
📌 Bigger houses (higher sq ft) fall in medium & high categories
📌 Bachelors prefer 1–2 BHK more while families prefer 2–3 BHK
