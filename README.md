# Intelligent Sales Prediction using Machine Learning

## Overview
This project aims to forecast diamond sales by implementing multiple machine learning models and identifying the optimal one. The dataset, sourced from Kaggle, contains 53,940 samples with 10 properties each, including carat, cut, color, clarity, depth, table, price, and the x, y, z dimensions.

## Dataset Description
The dataset consists of the following features:

- **Carat**: The mass of the diamond (1 carat = 200mg). It is the main quantitative proportion of the 4 Cs and is directly related to the price.
- **Cut**: Refers to the shape of the stone and the quality of its sparkle, classified from "Fair" to "Ideal".
- **Color**: Diamonds range from colorless to light yellow. The Gemmological Foundation of America's classification, from "D" (colorless) to "Z" (light yellow), is used.
- **Clarity**: Evaluates internal imperfections, rated from FL (Flawless) to I3 (Obvious Inclusions) based on the size, nature, position, and quantity of imperfections.
- **Depth**: The ratio between the z dimension and the average width of the diamond's top.
- **Table**: The width of the diamond's top at its widest point.
- **Price**: The price of the diamond.
- **x, y, z**: The dimensions of the diamond.

## Objective
The primary objective is to implement and evaluate multiple machine learning models to find the optimal model for forecasting diamond prices. A penalty term was added to some models to stabilize them, leading to improved accuracy.

## Machine Learning Models Used
- Linear Regression
- Polynomial Regression
- Decision Tree Algorithm
- Random Forest Regressor
- Gradient Boost Algorithm

## Key Insights
- **Carat**: Proven to be among the most significant variables in pricing determination.
- **Model Stability**: Adding a penalty term helped stabilize the models, leading to the highest accuracy of around 98% with the Gradient Boost Algorithm.

## How It Works
### Data Preprocessing
1. **Data Cleaning**: Handle missing values and outliers.
2. **Feature Engineering**: Transform and encode categorical variables.
3. **Data Splitting**: Split the dataset into training and testing sets.

### Model Implementation
1. **Linear Regression**: Implemented to understand the linear relationship between features and price.
2. **Polynomial Regression**: Used to capture non-linear relationships.
3. **Decision Tree Algorithm**: Implemented to handle non-linearity and interactions between features.
4. **Random Forest Regressor**: Used for ensemble learning to improve predictive performance.
5. **Gradient Boost Algorithm**: Implemented to boost the model's performance by adding a penalty term, resulting in the highest accuracy.

### Model Evaluation
1. **Visualization**: Visualize the behavior of characteristics using graphs and plots.
2. **Model Stability**: Assess and enhance model stability by adding penalty terms.
3. **Accuracy Measurement**: Evaluate model performance using metrics like Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and R-squared (R²).

## Results
- The Gradient Boost Algorithm achieved the highest accuracy of around 98%.

## Conclusion
The project demonstrates the effectiveness of various machine learning models in forecasting diamond sales. The inclusion of a penalty term significantly improved the model's stability and accuracy.

## Installation
1. Clone the repository:
    ```sh
    git clone https://github.com/your-username/diamond-sales-prediction.git
    ```
2. Install the required dependencies:
    ```sh
    pip install -r requirements.txt
    ```

## Usage
1. Run the data preprocessing script:
    ```sh
    python data_preprocessing.py
    ```
2. Train the machine learning models:
    ```sh
    python train_models.py
    ```
3. Evaluate the models:
    ```sh
    python evaluate_models.py
    ```

