# Parkinson's Disease Prediction using Support Vector Machine (SVM)

## 🧠 Overview

Parkinson's Disease Prediction using Support Vector Machine (SVM) is a machine learning project that predicts whether a person is affected by Parkinson's disease using biomedical voice measurements.

The project demonstrates an end-to-end machine learning pipeline, including data preprocessing, feature scaling, model training using a Support Vector Machine (SVM) classifier, model evaluation, and prediction on unseen data.

The notebook was developed in **Google Colab** using Python and the Scikit-learn library.

---

# 📌 Problem Statement

Parkinson's disease is a progressive neurological disorder that primarily affects movement, speech, and motor control. Early diagnosis is important because timely treatment can help manage symptoms and improve the patient's quality of life.

Voice impairment is one of the earliest symptoms of Parkinson's disease. Biomedical voice measurements can therefore be used as input features for machine learning algorithms to assist in disease prediction.

The objective of this project is to build an accurate machine learning model capable of classifying whether a person has Parkinson's disease based on voice-related biomedical features.

---

# 🎯 Objectives

* Build a Parkinson's disease prediction model using Support Vector Machine (SVM)
* Perform data preprocessing and feature scaling
* Train and evaluate the machine learning model
* Predict disease status for new patient data
* Demonstrate a complete machine learning workflow from data loading to deployment-ready model saving

---

# 📂 Dataset Information

The dataset contains biomedical voice measurements collected from healthy individuals and Parkinson's disease patients.

Each record corresponds to one voice recording and contains multiple numerical features extracted from speech signals.

### Input Features

* MDVP:Fo(Hz)
* MDVP:Fhi(Hz)
* MDVP:Flo(Hz)
* MDVP:Jitter(%)
* MDVP:Jitter(Abs)
* MDVP:RAP
* MDVP:PPQ
* Jitter:DDP
* MDVP:Shimmer
* MDVP:Shimmer(dB)
* Shimmer:APQ3
* Shimmer:APQ5
* MDVP:APQ
* Shimmer:DDA
* NHR
* HNR
* RPDE
* DFA
* Spread1
* Spread2
* D2
* PPE

### Target Variable

| Value | Meaning             |
| ----- | ------------------- |
| 0     | Healthy Person      |
| 1     | Parkinson's Disease |

---

# 🛠️ Technologies Used

* Python
* Google Colab
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-learn
* Pickle

---

# 🤖 Machine Learning Algorithm

## Support Vector Machine (SVM)

This project uses the **Support Vector Machine (SVM)** classifier from Scikit-learn.

### Why SVM?

Support Vector Machine is a powerful supervised machine learning algorithm widely used for binary classification problems.

Advantages include:

* High classification accuracy
* Performs well on small and medium-sized datasets
* Effective in high-dimensional feature spaces
* Finds the optimal decision boundary that maximizes the margin between classes
* Less prone to overfitting when properly tuned

The implementation uses:

```python
SVC(kernel='linear')
```

---

# ⚙️ Project Workflow

### 1. Import Libraries

Import all required Python libraries.

---

### 2. Load Dataset

Read the Parkinson's dataset using Pandas.

---

### 3. Data Exploration

* Display dataset information
* Check missing values
* Understand feature distributions
* View statistical summary

---

### 4. Feature and Target Separation

Separate:

* Input Features (X)
* Target Labels (Y)

---

### 5. Train-Test Split

Split the dataset into training and testing sets.

Typical ratio:

* Training: 80%
* Testing: 20%

---

### 6. Feature Scaling

Standardize all numerical features using **StandardScaler**.

Feature scaling is essential because SVM is sensitive to differences in feature magnitudes.

---

### 7. Model Training

Train the Support Vector Machine classifier using the scaled training data.

---

### 8. Model Evaluation

Evaluate model performance using:

* Training Accuracy
* Testing Accuracy
* Confusion Matrix
* Classification Report

---

### 9. Prediction

Accept new biomedical voice measurements as input.

The model predicts:

* Healthy Person
* Parkinson's Disease

---

### 10. Model Saving

Save the trained model and scaler using Pickle.

Saved files:

* parkinson_model.pkl
* scaler.pkl

These files can later be loaded without retraining the model.

---

# 📁 Project Structure

```text
Parkinsons-Disease-Prediction-ML/
│
├── parkinson.ipynb
├── parkinsons.csv
├── README.md
├── requirements.txt
├── parkinson_model.pkl
└── scaler.pkl
```

---

# 📊 Evaluation Metrics

The model performance is evaluated using:

* Accuracy Score
* Confusion Matrix
* Precision
* Recall
* F1 Score
* Classification Report

These metrics help determine how effectively the SVM classifier distinguishes between healthy individuals and Parkinson's patients.

---

# 🚀 How to Run

## Clone Repository

```bash
git clone https://github.com/yourusername/Parkinsons-Disease-Prediction-ML.git
```

---

## Navigate to Project

```bash
cd Parkinsons-Disease-Prediction-ML
```

---

## Install Dependencies

```bash
pip install -r requirements.txt
```

---

## Run Notebook

```bash
jupyter notebook
```

or open directly in **Google Colab**.

---

# 📦 Requirements

```text
numpy
pandas
matplotlib
seaborn
scikit-learn
```

---

# 🔮 Future Improvements

* Compare SVM with Random Forest, XGBoost, and Logistic Regression
* Perform hyperparameter tuning using GridSearchCV
* Apply cross-validation for improved generalization
* Build an interactive web application using Streamlit or Flask
* Deploy the trained model to cloud platforms
* Integrate real-time voice recording for instant prediction
* Experiment with deep learning approaches for speech analysis

---

# 📚 Learning Outcomes

This project helped strengthen knowledge in:

* Data preprocessing
* Feature engineering
* Standardization using StandardScaler
* Support Vector Machine (SVM)
* Supervised Machine Learning
* Binary Classification
* Model evaluation techniques
* Machine learning inference
* Saving and loading trained models using Pickle

---

# 👨‍💻 Author

**Sanjay Saravanan**

B.Tech – Electronics and Communication Engineering (ECE)

VIT Chennai

---

# ⭐ If you found this project useful, consider giving the repository a star!
