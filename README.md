# 🎓 Student Performance Prediction Using Machine Learning

A Machine Learning project that analyzes student-related data and applies different Machine Learning algorithms to predict student outcomes.

## 📌 Project Overview

This project explores the relationship between **student characteristics, study habits, attendance, and academic performance** using Machine Learning.

The dataset contains **11,926 student records** with features such as:

* Age
* Gender
* Study Hours
* Attendance Percentage
* Internet Access
* Extra Activities
* Mathematics Score
* Science Score
* English Score
* Overall Score
* Final Grade (A–F)

The project includes both **regression and classification** tasks depending on the target variable.

## 🎯 Objectives

* Analyze factors that influence student performance.
* Predict continuous academic scores.
* Classify categorical student outcomes.
* Compare different Machine Learning algorithms.
* Understand the strengths and limitations of each algorithm.
* Evaluate the predictive power of student-related features.

## 🤖 Machine Learning Algorithms

Five Machine Learning algorithms were studied:

| Algorithm                    | Problem Type   | Used For                           |
| ---------------------------- | -------------- | ---------------------------------- |
| Linear Regression            | Regression     | Predicting overall/exam scores     |
| Logistic Regression          | Classification | Predicting Internet Access         |
| K-Nearest Neighbors (KNN)    | Classification | Predicting Final Grade             |
| Support Vector Machine (SVM) | Classification | Separating Extra Activities groups |
| Naive Bayes                  | Classification | Predicting Extra Activities        |

These algorithms were selected according to the type of target variable and the characteristics of the prediction task.

## 📊 Model Details

### 1. Linear Regression

Linear Regression was used for predicting continuous values such as `overall_score`.

It provides a simple and interpretable baseline for understanding how features such as study hours and attendance relate to academic scores.

### 2. Logistic Regression

Logistic Regression was used to predict `internet_access` as a binary outcome (`Yes/No`).

The model achieved approximately **50% accuracy**, indicating that `study_hours` alone is a weak predictor of internet access in this dataset.

### 3. K-Nearest Neighbors (KNN)

KNN was considered for predicting `final_grade`.

The algorithm classifies students based on similarity to other students, making it useful for identifying local patterns among students with similar study habits, attendance, and scores.

### 4. Support Vector Machine (SVM)

SVM was used to analyze the separation between `extra_activities` groups.

It focuses on finding a decision boundary with the maximum margin between classes and can handle non-linear relationships using kernels.

### 5. Naive Bayes

Naive Bayes was used to predict `extra_activities` (`Yes/No`) using:

* Age
* Study Hours
* Attendance Percentage

The model achieved approximately **50% accuracy**, suggesting that these features have limited predictive power for determining participation in extra activities.

## 📈 Results

The classification experiments showed relatively low predictive performance, with some models achieving accuracy close to **50%**.

This suggests that features such as **study hours, attendance percentage, and age alone are not sufficient to accurately predict some categorical student outcomes**.

### Key Findings

* `overall_score` is suitable for regression-based prediction.
* Logistic Regression provides an interpretable baseline for binary classification.
* KNN can capture local similarities between students.
* SVM can be useful for analyzing class separation.
* Naive Bayes provides a fast probabilistic baseline.
* Additional features and better feature engineering may improve classification performance.

## 🛠️ Technologies Used

* Python
* Jupyter Notebook
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

## 📂 Project Structure

```text
Student-Performance-ML/
│
├── student_performance 2.ipynb
├── Student performance ML_Project_Report.docx
├── README.md
└── dataset/
    └── student_performance.csv
```

> Update the dataset filename/folder if your actual project uses a different name.

## 🚀 How to Run the Project

### 1. Clone the repository

```bash
git clone <your-github-repository-url>
cd Student-Performance-ML
```

### 2. Install the required libraries

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### 3. Start Jupyter Notebook

```bash
jupyter notebook
```

### 4. Open the notebook

Open:

```text
student_performance 2.ipynb
```

Run the notebook cells sequentially to perform the analysis and Machine Learning experiments.

## 🔍 Project Workflow

```text
Dataset
   ↓
Data Loading
   ↓
Data Exploration
   ↓
Data Preprocessing
   ↓
Feature Selection
   ↓
Train-Test Split
   ↓
Machine Learning Models
   ↓
Model Evaluation
   ↓
Result Analysis
```

## 📌 Limitations

The classification models showed relatively low accuracy in the experiments. This indicates that the selected features do not contain enough information to reliably predict some categorical outcomes.

The project report recommends exploring:

* Additional student-related features
* Feature engineering
* Hyperparameter tuning
* More comprehensive model comparison

These improvements could potentially increase prediction performance.

## 🔮 Future Improvements

Possible future enhancements include:

* Feature engineering
* Hyperparameter optimization
* Cross-validation
* More Machine Learning algorithms
* Better handling of class imbalance
* Additional student behavioral and academic features
* Improved model evaluation using precision, recall, F1-score, and confusion matrices
* Deployment as a web application

## 🏆 Conclusion

This project demonstrates that **there is no single best Machine Learning algorithm for every problem**. The appropriate algorithm depends on the type of target variable and the structure of the data.

Linear Regression is appropriate for continuous score prediction, while Logistic Regression and Naive Bayes provide probabilistic approaches for binary classification. KNN provides a similarity-based approach, and SVM provides a margin-based classification perspective.

Overall, the project provides a practical comparison of multiple Machine Learning techniques for analyzing and predicting student performance.

## 👨‍💻 Author

**VeeraTamil V K**

---

⭐ If you found this project useful, consider giving the repository a star!
