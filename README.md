# titanic-survival-prediction
End-to-end Machine Learning project on the Titanic dataset including EDA, data preprocessing, feature engineering, model training, evaluation, and survival prediction using Python, Scikit-learn, XGBoost, and LightGBM.

-------------------------------------------------------------------------------------------------------------------------------

# 🚢 Titanic Survival Prediction using Machine Learning

![Titanic Ship](https://upload.wikimedia.org/wikipedia/commons/f/fd/RMS_Titanic_3.jpg)

## 📌 Project Overview

This project is an end-to-end Machine Learning classification project based on the famous Titanic dataset from Kaggle.

The main objective of this project is to predict whether a passenger survived the Titanic disaster using different passenger-related features such as:

- Gender
- Age
- Passenger Class
- Fare
- Embarked Station
- Family Information

This notebook covers the complete Machine Learning workflow including:

- Data Understanding
- Exploratory Data Analysis (EDA)
- Data Cleaning
- Feature Engineering
- Data Preprocessing
- Model Training
- Model Evaluation
- Final Prediction Generation

---

# 📂 Dataset Information

Dataset Source:
- Kaggle Titanic Competition

Files Used:
- `train.csv`
- `test.csv`

Target Variable:
- `Survived`

---

# 🛠 Libraries & Technologies Used

## Programming Language
- Python

## Libraries
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Models Building
- XGBoost
- LightGBM

## Environment
- Jupyter Notebook

---

# 📊 Data Understanding

The project started with understanding the dataset structure using:

```python
.head()
.info()
.describe()
.shape
```

This helped identify:
- feature types
- missing values
- categorical columns
- numerical columns
- dataset distribution

---

# 📈 Exploratory Data Analysis (EDA)

Exploratory Data Analysis was performed to understand survival patterns and relationships between different features.

## Analysis Performed

### ✅ Survival Distribution
Analyzed overall passenger survival distribution.

### ✅ Gender-Based Survival Analysis
Observed that female passengers had a much higher survival rate compared to male passengers.

### ✅ Passenger Class Analysis
Passengers from higher classes had better survival chances.

### ✅ Embarked Station Analysis
Analyzed survival patterns based on embarkation location.

### ✅ Family Size Analysis
Created a new feature called `FamilySize` using:

```python
FamilySize = SibSp + Parch + 1
```

This feature helped better represent family relationships among passengers.

---

# 📊 Data Visualization

The following visualizations were used:

- Heatmaps
- Countplots
- Barplots
- Correlation Matrix

These visualizations helped identify:
- survival trends
- feature relationships
- important predictors

---

# ⚙️ Data Cleaning & Preprocessing

Several preprocessing steps were performed before training machine learning models.

---

## Missing Value Handling

Missing values were handled in:
- Age
- Fare
- Embarked

Techniques used:
- Mean Imputation
- Median Imputation
- Removing minimal missing rows

---

## Dropped Columns

The following columns were removed:

```python
Cabin
Name
Ticket
```

Reason:
- excessive missing values
- unstructured information
- lower predictive importance

---

## Encoding Categorical Variables

Categorical features were converted into numerical format using:

```python
LabelEncoder()
```

Encoded Features:
- Sex
- Embarked

This step was necessary because machine learning models cannot process text values directly.

---

# 🧠 Feature Engineering

Feature Engineering was performed by creating:

```python
FamilySize
```

This improved the dataset by combining family-related information into a single meaningful feature.

---

# 🔀 Train-Test Split

The dataset was divided into:
- Training Data
- Validation Data

using:

```python
train_test_split()
```

This allowed proper model evaluation on unseen data.

---

# 🤖 Machine Learning Models Used

Multiple machine learning models were trained and evaluated.

---

## 1️⃣ Logistic Regression

Used as a baseline classification model.

### Advantages
- Simple
- Fast
- Easy to interpret

---

## 2️⃣ XGBoost Classifier

Advanced boosting algorithm used to improve prediction performance.

### Advantages
- High accuracy
- Handles complex patterns
- Strong ensemble learning approach

---

## 3️⃣ LightGBM Classifier

Efficient gradient boosting framework optimized for speed and scalability.

### Advantages
- Faster training
- Efficient memory usage
- Good performance on structured data

---

# 📊 Model Evaluation

Models were evaluated using:

- Accuracy Score
- Confusion Matrix
- Classification Report

These metrics helped measure model performance and classification quality.

---

# 🎯 Final Result

## ✅ Final Accuracy Achieved:
# **75.358%**

The final model successfully predicted passenger survival with competitive beginner-intermediate level performance.

---

# Author
Gaurav Kumar

# 📁 Project Structure

```bash
├── titanic-survival-prediction.ipynb
├── train.csv
├── test.csv
├── submission.csv
├── requirements.txt
└── README.md
```

---

# ▶️ How to Run the Project

## 1️⃣ Clone Repository

```bash
git clone https://github.com/yourusername/titanic-survival-prediction.git
```

---

## 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 3️⃣ Open Jupyter Notebook

```bash
jupyter notebook
```

Then open:

```bash
titanic-survival-prediction.ipynb
```

---

# 📌 Key Learnings

Through this project, I learned:

- Data preprocessing techniques
- Handling missing values
- Exploratory Data Analysis (EDA)
- Feature engineering
- Machine Learning classification models
- Model evaluation techniques
- End-to-end ML workflow

---

# 🚀 Future Improvements

Possible future improvements include:

- Hyperparameter tuning
- Cross-validation
- Pipeline implementation
- Advanced feature engineering
- Ensemble techniques
- Deployment using Flask or Streamlit

---

# 🏆 Kaggle Competition

This project is based on the famous Kaggle Titanic competition:

https://www.kaggle.com/competitions/titanic

---

# 🙌 Acknowledgements

Special thanks to:

- Kaggle
- Scikit-learn Documentation
- Open-source ML Community

---

# ⭐ If You Like This Project

If you found this project useful, consider giving this repository a ⭐ on GitHub.
