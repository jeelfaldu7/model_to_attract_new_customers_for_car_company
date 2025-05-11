# 🚗 Car Price Prediction Model – Rusty Bargain
Rusty Bargain, a used car sales service, is developing an app to attract new customers. So, for this the project is to build a model to predict the market value of vehicles based on historical data including technical specifications, trim versions, and pricing information. 

## 🧠 Project Description
Rusty Bargain is developing an app to attract new customers by offering a feature that estimates a car's market value instantly. This project aims to build a regression model that predicts car prices with:
   - the quality of the prediction (low RMSE)
   - the speed of the prediction ( fast speed)
   - the time required for training (efficient training time)

## 📊 Features
  - Cleaned and preprocessed real-world used car dataset
  - Multiple regression models evaluated:
      - Linear Regression (baseline sanity check)
      - Decision Tree Regressor
      - Random Forest Regressor
      - CatBoost Regressor
      - LightGBM Regressor
 - Hyperparameter tuning for tree-based models
 - Performance metrics: RMSE, training time, and prediction time
 - Categorical feature encoding for compatibility with specific models
 - Final model selection based on validation RMSE and execution efficiency

## 📁 Table of Contents
  - Project Description
  - Features
  - Run this project
  - Usage
  - Model Evaluation
  - Tools and Libraries Used
  - Credits

## 🛠️ Run this project
  - Clone the repository
      ```bash
      git clone https://github.com/yourusername/rusty-bargain-price-prediction.git
  - Install dependencies
      ```bash
      pip install -r requirements.txt

## 🚀 Usage
  1. Run the Jupyter Notebook:
     ```bash
     notebook.ipynb
  2. Explore the notebook to:
     - Clean and preprocess the data
     - Train multiple models
     - Compare RMSE and training times
     - Choose the best-performing model
  3. Evaluate model predictions using the test set RMSE.

## ✅ Model Evaluation 
| Model             | RMSE (Validation) | Training Time | Notes                       |
| ----------------- | ----------------: | ------------: | --------------------------- |
| Linear Regression |            \~3815 |     Very fast | Sanity check                |
| Decision Tree     |            \~2534 |          \~1s | Moderate improvement        |
| Random Forest     |          **2018** |  1 min 17 sec | ✅ Best RMSE, selected model |
| LightGBM          |              2053 |       3.2 sec | Fastest complex model       |
| CatBoost          |              2028 |      2.33 sec | Competitive RMSE, very fast |

  - Test RMSE for Random Forest Regressor (best model): 2039.59
  - The Random Forest Regressor was selected due to its best validation RMSE and generalization ability (minimal overfitting).
  - The model's average prediction error is approximately €2040, which is acceptable for business use.

## ⚙️ Tools and Libraries Used
  - Python (Pandas, NumPy, Scikit-learn)
  - LightGBM
  - CatBoost
  - Matplotlib / Seaborn for visualization
  - Jupyter Notebook

## 🤝 Credits
This project was created as part of the TripleTen Data Science program. Special thanks to:
  - TripleTen instructors and peers for ongoing support and feedback. 

