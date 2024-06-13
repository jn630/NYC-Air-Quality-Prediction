# NYC-Air-Quality-Prediction

## Objective

This project aims to compare the performance of two models, XGBoost and Prophet, in predicting AQI (Air Quality Index). Here is the data.

## Metrics Used

- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- Mean Absolute Error (MAE)
- Mean Absolute Percentage Error (MAPE)
- Additional metrics for Prophet: Median Absolute Percentage Error (MDAPE), Symmetric Mean Absolute Percentage Error (SMAPE), and Coverage.

## XGBoost Results

- **MSE**: 379.26
- **RMSE**: 19.48 (calculated as sqrt(379.26))
- **MAE**: 15.15
- **MAPE**: 31.39%

## Prophet Results

Averaged over different horizons:

- **MSE**: Average of [318.48, 316.81, 318.45, 323.58, 324.09] = 320.28
- **RMSE**: Average of [17.85, 17.80, 17.85, 17.99, 18.00] = 17.90
- **MAE**: Average of [12.99, 12.96, 13.02, 13.09, 13.13] = 13.04
- **MAPE**: Average of [24.05%, 23.96%, 24.05%, 24.16%, 24.34%] = 24.11%

Additional Prophet Metrics:

- **MDAPE**: 19.68%
- **SMAPE**: 22.92%
- **Coverage**: 89.36%

## Comparative Analysis

- **MSE** and **RMSE**: Prophet has lower values, indicating it makes smaller errors on average.
- **MAE**: Prophet shows lower values, suggesting its predictions are closer to the actual values on average.
- **MAPE**: Prophet has a significantly lower percentage error, indicating better relative accuracy.

## Conclusion

Based on the analysis:
- The Prophet model outperforms the XGBoost model in predicting AQI, as indicated by lower MSE, RMSE, MAE, and MAPE values.
- Additional metrics for Prophet, such as MDAPE, SMAPE, and coverage, further support its reliability and accuracy.
- The composite score approach suggests that Prophet has higher prediction power, with performance approximately 15.2% better than XGBoost.
