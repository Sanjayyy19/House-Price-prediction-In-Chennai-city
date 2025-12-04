
## 🏠 Project Overview – Step by Step

### 1. **Base Paper & Motivation**
- I started with a base paper on **warehouse rental prices** using spatial machine learning (Elsevier, 2025).  
- That inspired you to adapt the idea to **housing rent prediction**, focusing on **feature interactions**.

---

### 2. **Problem Refinement**
- Initially, I tried predicting rents across **all metro cities**.  
- Accuracy was inconsistent because rent ranges and locality impacts varied widely.  
- So I refined the scope to **Chennai city only**, for better stability and performance.

---

### 3. **Objective**
- Predict house rent prices in Chennai using ML.  
- Study **non-linear feature interactions** (e.g., area + locality, amenities).  
- Compare models (Random Forest, Gradient Boosting, LightGBM).  
- Build a **practical framework** for tenants, owners, and planners.

---

### 4. **Dataset**
- Source: Cleaned rental dataset of metro cities.  
- Records for Chennai: **8419**.  
- Features: **10 main variables** (seller type, bedrooms, layout, property type, locality, area, furnishing, bathrooms, city).  
- Target: **Monthly rent (price)**.

---

### 5. **Workflow**
1. **Data Collection** – Gathered rental data with features like size, layout, locality, amenities.  
2. **Preprocessing** – Handled missing values, removed duplicates, encoded categorical variables.  
3. **Feature Engineering** – Created new features (e.g., area per room), studied interactions (location + amenities).  
4. **Model Building** – Trained Random Forest, Gradient Boosting, LightGBM.  
5. **Model Evaluation** – Compared RMSE, MAE, R².  
6. **Interpretation** – Used **SHAP values** to explain feature importance.

---

### 6. **Models & Results**
| Model                  | MAE   | RMSE  | R² Score |
|-------------------------|-------|-------|----------|
| Random Forest           | 0.15  | 0.31  | **0.8603** |
| Gradient Boosting       | 0.17  | 0.21  | 0.8562 |
| LightGBM                | 0.10  | 0.30  | 0.8550 |

- **Random Forest** gave the best overall balance (highest R²).  
- **LightGBM** was faster but slightly less stable.  
- **Gradient Boosting** also performed well, showing non-linear feature capture.


### 7. **Insights from SHAP**
- **Area** and **locality** were the strongest predictors.  
- **Bedrooms + furnishing type** had significant interaction effects.  
- **Seller type** and **property type** influenced rent but less than size/location.  
- Non-linear combinations (e.g., large furnished flats in prime localities) drove higher rents.

### 8. **Conclusion**
- I successfully built a **city-level rent prediction model** for Chennai.  
- Random Forest was the most reliable model.  
- Feature interaction analysis improved interpretability.  
- The framework can help **tenants, owners, and planners** make informed rental decisions.



---

