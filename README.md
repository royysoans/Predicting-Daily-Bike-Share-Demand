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

- Observations:-
    It is easier for the model to predict the number of registered users(R²=84%) however it is more difficult to predict for casual users (R²=67%).