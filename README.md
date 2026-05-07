# 🚢 Day 5 - Titanic Classifier

This notebook performs data cleaning, EDA, feature engineering, and classification modeling on the Titanic dataset.

## 📌 Dataset

The dataset contains information about passengers aboard the Titanic. The goal is to predict **who survived** based on features like age, sex, class, fare, etc.

---

## 🔍 Steps Performed

### ✅ 1. Data Cleaning
- Filled missing `Age` values with the median.
- Dropped the `Cabin` column (too many missing values).
- Filled missing `Embarked` values with the mode.

### 📊 2. Exploratory Data Analysis
- Visualized null values
- Heatmap of correlation between features and target
- Checked survival rate by features

### 🛠️ 3. Feature Engineering
- Converted `Sex` and `Embarked` to numerical using `pd.get_dummies`.
- Selected useful features for training.

### 🧠 4. Model Building
- Used `RandomForestClassifier` from `sklearn`.
- Trained model with 80/20 train-test split.

---

## 📈 Model Performance

### ✅ Confusion Matrix

|               | Predicted: 0 | Predicted: 1 |
|---------------|--------------|--------------|
| Actual: 0     | 88           | 17           |
| Actual: 1     | 17           | 57           |

### 📊 Classification Report

| Metric    | Died (0) | Survived (1) | Accuracy |
|-----------|----------|--------------|----------|
| Precision | 0.84     | 0.77         | 0.81     |
| Recall    | 0.84     | 0.77         |          |
| F1-score  | 0.84     | 0.77         |          |

---

## 📁 Files Included
- `titanic_classifier.ipynb`: Jupyter notebook
- `README.md`

---

## 📚 Learnings
- Real-world data is messy — handling nulls is critical
- EDA helps understand hidden patterns (like class or sex affecting survival)
- Confusion matrix and classification report show how your model performs beyond accuracy

---

## 🚀 Next Step
On to **Day 6** – building smarter models!

