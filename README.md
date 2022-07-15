# Classification Models to Identify Water Pump Functionality in Tanzania


# Overview

This project consists of classification models to identify water pump functionality in Tanzania. Limited access to safe water is a major health risk. These models are potential tools for government agencies or non-governmental organizations to identify areas with limited access to clean water. Through an iterative modeling process, we produced a model that predicted pump functionality with 85% accuracy. By identifying non-functional water pumps, organizations can divert resources to areas in need of assistance and improve water access and health in Tanzania.

# Business Understanding

Millions of people in Tanzania lack access to safe water. This results in paying high prices for water from vendors or collecting water from unsafe natural sources. In order to combat this problem, resources must be allocated to fix non-functioning water distribution points. Age is an important metric in predicting the condition of distribution points. Older pumps and engine systems are more likely to fail than newer ones. In many cases age related data is not available. The goal of this analysis is to build the model that can predict the condition of waterpoints based on their other features such as regional factors, installer, type of pump, population and others.

# Data Understanding and Analysis

The data was sourced from the Taarifa waterpoint dashboard, which aggregates data from the Tanzania Ministry of Water. The information collected was recorded by GeoData Consultants Ltd. There are 59,400 rows and 40 columns in the "water_well_train_data.csv".

Our target data is stored in "water_well_train_labels.csv". There are 59,400 rows and 2 columns in this csv file. The two columns in this csv file are 'id' and 'status_group'. The 'id' column aligns with the 'id' column in the "water_well_train_data.csv" file. Our target column is 'status_group' which consists of three values describing the status of a water pump: "functional", "functional needs repair", and "non-functional".

# Results

Using an iterative model building process, we developed three different types of models and evaluated their accuracy scores. 

Based on accuracy score alone, the Bagging classifier was our strongest performing model. The test scores for all three models were relatively close. Bagging classifier was at the top with 85.0% accuracy, the Random Forest classifier had 84.8% accuracy, and the K-Nearest Neighbors classifier had 83.2% accuracy.

![Model Accuracy Results on Test Data](./test_accuracy_scores.png)
