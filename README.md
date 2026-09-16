# 🏃 Activity Recognition Using Random Forest

## 📌 Project Overview

This project uses a **Random Forest Classifier** to recognize and classify different human activities from the provided dataset.

The model learns patterns from the input features and predicts the corresponding activity.

The project also evaluates the model using **Accuracy, Precision, Recall, and F1 Score**, with a **Confusion Matrix** used to visualize classification performance.

## 🎯 Project Objective

The objective of this project is to build a machine learning model capable of classifying different types of human activities.

This project demonstrates:

* Data loading and preprocessing
* Feature and target separation
* Train-test splitting
* Random Forest classification
* Multiclass model evaluation
* Confusion matrix visualization

## 📊 Dataset

The project uses a CSV dataset containing features related to human activity.

The target variable is:

```text id="5y3x8k"
Activity
```

The `Activity` column contains the activity classes, while the remaining columns are used as input features.

## 🤖 Machine Learning Model

### Random Forest Classifier

Random Forest is an ensemble machine learning algorithm that combines multiple decision trees to make predictions.

In this project, the model is configured with:

```python id="gq2n1c"
RandomForestClassifier(
    n_estimators=100,
    random_state=42
)
```

* `n_estimators=100` → Creates 100 decision trees.
* `random_state=42` → Ensures reproducible results.

## 🔄 Project Workflow

```text id="7x0h5n"
Load Dataset
     ↓
Separate Features and Target
     ↓
Split Data into Training and Testing Sets
     ↓
Train Random Forest Classifier
     ↓
Make Predictions
     ↓
Calculate Evaluation Metrics
     ↓
Visualize Confusion Matrix
```

## 📈 Model Evaluation

The model is evaluated using four classification metrics.

### Accuracy

Measures the overall percentage of correctly classified activities.

### Precision

Measures how accurately the model identifies each activity when making predictions.

### Recall

Measures how many of the actual activity samples are correctly identified.

### F1 Score

Combines precision and recall into a single metric.

Because this is a **multiclass classification problem**, the project uses:

```python id="z4h1qh"
average='weighted'
```

This calculates the metrics across all activity classes while taking the number of samples in each class into account.

## 📉 Confusion Matrix

A confusion matrix is used to visualize how well the Random Forest model distinguishes between the different activity classes.

The diagonal elements represent correctly classified samples, while values outside the diagonal represent misclassifications.

## 📁 Project Structure

```text id="f1g2v7"
Activity-Recognition/
│
├── train.csv
├── main.py
└── README.md
```

## 🛠️ Technologies Used

* Python
* Pandas
* Scikit-learn
* Random Forest
* Seaborn
* Matplotlib

## ▶️ How to Run

### 1. Clone the repository

```bash id="k5x2dz"
git clone https://github.com/Vedline2547/Human-activity-recognition.git
```

### 2. Navigate to the project

```bash id="z8b2hm"
cd Activity-Recognition
```

### 3. Create a virtual environment

```bash id="x3v9qk"
python -m venv .venv
```

### 4. Activate the virtual environment

Windows PowerShell:

```bash id="c7m1wr"
.venv\Scripts\Activate.ps1
```

### 5. Install dependencies

```bash id="q2n6vt"
pip install pandas scikit-learn seaborn matplotlib
```

### 6. Run the project

```bash id="r8d4pk"
python main.py
```

## 💡 What I Learned

Through this project, I practiced:

* Working with multiclass classification problems
* Training Random Forest models
* Splitting datasets into training and testing sets
* Evaluating multiclass classification models
* Using weighted precision, recall, and F1 score
* Creating and interpreting confusion matrices
* Visualizing machine learning results with Seaborn and Matplotlib

## 🚀 Future Improvements

Possible improvements include:

* Feature scaling and preprocessing
* Hyperparameter tuning
* Feature importance analysis
* Comparin
