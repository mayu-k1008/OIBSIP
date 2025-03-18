# Sales Prediction Using Python

## Overview
This project predicts product sales based on advertising budgets for **TV, Radio, and Newspaper**. It applies **Linear Regression and Polynomial Regression** to analyze and improve sales forecasts.

## Dataset
- **Columns:**
  - `TV`: Advertising budget for TV (in thousands of dollars)
  - `Radio`: Advertising budget for Radio (in thousands of dollars)
  - `Newspaper`: Advertising budget for Newspaper (in thousands of dollars)
  - `Sales`: Sales of the product (in thousands of units)

## Steps in the Project
### 1. Load Dataset
- Read the dataset (`Advertising.csv`) and remove unnecessary columns.

### 2. Exploratory Data Analysis (EDA)
- Display dataset summary statistics.
- Visualize relationships using **pair plots** and **correlation heatmaps**.

### 3. Define Features & Target Variable
- Set **TV, Radio, and Newspaper** as input features.
- Set **Sales** as the target variable.

### 4. Train & Evaluate Models
#### **Linear Regression Model**
- Trained on 80% of the dataset.
- Evaluated on the test set using **MAE, MSE, RMSE, and R² Score**.

#### **Polynomial Regression Model (Degree = 2)**
- Captures non-linear relationships in the data.
- Demonstrates **higher accuracy (R² = 98.7%)** than Linear Regression.

### 5. Visualizations
- **Actual vs. Predicted Sales** plot.
- **Residual Distribution** plot.

## Results
| Model                | MAE  | MSE  | RMSE | R² Score |
|----------------------|------|------|------|----------|
| **Linear Regression**  | 1.46 | 3.17 | 1.78 | 89.9%    |
| **Polynomial (Degree 2)** | 0.52 | 0.41 | 0.64 | **98.7%** |

## Conclusion
- **Polynomial Regression (degree = 2) is the best-performing model** for sales prediction.
- Higher accuracy and reduced errors make it **ideal for forecasting future sales based on advertising budgets**.

## Requirements
To run this project, install the required Python libraries:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## How to Run
1. Download and place `Advertising.csv` in the project directory.
2. Run the Python script:  
   ```bash
   python sales_prediction.py
   ```
3. View the results and visualizations.