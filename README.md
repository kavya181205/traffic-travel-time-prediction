# 🚗 AI-Based Traffic Travel Time Prediction

## Overview
This project predicts travel time for urban trips using machine learning. The model analyzes factors such as distance, traffic density, weather conditions, time of day, and route locations to estimate accurate travel duration. The system can be useful for smart city traffic management, route planning, and congestion analysis.

---

## Problem Statement
Urban traffic congestion leads to increased travel time and inefficiency. Accurate prediction of travel time can help in:
- Better route planning
- Traffic management
- Smart city transportation systems
- Reducing delays and fuel consumption

---

## Dataset
The dataset contains trip-level information including:
- Start Area
- End Area
- Distance (km)
- Average Speed (km/h)
- Traffic Density Level
- Time of Day
- Day Type (Weekday/Weekend)
- Weather Condition
- Road Type
- Travel Time (Target)

---

## Feature Engineering
The following features were created:
- **Traffic density encoding**
- **Peak hour indicator (is_peak)**
- **Weekend indicator (is_weekend)**
- **Weather risk levels**
- **Road type encoding**
- **One-hot encoding for start and end locations**
- Removed redundant features after correlation analysis

---

## Models Used
- Random Forest Regressor
- XGBoost Regressor

Hyperparameter tuning was performed using GridSearchCV.

---

## Model Performance

### XGBoost (Final Model)
- **MAE:** ~1.9 minutes  
- **R² Score:** ~0.989  

The model shows strong generalization and accurate prediction across different traffic conditions.

---

## Evaluation

### Key Visualizations
- Correlation Matrix
- Actual vs Predicted Plot
- Residual Analysis
- Feature Importance

These analyses confirm that the model captures real-world traffic patterns effectively.

---

## Important Insights
- Distance and average speed are the most influential factors.
- Traffic density and peak hours significantly affect travel time.
- Location-based features help capture area-specific congestion patterns.
- Model performance remains high even without derived baseline features.

---

## Project Structure
