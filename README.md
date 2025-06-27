# Condition-Based Maintenance Plus (CBM+) Analytics Project

## Overview

This Jupyter notebook demonstrates technical competence in applying data analysis and predictive modeling techniques for Condition-Based Maintenance Plus (CBM+) scenarios. Leveraging NASA’s publicly available C-MAPSS (Commercial Modular Aero-Propulsion System Simulation) turbofan engine degradation dataset, the notebook explores statistical analyses, predictive modeling, and visualization methods suitable for CBM+ applications.

---

## Data Source

The dataset utilized is the C-MAPSS turbofan engine degradation simulation dataset from NASA, specifically scenario FD001. It includes:
- Sensor measurements capturing operational settings and engine conditions.
- Engine run-to-failure cycles for training robust predictive models.

---

## Key Analyses and Methods

### Data Exploration and Visualization
- Comprehensive initial exploration of sensor data.
- Visualizations of sensor evolution over the lifecycle of engines, providing immediate insight into degradation patterns.

### Statistical Modeling
- **Weibull and Gamma Distribution Fitting:**
  - Determined optimal statistical distributions for failure prediction.
  - Evaluated models based on log-likelihood and Akaike Information Criterion (AIC).
- **Non-Homogeneous Poisson Process (NHPP):**
  - Multi-year maintenance forecasting to assist budgetary and spare inventory decisions.

### Predictive Modeling
- Machine learning approaches evaluated include:
  - **Support Vector Machine (SVM)**
  - **Random Forest**
  - **LSTM (Long Short-Term Memory networks)**
  - **k-Nearest Neighbors (kNN)**
  - **XGBoost**
  - **Tiny GPT**
  - **1D Convolutional Neural Network (CNN-1D)**
- Evaluation metrics include R-squared (R²), Root Mean Square Error (RMSE), and computational time for training and predictions.
- Selected **SVM** model for superior accuracy in Remaining Useful Life (RUL) predictions.

### Practical Applications Demonstrated
- **Short-Term Maintenance Planning:**
  - Calculated expected number of engine removals within operational cycles, aiding short-term maintenance resource allocation.
- **Spare Inventory Optimization:**
  - Provided spare engine quantity recommendations based on calculated probabilities of fleet-wide engine failure.
- **Budget and Resource Forecasting:**
  - Leveraged NHPP to project maintenance requirements over multiple years.

---

## Technical Stack
- **Python** with libraries:
  - Pandas
  - NumPy
  - Matplotlib
  - SciPy
  - TensorFlow/Keras
  - Scikit-learn
  - XGBoost

---

## Intended Audience
This notebook serves as a showcase of analytical and predictive modeling capabilities relevant to teams involved in CBM+ analytics, specifically:
- Maintenance engineers and planners
- Reliability and logistics analysts
- Technical stakeholders involved in predictive maintenance programs

---

## Conclusion
This project highlights the practical application of advanced analytics and machine learning methods to real-world predictive maintenance scenarios. It demonstrates both statistical rigor and operational utility, aligning closely with industry best practices for CBM+ solutions.

