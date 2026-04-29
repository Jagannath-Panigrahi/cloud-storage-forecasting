# Cloud Storage Cost Forecasting and Optimization

This repository contains the implementation of my M.Tech thesis titled **"Cloud Storage Cost Forecasting and Policy Simulation Using Machine Learning"**. The work focuses on predicting future cloud storage usage and estimating associated costs using time-series forecasting models, followed by applying a dynamic optimization policy to reduce overall expenses.

Cloud storage usage is not constant and changes over time due to varying workloads. This project addresses that challenge by combining forecasting techniques with cost analysis and optimization strategies. The goal is to not only predict future storage demand but also simulate how intelligent policies can help reduce cloud costs in a practical scenario.

The models implemented in this work include Naive forecasting, Moving Average, ARIMA, Holt-Winters, and XGBoost. These models provide a balanced comparison between baseline approaches, statistical methods, and machine learning techniques. Their performance is evaluated using standard metrics such as RMSE (Root Mean Squared Error), MAE (Mean Absolute Error), and sMAPE (Symmetric Mean Absolute Percentage Error).

A synthetic dataset is generated to simulate realistic cloud storage behavior, incorporating trend, seasonality, and noise. The experiments also include multi-horizon forecasting (7, 14, 28, 45, and 90 days) to evaluate how model performance changes over time. Additionally, stability testing is performed across different workload patterns such as steady, seasonal, bursty, and mixed conditions.

The predicted storage values are converted into cost using a simple pricing model. A dynamic optimization policy is then applied, where different levels of reduction are used depending on the storage usage. For example, low usage results in minimal reduction, while higher usage leads to more aggressive optimization. This simulates real-world strategies such as data archival and compression.

The results show that forecasting models provide reasonably stable predictions, while errors increase as the prediction horizon becomes longer. The proposed dynamic policy achieves measurable cost savings of approximately 5%, demonstrating the practical usefulness of combining forecasting with optimization.

The repository is structured in a simple and clear manner. The main implementation is provided in a Jupyter Notebook file, which includes dataset generation, model training, evaluation, visualization, and cost analysis. Any additional files such as datasets or plots are included where necessary.

To run the project, open the notebook file and execute the cells sequentially. All results, including graphs and evaluation metrics, will be generated automatically. The notebook is designed to be self-contained so that the entire experiment can be reproduced easily.

All code, dataset generation steps, and experiments are provided in this repository to support reproducibility. The implementation follows a straightforward workflow so that other researchers or students can understand and extend the work without difficulty.

Author: Jagannath Panigrahi
Degree: M.Tech in Computer Science and Engineering

This repository is intended for academic and research purposes. The work can be used as a reference or extended further with proper acknowledgment.

