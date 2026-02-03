# customer-lifetime-value-prediction-ml
Ensemble machine learning system that predicts customer lifetime value using RFM-based behavioral features from retail transaction data

An end-to-end machine learning project that predicts **Customer Lifetime Value (CLV)** using transactional retail data. This project applies RFM-based feature engineering and ensemble regression techniques to estimate future customer spending and support data-driven business decisions.

---

## Project Overview

Customer Lifetime Value is a critical business metric that helps organizations identify high-value customers, optimize marketing strategies, and improve revenue forecasting.

This project builds a regression pipeline that transforms raw transaction data into meaningful behavioral features and evaluates multiple ensemble models to predict customer monetary value.

### Workflow Includes:
- Data cleaning and preprocessing  
- Outlier handling using IQR  
- RFM (Recency, Frequency, Monetary) feature engineering  
- Ensemble model training  
- Model evaluation  
- Feature importance analysis  

---

## Dataset

The project uses a real-world **online retail transactional dataset** containing customer purchases.

### Key Features:
- Invoice details  
- Product information  
- Purchase quantity  
- Transaction timestamps  
- Unit prices  
- Customer identifiers  

*Dataset not included due to size.*

---

## Feature Engineering — RFM Analysis

Customers were profiled using:

- **Recency** → Days since last purchase  
- **Frequency** → Number of transactions  
- **Monetary** → Total spending  

RFM modeling is widely used in industry for customer analytics and lifetime value estimation.

---

## Models Implemented

- Random Forest (Bagging)  
- Gradient Boosting (Boosting)  
- XGBoost (Advanced Boosting)  
- Stacking Regressor (Meta-Ensemble)  

These models were selected to compare different ensemble learning strategies for regression tasks.

---

## Model Performance

| Model | MSE | R² Score |
|--------|------------|------------|
| Random Forest | 7,946,747.72 | 0.19 |
| Gradient Boosting | 15,016,718.66 | -0.52 |
| XGBoost | 9,401,050.23 | 0.05 |
| **Stacking Regressor** | **7,775,503.17** | **0.21** |

---

## Best Performing Model

**Stacking Regressor** achieved the highest predictive performance among the tested models.

> The results demonstrate how combining multiple ensemble learners can improve regression outcomes compared to individual models.

---

## Key Insight

> Predicting customer spending is inherently complex due to variability in purchasing behavior. The results highlight the challenges of real-world regression problems and emphasize the importance of feature engineering and model tuning.

*(This line makes you sound like a real data scientist.)*

---

## Feature Importance

Feature importance analysis revealed that **purchase frequency and recency** were among the strongest predictors of customer monetary value, reinforcing the effectiveness of RFM-based behavioral modeling.

---

## 🛠 Tech Stack

### Languages & Libraries
- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- XGBoost  
- Matplotlib  
- Seaborn  

---

## How to Run This Project

### Clone the repository
```bash
git clone https://github.com/YOUR-USERNAME/customer-lifetime-value-prediction-ml.git
```

### Install dependencies
```bash
pip install -r requirements.txt
```

### Add the dataset  
Place the dataset inside the project directory.

### Run the notebook
```bash
jupyter notebook
```

Open:

```
Customer_Lifetime_Value_Prediction.ipynb
```

---

## Project Highlights

✅ Built a complete regression pipeline  
✅ Applied industry-standard RFM modeling  
✅ Implemented advanced ensemble techniques  
✅ Compared multiple regression algorithms  
✅ Generated actionable customer insights  

---

## Future Improvements

- Hyperparameter tuning (GridSearchCV / RandomizedSearchCV)  
- Advanced feature engineering  
- Customer segmentation using K-Means  
- Deep learning regression models  
- Deployment for real-time value prediction  

---

## Support

If you found this project useful, consider **starring ⭐ the repository**.

---
