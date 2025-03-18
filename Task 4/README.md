# 📧 Email Spam Detection with Machine Learning

## 📌 Project Overview
This project aims to build an **Email Spam Detector** using **Machine Learning**. The model classifies emails as **Spam (1)** or **Not Spam (0)** based on their content.

## 📂 Dataset
- **Dataset Used**: `spam.csv`
- **Total Entries**: 5572 emails
- **Columns**:
  - `label`: (ham/spam → converted to 0/1)
  - `message`: Email content

## 🛠️ Tech Stack
- **Python**
- **Pandas, NumPy** (Data Handling)
- **NLTK** (Text Processing)
- **Scikit-learn** (Machine Learning)

## 🔄 Data Preprocessing
1. **Lowercasing**
2. **Removing Punctuation & Stopwords**
3. **Stemming** (reducing words to root form)
4. **TF-IDF Vectorization** (converting text to numerical data)

## 🧠 Model Used
- **Multinomial Naïve Bayes** (Best suited for text classification)

## 📊 Model Evaluation
| Metric     | Score  |
|------------|--------|
| Accuracy   | 96.68% |
| Precision  | 99.12% |
| Recall     | 75.83% |
| F1-score   | 85.93% |

## 🚀 How to Run the Project
1. **Install Dependencies:**  
   ```bash
   pip install pandas numpy nltk scikit-learn
