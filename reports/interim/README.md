# Introduction

This report is meant to serve as a progress report for the activities carried out in the first half of the semester and is an extension of report 3. The report is divided into three sections: the research strategy, Exploratory Data Analysis (EDA), and Model Training Results. The research strategy section provides a brief overview of the project and the research plan. The EDA section provides a detailed analysis of the data and the insights gained from the analysis. The Model Training Results section provides a summary of the model training results and the insights gained from the process.

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
        
        This method was used to generate the necessary input sequences to the model. The conducted experiments include different input sequence length with the same 1440 minutes of forecasting time step. The results of the experiments will be demonstrated in a later section.
    2. ~~Scaling and Feature Engineering~~
        
        Experiments on scaling have already been conducted and the results are shown in its dedicated section below. To summarize the results of this step the following can be stated:
        - The data was scaled using the MinMaxScaler from sklearn.preprocessing. The scaler was fit on the training data and then used to transform the training and testing data.
        - The only feature that is worth considering as the model input out of the fields available in the original dataset is the Close price. The other features have either negative or a very insignificant positive influence on the model performance.
        - The data is processed as a sliding window and it has been discovered that adding the mean and the standard deviation of the input sequence as static features greatly improves the model performance. For a 1 minute prediction (single-step prediction) I managed to reduce the LSTM architecture's footprint from 4 layers with 250 units each to 4 layers with 180 units without any loss in performance. This phenomenon was later on observed in the case of 720-minute and 1440-minute forecasts as well.
4. Model Training
    1. ~~LSTM Model Training and Hyperparameter Tuning~~

        It should be noted that due to the way in which the training pipeline is developed, in/exclusion of original dataset fields as a part of the input sequence, addition of static features (as mentioned above) and addition of the differently scaled moving averages of the input sequence as a part of the input data can easily be achieved through changes in a config file, rather than a change in the code itself. This allows for a very flexible and efficient way of experimenting with different model architectures and input data. Thus, the input features can also be referred to as a hyperparameter of the model.


        **The experiments on this specific hyperparameter are still on-going, but the results will be presented in a later report.**
    2. Neural Prophet Model Training and Hyperparameter Tuning
5. Model Evaluation
    1. ~~Direct Forecasting~~
    2. Recursive Forecasting over a fixed time horizon with smaller model prediction intervals - ***In Progress***
6. Comparative Analysis of Model Performance and Hyperparameter Tuning - Written Submission
    1. Comparison of the model performance based on the evaluation metrics
    2. Comparison of the impact of different hyperparameters on the model performance


# Measurement strategies

## Training and Testing Data
Given that the data for this research project will be obtained through an Application Programming Interface (API), there is no specific measurement stage required to collect the necessary data. The API will serve as a direct source, providing access to real-time and historical cryptocurrency price data for Bitcoin and DOT. This eliminates the need for manual data collection or additional measurement procedures, ensuring a streamlined and efficient data acquisition process. By directly accessing the API, we can ensure the accuracy and reliability of the data, enabling a robust analysis and comparison of the LSTM and Neural Prophet models without any measurement-related uncertainties or biases.

## Generated Experimental Data

The measurement strategies employed in this research project aim to facilitate a comprehensive and fair comparison between the purely LSTM model and the Neural Prophet model by META. To ensure an unbiased evaluation, a consistent set of measurement criteria will be utilized, focusing on the USD equivalents of two cryptocurrencies: Bitcoin and DOT.

The primary measurement criteria for comparing the performance of the models will include the Root Mean Squared Error (RMSE) and the Mean Absolute Percentage Error (MAPE) of the predicted price. These metrics provide insights into the accuracy and precision of the models' price predictions. By comparing these metrics for both models, we can assess their respective strengths and weaknesses in forecasting cryptocurrency prices.

To ensure a fair comparison, identical data preprocessing, model training, and model evaluation pipelines will be implemented for both the LSTM and Neural Prophet models. This approach guarantees that any performance differences observed can be attributed solely to the characteristics and capabilities of the models themselves, rather than the specific procedures employed.

By carefully tuning the hyperparameters, we aim to maximize the performance of each model and explore the impact of different hyperparameter configurations on their predictive accuracy. The resulting insights gained from this process will be thoroughly documented, analyzed, and presented in the final research report.


**Ps. The detailed report can be found in the pdf file under this directory or in the dedicated ![Jupyter Notebook file]()**