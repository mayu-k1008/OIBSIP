
# Car Price Prediction using Machine Learning

## Overview
Car price prediction is an essential problem in the automotive industry, where various factors like brand value, car features, mileage, and condition impact the price. In this project, we developed a machine learning model to predict car selling prices based on historical data.

## Dataset
The dataset consists of various features like:
- **Year**: Year of car manufacture
- **Selling_Price**: Price at which the car is sold (Target variable)
- **Present_Price**: Current market price of the car
- **Driven_kms**: Number of kilometers the car has been driven
- **Fuel_Type**: Type of fuel used (Petrol/Diesel/CNG)
- **Seller_Type**: Whether the seller is an individual or a dealer
- **Transmission**: Whether the car is Manual or Automatic
- **Owner**: Number of previous owners

## Project Workflow
1. **Data Collection & Exploration**
   - Loaded dataset using Pandas
   - Explored data using `.head()`, `.info()`, `.describe()`
   - Checked for missing values and data types

2. **Data Preprocessing & Feature Engineering**
   - Created a new feature **Car_Age** from the year of manufacture
   - Dropped irrelevant columns (**Year, Car_Name**)
   - Encoded categorical features using OneHotEncoding
   - Split the dataset into training and testing sets (80-20 ratio)

3. **Exploratory Data Analysis (EDA)**
   - Visualized data distribution and relationships using **Seaborn**
   - Generated **correlation heatmaps** to analyze feature dependencies

4. **Model Selection & Training**
   - **Linear Regression Model**
   - **Random Forest Regressor** (Best performance)
   - Evaluated models using **Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and R² Score**

5. **Hyperparameter Tuning**
   - Used **GridSearchCV** to optimize Random Forest hyperparameters for better accuracy
   
## Results
- **Linear Regression**: Achieved **R² score of 0.85**
- **Random Forest**: Performed better with higher accuracy and lower error rates
- **Feature Importance Analysis**: Showed that **Present Price and Car Age** were the most significant factors in predicting car prices.

## Technologies Used
- **Python**
- **Pandas, NumPy** (Data Handling)
- **Matplotlib, Seaborn** (Data Visualization)
- **Scikit-Learn** (Machine Learning Models)

## Conclusion
- **Random Forest Regressor** outperformed Linear Regression in predicting car prices.
- Feature Engineering (Car Age) improved model accuracy.
- The model can be further enhanced with advanced techniques like **feature scaling, polynomial regression, and deep learning models**.

## Future Improvements
- Deploying the model as a **web application** for users to estimate car prices.
- Expanding the dataset with more real-world features like **car condition, accident history, and region-specific pricing**.





