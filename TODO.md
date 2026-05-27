# general workflow

- investigate data
- clean useless columns, drop some rows with nan, etc
- preprocess
    - one hot encoding for cat
    - Pick a scaler, scale numerical columns
        - especially important are the date related columns
- pick some regression models
    - xgboost
    - catboost
    - gaussian process regressor
    - elastic-net;as a baseline
    - huber regressor
    - pls regressor
    - random forest regressor
    - extra trees regressor
- stratified kfold cross validation

- evaluation metric: root mean squared (logarithmic) error rmse between the log values of predicted and observed
- evaluation metric 2: mean absolute error, but dubious if real or not

