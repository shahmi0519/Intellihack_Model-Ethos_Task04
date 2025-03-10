
# Stock Price Prediction using Machine Learning

## Overview
This project aims to predict stock prices 5 trading days into the future using machine learning techniques. The solution demonstrates predictive accuracy and practical trading value through exploratory data analysis (EDA), feature engineering, model training, and performance evaluation. The workflow is designed to provide actionable insights for traders and investors.

---

## Table of Contents
- [Problem Statement](#problem-statement)
- [Features](#features)
- [Models](#models)
- [Results](#results)
- [Installation](#installation)
- [Usage](#usage)
- [Dataset](#dataset)
- [Future Improvements](#future-improvements)
- [License](#license)
- [Contributing](#contributing)
- [Contact](#contact)

---

## Problem Statement
Stock price prediction is critical for informed trading decisions but remains challenging due to market volatility and complex temporal dependencies. This project addresses these challenges by:
- Identifying key patterns in historical stock data.
- Engineering relevant features to capture trends and volatility.
- Building a robust machine learning model for accurate predictions.

---

## Features
### Engineered Features
- **Lag Features**: `Close_Lag_1`, `Close_Lag_5`, `Close_Lag_10` (past closing prices).
- **Volatility**: `Volatility_5` (standard deviation of closing prices over 5 days).
- **Momentum**: `Momentum_5` (difference between current and past closing prices).
- **Moving Averages**: `SMA_5`, `SMA_20` (5-day and 20-day simple moving averages).
- **Target Variable**: `Target` (closing price 5 days ahead).

---

## Models
- **Algorithms Tested**:
  - Linear Regression
  - Random Forest Regressor
  - Support Vector Regressor (SVR)
  - K-Nearest Neighbors Regressor (KNN)
- **Best Model**: K-Nearest Neighbors Regressor (KNN) achieved the highest **R² score of 0.9892**.

---

## Results
### Performance Metrics
- **RMSE**: 3.4147878464047645
- **MAE**: 1.7928729851183673
- **R² Score**: 0.9955236784278279

### Visualizations
- **Figure 1**: Stock Closing Price Over Time 
- **Figure 2**: Stock Price with Moving Averages  
- **Figure 3**: Model Accuracy Comparison (Learning Curves)  
- **Figure 4**: Actual vs Predicted Closing Prices  
- **Figure 5**: Residual Error Distribution  
- **Figure 6**: Correlation Matrix Heatmap  
- **Figure 7**: Permutation Importance for KNN Model  

---

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/shahmi0519/Intellihack_Model-Ethos_Task04/tree/main
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
   **requirements.txt**:
   ```
   pandas
   numpy
   matplotlib
   seaborn
   scikit-learn
   joblib
   jupyter
   ```

---

## Usage
1. Run the Jupyter Notebook:
   ```bash
   jupyter notebook stock_price_prediction.ipynb
   ```
2. **Data Preprocessing**:
   - Load and clean the dataset (`question4-stock-data.csv`).
   - Handle missing values and normalize features.
3. **Model Training**:
   - Execute cells under "Model Training" to train and compare models.
4. **Predictions**:
   - Provide a CSV file with the last 10 days of data to generate predictions for the next 5 days.

---

## Dataset
- **Source**: `question4-stock-data.csv` (historical stock data with columns: `Date`, `Open`, `High`, `Low`, `Close`, `Volume`).
- **Preprocessing**: Missing values handled via forward-fill; lag features and indicators engineered.

---

## Future Improvements
- Incorporate external data (news sentiment, economic indicators).
- Experiment with LSTM/GRU for time series forecasting.
- Optimize hyperparameters for KNN.
- Enhance feature engineering with technical indicators (RSI, MACD).

---

## Contributing
Contributions are welcome!  
1. Fork the repository.  
2. Create a feature branch: `git checkout -b feature/new-feature`.  
3. Commit changes: `git commit -m 'Add new feature'`.  
4. Push to the branch: `git push origin feature/new-feature`.  
5. Open a pull request.

---

## Contact
For questions or feedback, contact:  
-  
- **GitHub**: shahmi0519(https://github.com/shahmi0519)
``` 

This README follows industry standards with clear sections for technical and non-technical audiences. Adjust placeholders (e.g., `[Insert RMSE value]`) with actual results from your analysis.
