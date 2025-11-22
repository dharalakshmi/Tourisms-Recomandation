# 🌍 Tourism Analytics & Intelligent Recommendation System  
### **Predictive Modeling • Sentiment Analysis • Time Series Forecasting • POI Insights**

---

## 📌 Project Summary  
This project integrates **three large tourism datasets**—Company Information, Geospatial POI Data, and Market Trends—into a unified analytical system for predicting tourist behavior, revenue patterns, visitor volumes, sentiment trends, and business performance.  
Using **Regression Models, Time Series Forecasting, NLP Sentiment Analysis, and Clustering**, the system generates actionable insights for tourism companies and provides a smart **dashboard-like analytics experience**.  
The final output helps in **revenue prediction, seasonality understanding, visitor segmentation, and tourism recommendation generation**.

---

## 🔄 Project Workflow Diagram  

Data Collection
↓
Data Preprocessing & Cleaning
↓
Merging 3 Datasets using POI_ID (5,000 × 51 matrix)
↓
Exploratory Data Analysis (EDA)
↓
Feature Engineering (Indices, Sentiment, Seasonality)
↓
ML Model Building (Regression, Time Series, NLP, Clustering)
↓
Evaluation & Interpretation
↓
Dashboard Insights & Business Recommendations



---

## 📂 Dataset Overview  

### **1️⃣ Company Information Dataset**
- Includes company name, service type, revenue, customer rating, digital share, retention, etc.  
- Columns used: Revenue, Avg_Customer_Rating, Customer_Retention, Booking Platforms.

### **2️⃣ Geospatial POI Dataset**
- Includes POI location, region type, safety index, cost, food index, connectivity index.  
- Contains 30+ **calculated indices** using formulas (Safety_Index, Seasonality_Index, Food_Index, etc.)

### **3️⃣ Market Trends Dataset**
- Reviews, sentiment, time spent, average rating, travel mode, overall experience.

### **Kaggle Datasets Used**
**TripAdvisor Tourist Attraction Reviews (20k text reviews)**  
Used for:
- Mapping `reviews_text → Reviews`
- `rating → Avg_Customer_Rating`
- Sentiment Score creation  
- Extracting keywords for Family_Friendly_Index, Safety_Index, Food_Index

---

## 🧮 Derived Features (Feature Engineering)

The project generated **35+ engineered attributes** including:

- Family_Friendly_Index  
- Seasonality_Index  
- Food_Index  
- Safety_Index  
- Visitor_Volume (computed)  
- Connectivity_Index  
- Attractiveness_Score  
- Optimal Visit Score  
- Sentiment Score (NLP model)  
- Price Affordability Score  
- Weather Score  
- Popularity Score  

Formulas include weighted scoring, normalization, Haversine distance, derived cost, etc.

---

## 🤖 Machine Learning Models Implemented

### **📌 Regression Models (10 Total)**
- Linear Regression  
- Ridge Regression  
- Lasso Regression  
- Decision Tree Regressor  
- Random Forest Regressor  
- Gradient Boosting Regressor  
- XGBoost Regressor  
- LightGBM Regressor  
- SVR  
- KNN Regression  

**Prediction Tasks:**  
✔ Revenue Prediction  
✔ Visitor Volume Prediction  

---

### **📌 Time Series Forecasting Models (4 Total)**
- ARIMA  
- SARIMA  
- Holt-Winters Exponential Smoothing  
- Prophet Forecasting  

**Outputs:**  
✔ Monthly revenue forecasting  
✔ Visitor volume forecasting  
✔ Seasonality decomposition plots  

---

### **📌 NLP Sentiment Analysis**
- Text cleaning (tokenization, stopwords, lemmatization)  
- VADER/TextBlob sentiment scoring  
- Sentiment → Sentiment Score (Market Trends dataset)  

Used to determine:  
✔ Customer satisfaction  
✔ Seasonality (peak vs off-peak sentiment)  
✔ Popular POIs  

---

### **📌 Clustering Model**
- K-Means, Elbow Method  
- Used for **POI Segmentation**  
Clusters such as:  
- High revenue, high visitor volume  
- Low cost, high family-friendly  
- High seasonality outdoor destinations  

---

🖥 UI Dashboard Screenshots

Below images are part of the Business Insights dashboard showing
revenue analytics, customer distribution, risk analysis, and key metrics.

1️⃣ Company Overview

![s1](https://github.com/user-attachments/assets/beaa3215-cadc-4d54-81ca-2a7a9dcf08c9)


2️⃣ Revenue & Customer Distribution

![s2](https://github.com/user-attachments/assets/2fc2944f-9738-4e97-b3e8-497a9448e93d)


3️⃣ Revenue Trajectory & Budget Allocation

![s3](https://github.com/user-attachments/assets/d45fe7a1-d787-4a3c-aee0-20e138184a18)


These dashboards resemble Tableau/Power BI–style interfaces,
displaying business intelligence metrics generated from the ML models.
