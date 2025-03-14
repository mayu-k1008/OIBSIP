# 🌸 Iris Flower Classification

This project classifies **Iris flower species** based on sepal and petal measurements.

## 📌 Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Model Training](#model-training)
- [Model Evaluation](#model-evaluation)
- [Model Improvement](#model-improvement)
- [Hyperparameter Tuning](#hyperparameter-tuning)
- [Deployment](#deployment)

## 🔍 Introduction
This project implements machine learning models to classify **Iris flower species** (Setosa, Versicolor, Virginica) based on their sepal and petal measurements. We use **Decision Trees** and **Random Forest** classifiers for the classification task.

## 📊 Dataset
The dataset used is the famous **Iris Dataset**, which contains:
- 150 samples
- 4 feature columns: *SepalLengthCm, SepalWidthCm, PetalLengthCm, PetalWidthCm*
- 1 target column: *Species*

## 🛠 Installation
To run this project, install the required libraries:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## 🚀 Usage
Run the Python script to classify Iris flower species:
```bash
python iris_flower_classification.py
```

## 📊 Exploratory Data Analysis (EDA)
We perform EDA using:
- **Pair Plot** to visualize relationships between features
- **Correlation Heatmap** to observe feature correlations

## 🎯 Model Training
We train a **Decision Tree Classifier** on the dataset:
```python
model = DecisionTreeClassifier()
model.fit(X_train, y_train)
```

## 📈 Model Evaluation
We evaluate the model using:
- **Accuracy Score**
- **Confusion Matrix**
- **Classification Report**

Example:
```python
accuracy = accuracy_score(y_test, y_pred)
print(f"Model Accuracy: {accuracy:.2f}")
```

## 🔄 Model Improvement
We improve the model by training a **Random Forest Classifier**:
```python
rf_model = RandomForestClassifier(n_estimators=100, random_state=42)
rf_model.fit(X_train, y_train)
print("Random Forest Accuracy:", accuracy_score(y_test, y_rf_pred))
```

## 🔧 Hyperparameter Tuning
We use **GridSearchCV** to optimize the Decision Tree model:
```python
param_grid = {'max_depth': [3, 5, 7], 'criterion': ['gini', 'entropy']}
grid_search = GridSearchCV(DecisionTreeClassifier(), param_grid, cv=5)
grid_search.fit(X_train, y_train)
print("Best Parameters:", grid_search.best_params_)
```

## 🚀 Deployment
To classify a new sample:
```python
sample_data = pd.DataFrame([[5.1, 3.5, 1.4, 0.2]], columns=feature_names)
prediction = model.predict(sample_data)
predicted_species = label_encoder.inverse_transform(prediction)
print("Predicted Species:", predicted_species[0])
```



---

🎉 **Happy Coding!**

