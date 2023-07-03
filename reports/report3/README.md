# Introduction

This report entails the details on the measurements strategies that is used to conduct the project, and the statistical and visual analysis of the data at hand.

# Measurement strategies

## Training and Testing Data
Given that the data for this research project will be obtained through an Application Programming Interface (API), there is no specific measurement stage required to collect the necessary data. The API will serve as a direct source, providing access to real-time and historical cryptocurrency price data for Bitcoin and DOT. This eliminates the need for manual data collection or additional measurement procedures, ensuring a streamlined and efficient data acquisition process. By directly accessing the API, we can ensure the accuracy and reliability of the data, enabling a robust analysis and comparison of the LSTM and Neural Prophet models without any measurement-related uncertainties or biases.

## Generated Experimental Data

The measurement strategies employed in this research project aim to facilitate a comprehensive and fair comparison between the purely LSTM model and the Neural Prophet model by META. To ensure an unbiased evaluation, a consistent set of measurement criteria will be utilized, focusing on the USD equivalents of two cryptocurrencies: Bitcoin and DOT.

The primary measurement criteria for comparing the performance of the models will include the Root Mean Squared Error (RMSE) and the Mean Absolute Percentage Error (MAPE) of the predicted price. These metrics provide insights into the accuracy and precision of the models' price predictions. By comparing these metrics for both models, we can assess their respective strengths and weaknesses in forecasting cryptocurrency prices.

To ensure a fair comparison, identical data preprocessing, model training, and model evaluation pipelines will be implemented for both the LSTM and Neural Prophet models. This approach guarantees that any performance differences observed can be attributed solely to the characteristics and capabilities of the models themselves, rather than the specific procedures employed.

By carefully tuning the hyperparameters, we aim to maximize the performance of each model and explore the impact of different hyperparameter configurations on their predictive accuracy. The resulting insights gained from this process will be thoroughly documented, analyzed, and presented in the final research report.

