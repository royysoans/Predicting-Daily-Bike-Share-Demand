**Using Linear Regression Model**
- Why? Linear Regression is designed to model and predict a continuous number. Since `cnt` is a continuous number using Regression model is a good choice

- Model Evaluation Metrics:-
    R²: 0.8112069006017121(i.e 81% of the variation is explained by the model)
    MAE: 688.5329352801747(i.e model’s predictions are off by about 689 rentals)
    RMSE: 914.8831620767785(i.e error magnitude with penalty on large misses)

- I also predicted the `casual` and `registered` users seperately and then added them to get the total `cnt` prediction

- Model Evaluation Metrics:-
    Total R²: 0.8112069006017122
    Total MAE: 688.5329352801748
    Total RMSE: 914.8831620767785

After evaluating the Linear Regression model, I also explored a Decision Tree Regressor to capture potential non-linear relationships and feature interactions.

**Using Decision Tree Model**
- Why? Decision Tree Regression is a flexible, non-linear model that splits the data into smaller regions based on feature values. It’s especially useful when the relationship between features and the target (cnt) is not strictly linear. 

- Since cnt is a continuous number, Decision Tree Regressor can learn patterns by creating simple decision rules, making it a good choice for capturing hidden trends and interactions in the data.

- Model Evaluation Metrics
    R²: 0.8024639337588669
    MAE: 683.5740303378977
    RMSE: 935.8274437872456

- I also predicted the `casual` and `registered` users seperately and then added them to get the total `cnt` prediction

- Model Evaluation Metrics
    Total R²: 0.7956071879602671
    Total MAE: 694.7402080528375
    Total RMSE: 951.9308156959494

**Model Comparison Summary**  
- **Linear Regression** explains slightly more variance (R² = 81%) and has lower RMSE, meaning it performs better overall on this dataset.  
- **Decision Tree Regression** has a slightly worse R² and RMSE 