# Introduction

This report is meant to serve as a progress report for the activities carried out in the first half of the semester. The report is divided into three sections: the research strategy, data collection and data cleaning.

# Research Strategy

## Brief Overview of the Project
The primary aim of this research project is to compare the performance of two models: the LSTM model and the Neural Prophet model by META (formerly known as Facebook). The comparison will be based on the USD values of two cryptocurrencies, Bitcoin and DOT. Bitcoin is chosen due to its popularity and long history, while DOT is selected for its relatively recent establishment and highly volatile price history. The performance of the models will be assessed using two criteria: the Root Mean Squared Error (RMSE) and the Mean Absolute Percentage Error (MAPE) of the predicted price.

To ensure a fair comparison, both models will undergo identical data preprocessing, model training, and model evaluation pipelines. Equal effort will be devoted to finding the optimal hyperparameters for both models within the given time frame, ensuring that they are trained with the best possible hyperparameters.

The process of tuning hyperparameters will provide valuable insights into the impact of different hyperparameters on the performance of the models. These insights will be thoroughly documented, analyzed, and presented in the final report.


## Research Project Plan
The detailed project plan is as follows:
1. ~~Data Collection~~
2. ~~Data Cleaning~~
3. Data Preprocessing
    1. ~~Sliding Window Approach for creation of time series data~~
    2. Scaling and Feature Engineering - ***In Progress***
4. Model Training
    1. LSTM Model Training and Hyperparameter Tuning - ***In Progress***
    2. Neural Prophet Model Training and Hyperparameter Tuning
5. Model Evaluation
    1. Direct Forecasting - ***In Progress***
    2. Recursive Forecasting over a fixed time horizon with smaller model prediction intervals
6. Comparative Analysis of Model Performance and Hyperparameter Tuning - Written Submission
    1. Comparison of the model performance based on the evaluation metrics
    2. Comparison of the impact of different hyperparameters on the model performance
