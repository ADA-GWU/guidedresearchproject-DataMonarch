This repository contains the contents of the research conducted in line with the course "Guided Research Methods". Contents of this repository are as follows:
* `data`: contains (reference to) the data used in the project
* `notebooks`: contains the notebooks developed for testing purposes
* `papers`: contains the papers used for literature review and project development
* `reports`: contains the reports submitted for the course (proposal, midterm, final). Weekly reports are made available in the form of updates to the README file under the `reports` folder.
* `presentations`: contains the presentations prepared as a part of the course deliverables

# Reserach Project: "CRYPTOCURRENCY PRICE FORECASTING: COMPARATIVE ANALYSIS OF DEEP LEARNING MODELS WITH OUTLIER HANDLING"

## Problem Significance'

Cryptocurrencies have emerged as a popular investment asset class, attracting attention from individuals and institutions worldwide. However, the volatility and unpredictability of cryptocurrency prices pose significant challenges for investors and traders. Accurate forecasting of cryptocurrency prices can aid in decision-making, risk management, and potential profit generation. Deep learning models have shown promise in capturing complex patterns and dependencies in time-series data, making them suitable for cryptocurrency price prediction. However, there has been a fleet of such models developed to combat this task of time-series forecasting ranging from classical machine learning algorithms, most notably the ARIMA-family models, to more complex statistical, e.g. prophet by META, and deep learning models. The primary goal of this project is to study the various techniques that have been developed so far with, on publicly available data to provide a comprehensive comparative analysis. It should also be noted that heavy emphasis will be placed on deep learning models.

Furthermore, the presence of outliers in cryptocurrency data can affect the performance and accuracy of these models. Therefore, investigating the impact of outlier removal on the performance of deep learning models for cryptocurrency price prediction is crucial to improve the reliability and usefulness of such predictions. It is for this reason that the secondary objective of this study is to apply different outlier detection and removal techniques and  analyze the impact on the tested models.

Last, but not least, I am planning to analyze the interpretability and visualization of the inner layers of these models to gain insights into their predictive power.


## Technical Objectives

The technical objectives of this research project include:

* **Comparative Analysis**: Evaluate and compare the performance of various deep learning models, including ARIMA-family models, Prophet, RNN, LSTM, and Temporal-fusion Transformers for cryptocurrency price prediction. Assess their ability to capture the complex dynamics and non-linear patterns of cryptocurrency price data.

* **Outlier Removal Techniques**: Investigate the impact of different outlier removal techniques on the predictive power of the deep learning models. Explore methods such as statistical measures, anomaly detection algorithms, or data preprocessing techniques to mitigate the influence of outliers on model performance. Special efforts will be exerted to test the feasibility of SR-CNN architecture models for outlier detection, a technique borrowed from the Computer Vision domain

* **Inner Layer Interpretability and Visualization**: Analyze the inner layers of deep learning models to interpret and visualize their decision-making processes. Explore techniques such as activation maximization, gradient-based visualization, or saliency maps to gain insights into the features and patterns that drive the models' predictions.


