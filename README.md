# House Price Prediction — Linear Regression
 
This project implements a **linear regression model** to predict house prices based on square footage, number of bedrooms, and number of bathrooms.
 
> Task-01 of the Prodigy InfoTech Machine Learning Internship.
 
## 📊 Dataset
 
[House Prices - Advanced Regression Techniques](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data) (Kaggle)
 
Only `train.csv` is used. Relevant columns:
 
| Column         | Description                          |
|----------------|---------------------------------------|
| `GrLivArea`    | Above-ground living area (sq. ft.)    |
| `BedroomAbvGr` | Number of bedrooms                    |
| `FullBath`     | Number of full bathrooms              |
| `SalePrice`    | Sale price (target variable)          |
 
## ⚙️ How It Works
 
1. Load the dataset with `pandas`
2. Select the relevant features and target
3. Split data into 80% training / 20% testing
4. Train a `LinearRegression` model from `scikit-learn`
5. Evaluate using **RMSE** and **R² score**
6. Plot predicted vs. actual prices
7. Predict the price of a new, unseen house
## 📈 Results
 
- **RMSE:** ~52,975 (average prediction error in dollars)
- **R² score:** ~0.634 (the model explains ~63% of price variation)
![Prediction Plot](prediction_plot.png)
 
Blue points close to the red dashed line indicate accurate predictions. The model performs well for mid-range homes, with more variance at higher price points — expected, since location, lot size, and condition aren't included.
 
## 🛠️ Tech Stack
 
- Python
- pandas
- scikit-learn
- matplotlib
- numpy
## 🚀 How to Run
 
```bash
pip install pandas scikit-learn matplotlib numpy
python House_price_prediction.py
```
 
Make sure `train.csv` is in the same folder as the script.
 
## 🔮 Example Prediction
 
```
Predicted price for new house (1800 sqft, 3 bed, 2 bath): $XXX,XXX.XX
```
 
---
 
*Part of the Prodigy InfoTech ML Internship task series.*
