# California Housing Price Analysis 🏡📊
A data analysis and regression modeling project to predict housing prices in California based on various demographic and geographical factors.

# Features
+ **Data Exploration:** Provides insights into the dataset, including distributions and relationships among features.
+ **Feature Importance:** Identifies significant predictors of housing prices.
+ **Validation and Testing:** Evaluates the model performance on both validation and test datasets using metrics like MAE, MSE, and RMSE.
+ **Result Visualization:** Presents findings using data visualizations and model coefficients.
# Dataset
The project uses the California Housing Dataset from sklearn.datasets with 20,640 samples and 9 features. Key features include:

+ **MedInc:** Median income in the area.
+ **HouseAge:** Median age of the houses.
+ **AveRooms:** Average number of rooms per household.
+ **AveBedrms:** Average number of bedrooms per household.
+ **Population:** Total population in the area.
+ **Latitude and Longitude:** Geographical location.
+ **Target:** Median house price.

# Workflow
+ **Data Preprocessing:**

  + Checked for null values and ensured data completeness.
  + Normalized features to improve model performance.

+ **Exploratory Data Analysis (EDA):**

  Explored the relationship between features and the target variable.
  Visualized data distributions and trends.

+ **Modeling:**

     Trained a regression model and evaluated its performance on:

    **Validation Dataset:**

        Mean Absolute Error (MAE): 0.5350
        Mean Squared Error (MSE): 0.5363
        Root Mean Squared Error (RMSE): 0.7323
    **Test Dataset:**

        Mean Absolute Error (MAE): 0.5345
        Mean Squared Error (MSE): 0.5322
        Root Mean Squared Error (RMSE): 0.7295

+ **Feature coefficients indicate that:**
  
    **MedInc:** Most positively correlated with housing prices. 

    **AveBedrms:** Significant positive correlation.

    **Latitude and Longitude:** Show negative correlations.

                  Coefficients
                    MedInc          0.431340
                    HouseAge        0.009655
                    AveRooms       -0.096560
                    AveBedrms       0.558126
                    Population     -0.000009
                    AveOccup       -0.002955
                    Latitude       -0.418625
                    Longitude      -0.429426

# Results & Evaluation:

The model achieved similar performance on both validation and test datasets, with slightly better results on the test dataset (lower RMSE of 0.7295).
Key predictors: MedInc, AveBedrms, and HouseAge.

# Conclusions Drawn
+ **Income Impact:** Higher median income (MedInc) is the most significant predictor of housing prices.

+ **Geographic Trends:** Prices decrease as we move to higher latitudes and longitudes, indicating regional variations.

+ **Model Reliability:** Consistent performance on validation and test datasets demonstrates the model's robustness.

+ **Future Scope:** Include additional features (e.g., economic indicators, neighborhood ratings).Experiment with advanced regression models or neural networks for improved accuracy.
