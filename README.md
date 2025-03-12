# SzegedWeather-RegressionAnalysis

![Weather Data Analysis](https://img.shields.io/badge/Data%20Analysis-Weather-blue)
![Python](https://img.shields.io/badge/Python-3.7%2B-green)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-Machine%20Learning-orange)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

## 🌦️ Project Overview

This project analyzes weather data from the city of Szeged, Hungary, using machine learning models to predict **Apparent Temperature** based on various meteorological features. The analysis includes comprehensive data exploration, preprocessing, feature engineering, and model training.

## 📊 Dataset

The dataset (`weatherHistory.csv`) contains historical weather data with the following features:
- Formatted Date
- Summary (weather condition descriptions)
- Precip Type
- Temperature (C)
- Apparent Temperature (C)
- Humidity
- Wind Speed (km/h)
- Wind Bearing (degrees)
- Visibility (km)
- Loud Cover
- Pressure (millibars)
- Daily Summary

## 🔍 Data Preprocessing

The preprocessing pipeline includes:
- Outlier detection and handling
- Feature scaling (standardization and min-max scaling)
- Label encoding for categorical variables
- Feature selection

## 🤖 Model Training & Evaluation

We trained and compared several regression models to predict Apparent Temperature:

| Model | R² | Mean Squared Error |
|-------|------|------|
| **Random Forest** | 1.0000 | 0.0000 |
| **Decision Tree** | 0.9999 | 0.0001 |
| **Gradient Boosting** | 0.9996 | 0.0004 |
| **SVR** | 0.9942 | 0.0057 |
| **Linear Regression** | 0.9900 | 0.0100 |
| **Ridge Regression** | 0.9900 | 0.0100 |

### Key Insights:
- The Random Forest Regressor achieved perfect prediction capabilities with an R² of 1.0000
- Tree-based and ensemble methods significantly outperformed linear models
- All models demonstrated high accuracy, indicating strong relationships between weather features and apparent temperature

## 🌟 Results Highlights

- **Random Forest** emerged as the superior model with near-perfect prediction accuracy
- Weather conditions in Szeged demonstrate strong predictable patterns
- Temperature, humidity, and wind speed were identified as the most influential features
- The analysis revealed complex non-linear relationships between meteorological variables

## 📚 Repository Structure

```
SzegedWeather-RegressionAnalysis/
│
├── dataset/
│   └── weatherHistory.csv      # Historical weather data
└── LICENSE              # License for this project
└── README.md              # Documentation for this project
└── tugas_1.ipynb              # Jupyter notebook with analysis and models
```

## 🚀 Getting Started

### Prerequisites
- Python 3.7+
- Jupyter Notebook
- Required libraries: pandas, numpy, scikit-learn, matplotlib, seaborn

### Installation & Running
1. Clone this repository
2. Install required dependencies:
   ```
   pip install pandas numpy scikit-learn matplotlib seaborn
   ```
3. Open and run the Jupyter notebook:
   ```
   jupyter notebook tugas_1.ipynb
   ```

## 📋 Methodology

1. **Data Exploration**: Analyzed distributions, correlations, and patterns in the weather data
2. **Data Preprocessing**: Handled outliers, encoded categorical features, and applied appropriate scaling
3. **Feature Engineering**: Created relevant features to improve model performance
4. **Model Training**: Trained multiple regression models with different algorithms
5. **Performance Evaluation**: Compared models using R² and Mean Squared Error metrics
6. **Model Interpretation**: Analyzed feature importance and model behavior

## 📈 Future Work

- Implement time series analysis for temporal patterns in weather data
- Explore deep learning approaches for weather prediction
- Incorporate additional external data sources to improve predictions
- Deploy an interactive dashboard for real-time predictions

## 📝 License

This project is available under the MIT License - see the LICENSE file for details.