# 🏠 Nairobi Housing Market Analysis  

## 📌 Project Overview  
This project explores rental housing data from Nairobi using two datasets that were merged and cleaned. The aim is to understand the key factors influencing house prices and uncover patterns in location, size, and room composition.  

We practice end-to-end **data science workflow**:  
- Data collection & preparation  
- Cleaning & transformation  
- Exploratory data analysis (EDA)  
- Visualizations & relationships  
- Insights & interpretations  

---

## 📂 Data Sources  
I worked with two datasets:  

1. **nairobi_apt.csv**  
   - `Price`, `PropertyType`, `Location`, `Bedrooms`, `Bathrooms`, `House Size`, `Land Size`  

2. **nairobi_listings.csv**  
   - `Agency`, `Neighborhood`, `Price`, `Link`, `sq_mtrs`, `Bedrooms`, `Bathrooms`  

Both were cleaned, harmonized, and concatenated into a single processed dataset.  

---

## 🔧 Data Cleaning Steps  
1. Selected relevant features:  
   -`location`,`price_usd`, `bedrooms`, `bathrooms`, `area_m2`  
2. Standardized column names (e.g., `bathroom` → `Bathrooms`).  
3. Cleaned `Neighborhood` field:  
   - Split into `Road`, `Location`, `Area`.  
   - Normalized multiple delimiters and spacing.  
4. Created a consistent `Location` column (standardized to: **Kileleshwa, Lavington, Kilimani, Westlands**).  
5. Concatenated both datasets and stored in `processed/clean_nairobi.csv`.  

---

## 🎯 Research Questions  
1. What is the relationship between house price and house size (per m²)?  
2. How do bedrooms and bathrooms impact pricing?  
3. Which locations are the most expensive on average?  
4. Are there clear differences in pricing between Nairobi’s key neighborhoods?  
5. How strongly are price, size, bedrooms, and bathrooms correlated?  

---

## 📊 Exploratory Data Analysis (EDA)  
We carried out:  
- **Summary statistics** of all features.  
- **Correlation analysis** (heatmaps, pairplots).  
- **Scatter plots** of Price vs Size.  
- **Boxplots** of Price across Locations.  
- **Crosstabs** of Location vs Area.  

---

## 🔎 Key Insights (so far)  
- Larger houses generally correlate with higher prices, but not always linearly.  
- Locations like **Westlands and Lavington** show higher median prices than **Kilimani**.  
- Adding more bedrooms/bathrooms increases price, but the effect size varies by location.  

---

## 🚀 Next Steps  
- Build predictive models (Linear Regression, Decision Trees) for Price.  
- Test how much location vs house size drives rent predictions.  
- Create interactive visualizations (maybe with Streamlit).  

---

👉 This project was executed in **VS Code Jupyter Notebooks (`.ipynb`)**, following reproducible step-by-step workflows.  
