# Stock Price Movement Prediction - Classification Model

## Project Overview

This project aims to predict **stock price movement direction** (Buy/Sell) using **Logistic Regression** based on key financial indicators. The dataset consists of historical stock data from the Nairobi Stock Exchange (NSE). The model classifies whether the stock price will increase or decrease based on given features.

## Key Features

1. **Data Loading and Exploration**: The dataset is loaded and explored to understand its structure and key metrics.
2. **Preprocessing**:
   - Data cleaning and transformation.
   - Creation of a target variable (`Direction`), which indicates stock movement (1 for upward movement, 0 for downward movement).
3. **Feature Selection**: Identified relevant features for model training.
4. **Model Training and Evaluation**:
   - Logistic Regression is used for binary classification.
   - Performance is evaluated using metrics like **Confusion Matrix**, **Accuracy**, and **ROC-AUC**.

## Project Workflow

### 1. Data Preparation
- **Data Cleaning**: The `Change` column is converted into numerical values to represent stock price movement.
- **Feature Engineering**: The target variable `Direction` is derived from the `Change` column to indicate positive or negative stock price movement.
- **Feature Selection**: The following features were selected:
  - `12m High`
  - `12m Low`
  - `Day Low`
  - `Day High`
  - `Change`

### 2. Model Training
The dataset is split into training and test sets, and a **Logistic Regression** model is trained to predict the `Direction`.

### 3. Model Evaluation
- **Confusion Matrix**: Visualizes true vs. predicted classes.
- **Accuracy Score**: Measures the percentage of correct predictions.
- **ROC-AUC Curve**: Evaluates the modelâ€™s performance at various threshold levels.

### 4. Visualization
- Confusion matrix and ROC-AUC curve plots are generated to interpret model performance.

## Results

| Metric        | Value       |
|---------------|-------------|
| Accuracy      | **0.905716**|
| ROC-AUC Score | **0.994903**|



## Installation and Usage

### Prerequisites
- `Python 3.x`
- `pandas`
- `numpy`
- `scikit-learn`
- `matplotlib`

### Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/MuneneMutuma/Stock-Prediction-Classification.git
   cd Stock-Prediction-Classification
   ```

2. **Install Dependencies**:
   ```bash
   pip install pandas numpy matplotlib scikit-learn
   ```

3. **Run the Notebook**:
   Open the `Classification_Buy_Sell.ipynb` notebook in Jupyter or Colab and execute the cells in sequence.

## Conclusion

This project showcases the application of logistic regression to predict stock price movement direction. It provides a foundation for implementing more advanced classification models for financial prediction tasks.