# README: Emissions Analysis Using Machine Learning Models

## Table of Contents

1. [Overview](#overview)
2. [Dataset Description](#dataset-description)
3. [Analysis Process](#analysis-process)
4. [Model Performance and Findings](#model-performance-and-findings)
5. [Conclusion and Recommendations](#conclusion-and-recommendations)

## Overview

This project aims to analyze emissions data using various machine learning models to identify trends and insights. The dataset used contains records from the Carbon Majors Emissions dataset, which includes emissions data from various entities over several years. The main goal is to evaluate the performance of different models in predicting emissions based on historical data.

## Dataset Description

The dataset contains the following key features:

- **Year**: The year of the emission record.
- **Parent Entity**: The entity responsible for the emissions.
- **Parent Type**: The type of entity (e.g., state-owned, private).
- **Commodity**: The type of commodity (e.g., Oil & NGL, Natural Gas).
- **Production Value**: The production value for the commodity.
- **Production Unit**: The unit of measurement for production (e.g., Million bbl/yr, Bcf/yr).
- **Total Emissions (MtCO2e)**: The total emissions in million tonnes of CO2 equivalent.

The dataset is highly detailed and provides a comprehensive view of emissions over time, making it suitable for machine learning analysis.

## Analysis Process

The analysis process involved the following steps:

1. **Data Preprocessing**: Cleaning and preparing the data for analysis, including handling missing values and normalizing the data.
2. **Feature Selection**: Identifying the most relevant features for predicting emissions.
3. **Model Training**: Training various machine learning models on the dataset, including Linear Regression, Decision Trees, Random Forests

## Model Performance and Findings

### Imbalance and Bias in the Data

- **Different Units**: The dataset was found to have values in different units in terms of the Production Value. Which forced me to drop the minority Production Value unit.
- **Bias**: There were inherent biases in the data due to the way it was collected and processed. These biases can skew the model's predictions and reduce its generalizability.

### Model Performance

- **Linear Regression**: Provided a baseline performance with moderate accuracy.
- **Decision Trees**: Showed improved performance but were prone to overfitting.
- **Random Forests**: Outperformed Decision Trees by averaging multiple trees to reduce overfitting.


## Conclusion and Recommendations

The analysis highlights the importance of using balanced and unbiased datasets for training machine learning models. For future work, the following steps are recommended:

1. **Data Balancing**: Apply techniques such as oversampling the minority class or undersampling the majority class to balance the dataset.
2. **Bias Mitigation**: Address biases in the data collection and processing stages to improve the model's generalizability.
3. **Continuous Monitoring**: Continuously monitor and update the model with new data to maintain its effectiveness.

By implementing these strategies, more reliable and valid machine learning models for emissions analysis can be developed.
