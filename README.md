# California Housing Prices

The housing market's complexity, especially with pricing influenced by geographic factors, makes accurate price prediction a significant challenge. This study aims to develop and enhance a predictive model tailored to the California housing market using advanced machine learning algorithms, providing valuable insights for buyers and sellers to make informed decisions.

**Technologies Used**: Random Forest - SVM - Linear Regression - Decision Tree - XGBoost

## California Housing Prices Dataset:

The California Housing Prices dataset, based on 1990 data, is featured in Aurélien Géron's book "Hands-On Machine Learning with Scikit-Learn and TensorFlow." It includes a CSV file with 10 features, such as geographic location (longitude and latitude), housing median age, total rooms, total bedrooms, and households per block. The target variable is the median house value in USD, representing the median value for households within a block.

<div align=center>
<img width="367" alt="Screenshot 2024-08-06 at 11 03 46 PM" src="https://github.com/user-attachments/assets/a30bc25c-a093-4fca-8e8b-4f39a4bb467b">
</div>

## Data Processing and Feature Engineering:

- Feature Engineering:
  
  - Created two new features: bedroom_ratio and household_rooms to mitigate high correlation between households, total_bedrooms, and total_rooms.
    
  - Removed highly correlated features to enhance model performance.
    
- Categorical Data Handling:

  - Applied One Hot Encoding to oceanProximity to represent the house's proximity to the ocean.
    
- Visualization:

  - Utilized correlation matrices to display feature relationships before and after feature engineering, illustrating the impact of these modifications.
 
![image](https://github.com/user-attachments/assets/edad2d95-4aec-4ba1-bf8b-33355bc624aa)

![image](https://github.com/user-attachments/assets/b450581f-9456-4603-81c8-b94747247710)

## Evaluation Metrics:

- Mean Absolute Error (MAE): Measures the average absolute difference between predicted and actual values, providing a straightforward assessment of prediction precision.

- Mean Squared Error (MSE): Emphasizes larger errors by squaring differences, making it sensitive to outliers and providing a weighted assessment of prediction accuracy.

- Root Mean Squared Error (RMSE): Evaluates model accuracy in the same units as the target variable (USD), making it interpretable for house value predictions.

- R-squared (R²): Assesses how well the model captures variance between variables, indicating the proportion of variance explained by the model.

- Mean Absolute Percentage Error (MAPE): Shows the percentage difference between predicted and actual values, insensitive to scale, making it useful for evaluating model performance across different datasets.

## Results and Conclusion:

The study used regression models, including Random Forest, SVM, Linear Regression, Decision Tree, and XGBoost, to predict housing prices. Each model's performance was evaluated on training and test datasets using metrics such as MAE, MSE, RMSE, MAPE, and R². Parameters were optimized for accuracy, with techniques like GridSearchCV and log transformation.

<div align=center>
<img width="402" alt="Screenshot 2024-08-06 at 11 15 12 PM" src="https://github.com/user-attachments/assets/fdcf4880-c50d-42fd-a720-bb22953ff550">
</div>

The "California Housing Prices" project aimed to predict house prices using the California housing dataset through five machine learning algorithms: Linear Regression, Random Forest, Gradient Boosting, Decision Tree, and SVM. After analyzing correlations within the dataset and applying these models, performance was evaluated using MAE, RMSE, R², and MAPE metrics. The Random Forest model demonstrated superior performance, achieving an accuracy of 82.55%.
