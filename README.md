# Travellers-Modelling-Competition  

## Business Problem  
CloverShield Insurance aims to optimize call center operations by predicting the number of times a policyholder is likely to call. By leveraging segmentation data, the goal is to develop a predictive model that improves resource allocation and reduces costs.  

## Dataset & Preprocessing  
- **Log Transformation**: Applied to normalize skewed features.  
- **Robust Scaler**: Used to standardize all features.  
- **One-Hot Encoding**: Implemented for categorical variables.  
- **Correlation Matrix**: Analyzed feature relationships to improve model performance.  

## Model Development  
### Initial Models  
- **LightGBM Benchmark Model**: Achieved a baseline Relative Gini Score of **0.24398**.  
- **XGBoost Model**: Improved performance with a Relative Gini Score of **0.24790**.  

### Key Findings  
- Policyholders with **higher call counts** exhibit **higher frequency** and **higher pure premium**.  
- **Top 3 Important Features** influencing call frequency:  
  - **12-month call history**  
  - **Tenure at snapshot**  
  - **Household policy count**  

## Best Model  
- **XGBoost** delivered the highest predictive performance.  

## Future Improvements  
- **Ensemble Models**: Combining multiple models for improved accuracy.  
- **Vehicle-Specific Details**: Including factors such as make, model, annual mileage, and use type.  
- **Driver Information**: Incorporating age, gender, driving experience, and history.  
- **Claims Data**: Using past claims, severity, and frequency for better predictions.  
