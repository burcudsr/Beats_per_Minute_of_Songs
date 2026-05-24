# 🎵 Beats-per-Minute (BPM) Prediction

This project focuses on predicting the Beats-per-Minute (BPM) of songs using machine learning techniques. The project utilizes data from the **Kaggle Playground Series - Season 5, Episode 9**.

### 🚀 Live Demo
Explore the interactive BPM prediction model here: **[BPM Prediction App](https://huggingface.co/spaces/bdaser/BPM)**

### 📊 Dataset & Preprocessing
The dataset provides a set of audio-related features to predict song tempo, comprising a total of **524,164 training samples**. Key preprocessing steps include:
* **Feature Scaling**: To optimize model training, features were normalized using `MinMaxScaler`.
* **Data Integrity**: The dataset was processed to ensure all features are in a clean, numerical format ready for regression analysis.

### 🤖 Model Performance
Various regression algorithms were evaluated. Submissions are officially evaluated using **Root Mean Squared Error (RMSE)**, while our analysis also monitored **Mean Absolute Error (MAE)**. The performance metrics are summarized below:

| Model | R-Squared | RMSE | MAE |
| :--- | :--- | :--- | :--- |
| **Gradient Boosting** | 0.000486 | 26.438711 | 21.179755 |
| **Ridge** | 0.000095 | 26.443880 | 21.184139 |
| **Linear Regression** | 0.000095 | 26.443880 | 21.184139 |
| **XGBRegressor** | -0.008001 | 26.550723 | 21.263813 |

### 📈 Analysis Summary
The competition utilizes **Root Mean Squared Error (RMSE)** as the primary evaluation metric. Our analysis shows that while multiple models were tested, the **Gradient Boosting** regressor provided the most competitive performance in minimizing prediction error. 
